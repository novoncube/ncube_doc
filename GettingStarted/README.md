# NCube 2.0

## Getting Started

### 기본적인 설정 방법

1. NCube Project와 NCube.Themes.FlatWhite 를 Add Reference합니다.

2. App.xaml에 아래와 같이 코드를 삽입합니다.

```xml
<Application.Resources>
    <ResourceDictionary>
        <ResourceDictionary.MergedDictionaries>
        <!-- 아래의 코드를 삽입하세요 -->
        <ResourceDictionary Source="pack://application:,,,/NCube.Themes.FlatWhite.v2.0;component/Themes/Generic.xaml" />
        <ResourceDictionary Source="pack://application:,,,/NCube.v2.0;component/ControlResources/Generic.xaml" />
        <!-- end -->
        </ResourceDictionary.MergedDictionaries>
    </ResourceDictionary>
</Application.Resources>
```

3. MainWindow.xaml의 스타일을 아래의 코드를 삽입하면, NCube 기본 메인 윈도우가 Window 테마로 변경됩니다.
```
Style="{DynamicResource NCube.DXWindowTheme}"
```


---
### NCubeStartup 을 이용한 방법

1. AppStartup.cs 클래스를 하나 만듭니다.

2. AppStartup 클래스에 NCubeStartup를 상속받아 작성합니다. 예제로, 아래와 같이 샘플 코드를 구성합니다.

```cs
using GalaSoft.MvvmLight.Ioc;
using Microsoft.Practices.ServiceLocation;
using NCube.Builder;
using NCube.Services.Alarms;

namespace NCube.Sample.Report
{
    public class AppStartup : NCubeStartup
    {
        public override void Build(NCubeBuilder builder)
        {
            // Theme를 적용합니다.
            builder.UseTheme(NCubeThemeSelector.FlatWhite);

            // NCube 내에서 사용할 ServiceLocator를 설정합니다. 
            ServiceLocator.SetLocatorProvider(() => SimpleIoc.Default);
            SimpleIoc.Default.Register<IAlarmSeverityMethods, DefaultAlarmSeverityMethods>();
        }
    }
}
```

3. App.xaml에서 Startup 이밴트를 생성하고, AppStartup를 리소스로 등록합니다.

```xml
<Application x:Class="NCube.Sample.Report.App"
             xmlns="http://schemas.microsoft.com/winfx/2006/xaml/presentation"
             xmlns:x="http://schemas.microsoft.com/winfx/2006/xaml"
             xmlns:local="clr-namespace:NCube.Sample.Report"
             StartupUri="MainWindow.xaml" Startup="App_OnStartup">
  <Application.Resources>
    <local:AppStartup x:Key="builder"/>
  </Application.Resources>
</Application>
```

4. App.xaml에서 생성한 App_OnStartup 이밴트를 아래와 같이 실행시킵니다.

```cs
using System.Reflection;
using System.Windows;

namespace NCube.Sample.Report
{
    public partial class App : Application
    {
        private void App_OnStartup(object sender, StartupEventArgs e)
        {
            AppStartup.Start();
        }
    }
}
```

5. 나머지는 위 [기본적인 설정 방법]의 3번대로 사용하면 됩니다.

**#질문** [기본적인 설정 방법]보다 [NCubeStartup을 이용한 방법]이 좋은 이유가 있나요?

**#답변** [기본적인 설정 방법]을 이용하시면, Xaml Designer에서 Preview를 동작시키는데 일부 에러가 있을 수 있습니다. (다행히도 실행하거나 프로그래밍 하시는데에는 큰 무리가 없습니다) NCubeStartup을 사용하시면, Preview 시에도 에러가 나지 않도록 필요한 실행코드를 Resource에 등록하여 사용하도록 합니다. 만약 Preview에 에러가 난다면 ServiceLocator를 제대로 등록하지 않은 문제일 것입니다.


---
### NCubeStartup 을 이용한 방법2

1. 위 [NCubeStartup 을 이용한 방법] 1~3번을 따라합니다.

2. 아래의 샘플과 같이 구현합니다. builder를 이용해 NCube 스타일이 입혀진 메인 Window를 실행시키는 코드입니다. Frame은 App에서 제작된 MainWindow에 올릴 Panel인 UserControl입니다.

```cs
using System.Reflection;
using System.Windows;

namespace NCube.Sample.Report
{
    public partial class App : Application
    {
        private void App_OnStartup(object sender, StartupEventArgs e)
        {
            var builder = AppStartup.Start();
            builder.StartUp(new NCubeSetting(new Frame())
            {
                Title = Assembly.GetEntryAssembly().GetName().Name,
                Width = 1200,
                Height = 600
            });
        }
    }
}

```

**#주의** 이 방법은 MainWindow에 대한 Customize가 어려울 수 있습니다. 