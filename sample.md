# NCube.v2.0
 

## Controls.Charts.EthLogChartModel
            
CategoryChartControl에 사용하기 위한 Model
        
### *Properties*

#### Name
차트를 표현할 이름 CategoryChartControl에서는 콤보박스 Item에 표시됨
#### RxFramePoints
최대 값 리스트
#### RxFcsPoints
최소 값 리스트
### *Methods*


#### Constructor
CategoryChartControl에 사용하기 위한 Model
> ##### Parameters
> **name:** 차트를 표현할 이름

> **rxFrameList:** 최대 값

> **avrList:** 평균 값

> **rxFcsList:** 최소 값


## Controls.Charts.LogSeriesPoint
            
SeriesPoint 값 이외에 실제 값을 저장하기 위한 용도로 사용하는 클래스
        
### Properties

#### ActualDateTime
출력값의 실제 시간 값
#### ActualValue
출력 값의 실제 Value 값
### Methods


#### Constructor
SeriesPoint 값 이외에 실제 값을 저장하기 위한 용도로 사용하는 클래스
> ##### Parameters
> **argument:** x축 실제 시간

> **value:** y축 실제 값

> **viewArgument:** 보여질 x축 값

> **viewValue:** 보여질 y축 값


#### Constructor
SeriesPoint 값 이외에 실제 값을 저장하기 위한 용도로 사용하는 클래스 Value가 null이므로 차트에 공백으로 표시됩니다.
> ##### Parameters
> **argument:** x축 실제 시간

> **viewArgument:** 보여질 y축 값


## Controls.Charts.PieAreaChart
            
PieAreaChart.xaml에 대한 상호 작용 논리
            
PieAreaChart
        
### Methods


#### InitializeComponent
InitializeComponent

## Controls.Charts.CvLogChartControl
            
Interaction logic for CvLogChartControl.xaml
            
CvLogChartControl
        
### Fields

#### _enableZoom
Trackbar 이밴트와 Zoom 이밴트의 충돌을 막기 위한 용도
### Properties

#### MinViewValue
Y축에 최소로 보여줄 값을 설정합니다,
#### UasValueBrush
최대 값의 색을 설정
#### SesValueBrush
평균 값의 색을 설정
#### EsValueBrush
최소 값의 색을 설정
#### CvValueBrush
최소 값의 색을 설정
#### Items
현재 차트에 보여줄 Item들을 설정
#### CustomCrosshairTextAction
크로스헤어의 출력 값을 수정합니다.
### Methods


#### ShowChart
현재 적용된 값을 이용해 차트를 표현합니다.

#### ShowChart(NCube.Controls.Charts.CvLogChartModel)
현재 CvLogChartModel 적용된 값을 이용해 차트를 표현합니다.
> ##### Parameters
> **CvLogChartModel:** 적용할 CvLogChartModel


#### ResetAxisX(DevExpress.Xpf.Charts.XYDiagram2D)
X축을 초기로 리셋

#### RefreshLabel(DevExpress.Xpf.Charts.XYDiagram2D,DevExpress.Xpf.Charts.AxisX2D,System.String,System.String)
현재 크기에 맞추어 라벨 위치를 초기화 시킵니다.
> ##### Parameters
> **maxArg:** 최대 Argument 값

> **minArg:** 최소 Argment 값


#### LookUpEditBase_OnSelectedIndexChanged(System.Object,System.Windows.RoutedEventArgs)
콤보박스 Item이 변경되었을 때 동작합니다.
> ##### Parameters
> **sender:** 

> **e:** 


#### InitSeries(DevExpress.Xpf.Charts.XYSeries@,System.String,System.Collections.Generic.IEnumerable{DevExpress.Xpf.Charts.SeriesPoint},System.Windows.Media.SolidColorBrush)
그래프 선을 초기화 시킵니다.
> ##### Parameters
> **line:** 

> **crosshairName:** 

> **list:** 

> **brush:** 


#### InitStrackBarSeries(DevExpress.Xpf.Charts.XYSeries@,System.String,System.Collections.Generic.IEnumerable{DevExpress.Xpf.Charts.SeriesPoint},System.Windows.Media.SolidColorBrush)
그래프 선을 초기화 시킵니다.
> ##### Parameters
> **line:** 

> **crosshairName:** 

> **list:** 

> **brush:** 


#### SetChart2Range(System.Int32,System.Int32)
2번쨰 차트의 Y Range를 설정합니다.
> ##### Parameters
> **min:** 최소 값

> **max:** 최대 값


#### InitializeComponent
InitializeComponent

## Controls.Charts.EthLogChartControl
            
Interaction logic for EthLogChartControl.xaml
            
EthLogChartControl
        
### Fields

#### _enableZoom
Trackbar 이밴트와 Zoom 이밴트의 충돌을 막기 위한 용도
### Properties

#### MinViewValue
Y축에 최소로 보여줄 값을 설정합니다,
#### RxFrameValueBrush
최대 값의 색을 설정
#### RxFcsValueBrush
최소 값의 색을 설정
#### Items
현재 차트에 보여줄 Item들을 설정
#### CustomCrosshairTextAction
크로스헤어의 출력 값을 수정합니다.
### Methods


#### ShowChart
현재 적용된 값을 이용해 차트를 표현합니다.

#### ShowChart(NCube.Controls.Charts.EthLogChartModel)
현재 EthLogChartModel에 적용된 값을 이용해 차트를 표현합니다.
> ##### Parameters
> **chartModel:** 적용할 EthLogChartModel


#### ResetAxisX(DevExpress.Xpf.Charts.XYDiagram2D)
X축을 초기로 리셋

#### RefreshLabel(DevExpress.Xpf.Charts.XYDiagram2D,DevExpress.Xpf.Charts.AxisX2D,System.String,System.String)
현재 크기에 맞추어 라벨 위치를 초기화 시킵니다.
> ##### Parameters
> **maxArg:** 최대 Argument 값

> **minArg:** 최소 Argment 값


#### LookUpEditBase_OnSelectedIndexChanged(System.Object,System.Windows.RoutedEventArgs)
콤보박스 Item이 변경되었을 때 동작합니다.
> ##### Parameters
> **sender:** 

> **e:** 


#### InitSeries(DevExpress.Xpf.Charts.XYSeries@,System.String,System.Collections.Generic.IEnumerable{DevExpress.Xpf.Charts.SeriesPoint},System.Windows.Media.SolidColorBrush)
그래프 선을 초기화 시킵니다.
> ##### Parameters
> **line:** 

> **crosshairName:** 

> **list:** 

> **brush:** 


#### InitBarSeries(DevExpress.Xpf.Charts.XYSeries@,System.String,System.Collections.Generic.IEnumerable{DevExpress.Xpf.Charts.SeriesPoint},System.Windows.Media.SolidColorBrush)
그래프 선을 초기화 시킵니다.
> ##### Parameters
> **line:** 

> **crosshairName:** 

> **list:** 

> **brush:** 


#### InitializeComponent
InitializeComponent

## Controls.Charts.OtdrLogChartControl
            
Interaction logic for OtdrLogChartControl.xaml
            
OtdrLogChartControl
        
### Fields

#### _enableZoom
Trackbar 이밴트와 Zoom 이밴트의 충돌을 막기 위한 용도
### Properties

#### MinViewValue
Y축에 최소로 보여줄 값을 설정합니다,
#### BendValueBrush
최대 값의 색을 설정
#### ConnValueBrush
평균 값의 색을 설정
#### DistValueBrush
최소 값의 색을 설정
#### TotalValueBrush
OTDR 값의 색을 설정
#### Items
현재 차트에 보여줄 Item들을 설정
#### CustomCrosshairTextAction
크로스헤어의 출력 값을 수정합니다.
### Methods


#### ShowChart
현재 적용된 값을 이용해 차트를 표현합니다.

#### ShowChart(NCube.Controls.Charts.OtdrChartModel)
현재 OtdrChartModel 적용된 값을 이용해 차트를 표현합니다.
> ##### Parameters
> **OtdrLogChartModel:** 적용할 OtdrChartModel


#### ResetAxisX(DevExpress.Xpf.Charts.XYDiagram2D)
X축을 초기로 리셋

#### RefreshLabel(DevExpress.Xpf.Charts.XYDiagram2D,DevExpress.Xpf.Charts.AxisX2D,System.String,System.String)
현재 크기에 맞추어 라벨 위치를 초기화 시킵니다.
> ##### Parameters
> **maxArg:** 최대 Argument 값

> **minArg:** 최소 Argment 값


#### LookUpEditBase_OnSelectedIndexChanged(System.Object,System.Windows.RoutedEventArgs)
콤보박스 Item이 변경되었을 때 동작합니다.
> ##### Parameters
> **sender:** 

> **e:** 


#### InitSeries(DevExpress.Xpf.Charts.XYSeries@,System.String,System.Collections.Generic.IEnumerable{DevExpress.Xpf.Charts.SeriesPoint},System.Windows.Media.SolidColorBrush)
그래프 선을 초기화 시킵니다.
> ##### Parameters
> **line:** 

> **crosshairName:** 

> **list:** 

> **brush:** 


#### InitializeComponent
InitializeComponent

## Controls.Charts.OtdrSeriesPoint
            
SeriesPoint 값 이외에 실제 값을 저장하기 위한 용도로 사용하는 클래스
        
### Properties

#### ActualArgument
출력값의 실제 시간 값
#### ActualValue
출력 값의 실제 Value 값
### Methods


#### Constructor
SeriesPoint 값 이외에 실제 값을 저장하기 위한 용도로 사용하는 클래스
> ##### Parameters
> **argument:** x축 실제 시간

> **value:** y축 실제 값

> **viewArgument:** 보여질 x축 값

> **viewValue:** 보여질 y축 값


## Controls.Charts.OtdrTestChartControl
            
Interaction logic for OtdrTestChartControl.xaml
            
OtdrTestChartControl
        
### Fields

#### _enableZoom
Trackbar 이밴트와 Zoom 이밴트의 충돌을 막기 위한 용도
### Properties

#### MinViewValue
Y축에 최소로 보여줄 값을 설정합니다,
#### BendValueBrush
최대 값의 색을 설정
#### ConnValueBrush
평균 값의 색을 설정
#### DistValueBrush
최소 값의 색을 설정
#### Items
현재 차트에 보여줄 Item들을 설정
#### CustomCrosshairTextAction
크로스헤어의 출력 값을 수정합니다.
### Methods


#### ShowChart
현재 적용된 값을 이용해 차트를 표현합니다.

#### ShowChart(NCube.Controls.Charts.OtdrChartModel)
현재 OtdrChartModel에 적용된 값을 이용해 차트를 표현합니다.
> ##### Parameters
> **OtdrChartModel:** 적용할 OtdrChartModel


#### ResetAxisX
X축을 초기로 리셋

#### RefreshLabel(System.String,System.String)
현재 크기에 맞추어 라벨 위치를 초기화 시킵니다.
> ##### Parameters
> **maxArg:** 최대 Argument 값

> **minArg:** 최소 Argment 값


#### LookUpEditBase_OnSelectedIndexChanged(System.Object,System.Windows.RoutedEventArgs)
콤보박스 Item이 변경되었을 때 동작합니다.
> ##### Parameters
> **sender:** 

> **e:** 


#### InitSeries(DevExpress.Xpf.Charts.XYSeries@,System.String,System.Collections.Generic.IEnumerable{DevExpress.Xpf.Charts.SeriesPoint},System.Windows.Media.SolidColorBrush)
그래프 선을 초기화 시킵니다.
> ##### Parameters
> **line:** 

> **crosshairName:** 

> **list:** 

> **brush:** 


#### InitializeComponent
InitializeComponent

## Controls.Charts.BaseChartSeriesPoint
            
SeriesPoint 값 이외에 실제 값을 저장하기 위한 용도로 사용하는 클래스
        
### Properties

#### ActualDateTime
출력값의 실제 시간 값
#### ActualValue
출력 값의 실제 Value 값
### Methods


#### Constructor
SeriesPoint 값 이외에 실제 값을 저장하기 위한 용도로 사용하는 클래스
> ##### Parameters
> **argument:** x축 실제 시간

> **value:** y축 실제 값

> **viewArgument:** 보여질 x축 값

> **viewValue:** 보여질 y축 값


#### Constructor
SeriesPoint 값 이외에 실제 값을 저장하기 위한 용도로 사용하는 클래스 Value가 null이므로 차트에 공백으로 표시됩니다.
> ##### Parameters
> **argument:** x축 실제 시간

> **viewArgument:** 보여질 y축 값


## Controls.Charts.RealTimeLineSeries2D
            
RealTime 용도로 최적화된 Series 클래스
        
### Properties

#### MaxCount
실시간 그래프에 최대로 그릴 점들의 갯수
#### RealTimePoints
실시간 그래프 데이터
### Methods


#### Constructor
RealTime 용도로 최적화된 Series 클래스

## Controls.Charts.RealTimeLinePointModel
            
RealTimeLineSeries2D 에 사용할 데이터 클래스
        
### Methods


#### Constructor
RealTimeLineSeries2D 에 사용할 데이터 클래스
> ##### Parameters
> **argument:** X축 시간 값

> **value:** Y축 Value 값


## Controls.Charts.CategoryChartControl
            
Interaction logic for CategoryChartControl.xaml
            
CategoryChartControl
        
### Fields

#### _enableZoom
Trackbar 이밴트와 Zoom 이밴트의 충돌을 막기 위한 용도
### Properties

#### MinViewValue
Y축에 최소로 보여줄 값을 설정합니다,
#### MaxValueBrush
최대 값의 색을 설정
#### AverageValueBrush
평균 값의 색을 설정
#### MinValueBrush
최소 값의 색을 설정
#### Items
현재 차트에 보여줄 Item들을 설정
#### CustomCrosshairTextAction
크로스헤어의 출력 값을 수정합니다.
### Methods


#### ShowChart
현재 적용된 값을 이용해 차트를 표현합니다.

#### ShowChart(NCube.Controls.Charts.CategoryChartModel)
현재 categoryChartModel에 적용된 값을 이용해 차트를 표현합니다.
> ##### Parameters
> **categoryChartModel:** 적용할 CategoryChartModel


#### ResetAxisX
X축을 초기로 리셋

#### RefreshLabel(System.String,System.String)
현재 크기에 맞추어 라벨 위치를 초기화 시킵니다.
> ##### Parameters
> **maxArg:** 최대 Argument 값

> **minArg:** 최소 Argment 값


#### LookUpEditBase_OnSelectedIndexChanged(System.Object,System.Windows.RoutedEventArgs)
콤보박스 Item이 변경되었을 때 동작합니다.
> ##### Parameters
> **sender:** 

> **e:** 


#### InitSeries(DevExpress.Xpf.Charts.XYSeries@,System.String,System.Collections.Generic.IEnumerable{DevExpress.Xpf.Charts.SeriesPoint},System.Windows.Media.SolidColorBrush)
그래프 선을 초기화 시킵니다.
> ##### Parameters
> **line:** 

> **crosshairName:** 

> **list:** 

> **brush:** 


#### InitializeComponent
InitializeComponent

## Controls.Charts.CategoryChartModel
            
CategoryChartControl에 사용하기 위한 Model
        
### Properties

#### Name
차트를 표현할 이름 CategoryChartControl에서는 콤보박스 Item에 표시됨
#### MaxPoints
최대 값 리스트
#### AvrPoints
평균 값 리스트
#### MinPoints
최소 값 리스트
### Methods


#### Constructor
CategoryChartControl에 사용하기 위한 Model
> ##### Parameters
> **name:** 차트를 표현할 이름

> **maxList:** 최대 값

> **avrList:** 평균 값

> **minList:** 최소 값


## Controls.Charts.RealTimeChartControl
            
Interaction logic for RealTimeChartControl.xaml
            
RealTimeChartControl
        
### Properties

#### ThresholdViewType
Threshold를 표현할 방법을 선택합니다.
#### ValueViewType
차트 상에 표현되는 Data Type (아직 Runtime 상에서 변경되지 않습니다.)
#### IsNoDataVisibility
No Data로 그래프를 숨길지 여부를 결정합니다.
#### AlwaysShowZeroLevel
차트를 0에 고정할 것인지 아닌지 결정합니다.
#### AutoSideMargins
Y축 범위 위/아래로 margin을 자동으로 넣어줄 것인지를 결정합니다.
#### CustomCrosshairTextAction
크로스헤어의 출력 값을 수정합니다.
#### HighBiasValue
표현할 그래프 데이터에서 HighBiasValue 값 아래일 시, Y축을 기준으로 HighBiasValue 값을 고정시킴
#### LowBiasValue
표현할 그래프 데이터에서 LowBiasValue 값 높을 시, Y축을 기준으로 LowBiasValue 값을 고정시킴
### Methods


#### SetThresholdMax(System.Nullable{System.Double})
상위 임계치 값을 설정합니다.
> ##### Parameters
> **d:** 


#### SetThresholdMin(System.Nullable{System.Double})
최소 임계치 값을 설정합니다.
> ##### Parameters
> **d:** 


#### RefreshSeriesPoints
Series를 다시 표현합니다. HighBiasValue, LowBiasValue 값이 변경되었을 때 그래프 상에 보여질 ViewPoint가 변경되도록 합니다.

#### InitView
현재 차트 화면을 초기화 시킵니다.

#### RefreshAxisXLabel(System.String)
X축 라벨을 정리합니다.
> ##### Parameters
> **newestTimeStr:** 최신 시간 값


#### InitializeComponent
InitializeComponent

## Controls.Charts.RealTimeChartModel
            
RealTimeChartControl 에 사용할 모델
        
### Methods


#### Constructor
/// RealTimeChartControl 에 사용할 모델
> ##### Parameters
> **time:** X축 시간


## Controls.DisableControls
            
한번에 여러 컨트롤을 비활성화 시켜주는 헬퍼 클래스
        

## Controls.PageViews.MmiMsgBoxPageView
            
MmiMsgBoxPageView
        
### Methods


#### InitializeComponent
InitializeComponent

## Controls.PageViews.RdlRebootConfirmPopupPageView
            
RdlRebootConfirmPopupPageView
        
### Methods


#### InitializeComponent
InitializeComponent

## Controls.PageViews.ConfirmFlyPageView
            
ConfirmFlyPageView
        
### Methods


#### InitializeComponent
InitializeComponent

## Controls.PageViews.InputErrorFlyPageView
            
InputErrorFlyPageView
        
### Methods


#### InitializeComponent
InitializeComponent

## Controls.PageViews.InputNameFlyPageView
            
InputNameFlyPageView
        
### Methods


#### InitializeComponent
InitializeComponent

## Controls.PageViews.OkFlyPageView
            
OkFlyPageView
        
### Methods


#### InitializeComponent
InitializeComponent

## Controls.PageViews.UnderConstructionFlyPageView
            
UnderConstructionFlyPageView
        
### Methods


#### InitializeComponent
InitializeComponent

## Controls.PageViews.InitSysColdConfirmPopupPageView
            
InitSysColdConfirmPopupPageView
        
### Methods


#### InitializeComponent
InitializeComponent

## Controls.PageViews.SysCfgRestoreConfirmPopupPageView
            
SysCfgRestoreConfirmPopupPageView
        
### Methods


#### InitializeComponent
InitializeComponent

## Controls.PageViews.MsgBoxPopupPageView
            
MsgBoxPopupPageView
        
### Methods


#### InitializeComponent
InitializeComponent

## Controls.ProgressRingHolder
            
ProgressRing을 간단히 사용할 수 있게 도와주는 헬퍼 클래스
        

## Controls.Samples.SampleBox
            
Interaction logic for SampleBox.xaml
            
SampleBox
        
### Methods


#### InitializeComponent
InitializeComponent

## Controls.ScreenLock
            
투명하게 화면 잠금해주는 컨트롤
        

## Controls.Windows.ThemeWindow
            
Interaction logic for Window1.xaml
            
ThemeWindow
        
### Methods


#### InitializeComponent
InitializeComponent

## Controls.Buttons.AlarmClearButtons
            
AlarmClearButtons
        
### Methods


#### InitializeComponent
InitializeComponent

## Controls.Buttons.FilterOnOffButton
            
FilterOnOffButton
        
### Methods


#### InitializeComponent
InitializeComponent

## Controls.Buttons.OpenCloseButtons
            
OpenCloseButtons
        
### Properties

#### FilePath
파일 경로
### Methods


#### InitializeComponent
InitializeComponent

## Controls.Buttons.FlatButton
            
Interaction logic for FlatButton.xaml
            
FlatButton
        
### Properties

#### ItemBackground
ItemBackground
#### ItemForeground
ItemForeground
#### ProgressValue
ProgressValue
#### Status
버튼 상태
### Methods


#### Constructor
FlatButton

#### OnThemeChanged(System.Windows.DependencyObject,DevExpress.Xpf.Core.ThemeChangedRoutedEventArgs)
Runtime 상에서 Theme가 변경시에 동작
> ##### Parameters
> **sender:** 

> **e:** 


#### ColorConvert(System.Int32)
색상의 알파값을 변화시킵니다.
> ##### Parameters
> **convertValue:** 변화시키고자 하는 알파값

> ##### Return value
> 

#### InitializeComponent
InitializeComponent

## Controls.Buttons.FlatButton.ControlStatus
            
ControlStatus
        

## Controls.AlarmCountControl
            
Interaction logic for AlarmCountTemplate.xaml
            
AlarmCountControl
        
### Properties

#### IsHeaderVisiable
알람 Count위 Header를 표시할지 말지 결정합니다.
### Methods


#### InitializeComponent
InitializeComponent

## Controls.GSAlarmCountControl
            
Interaction logic for WorkingAlarmCountPanel.xaml
            
GSAlarmCountControl
        
### Methods


#### InitializeComponent
InitializeComponent

## Controls.GSGroupControl
            
Interaction logic for WorkingGroupTemplate.xaml
            
GSGroupControl
        
### Methods


#### InitializeComponent
InitializeComponent

## Controls.GSNodeControl
            
Interaction logic for WorkingNodeTemplate.xaml
            
GSNodeControl
        
### Methods


#### InitializeComponent
InitializeComponent

## Controls.Icons.ChartIcon
            
Interaction logic for ChartIcon.xaml
            
ChartIcon
        
### Methods


#### InitializeComponent
InitializeComponent

## Controls.Icons.LogIcon
            
Interaction logic for LogIcon.xaml
            
LogIcon
        
### Methods


#### InitializeComponent
InitializeComponent

## Controls.Icons.NetworkIcon
            
Interaction logic for NetworkIcon.xaml
            
NetworkIcon
        
### Methods


#### InitializeComponent
InitializeComponent

## Controls.Icons.OamIcon
            
Interaction logic for OamIcon.xaml
            
OamIcon
        
### Methods


#### InitializeComponent
InitializeComponent

## Controls.Icons.ProgressChartIcon
            
Interaction logic for ProgressChartIcon.xaml
            
ProgressChartIcon
        
### Methods


#### InitializeComponent
InitializeComponent

## Controls.Icons.WizardIcon
            
Interaction logic for WizardIcon.xaml
            
WizardIcon
        
### Methods


#### InitializeComponent
InitializeComponent

## Controls.LedControl
            
LedControl
        
### Properties

#### IsON
LED ON/OFF 여부
### Methods


#### InitializeComponent
InitializeComponent

## Controls.TableGraphTab
            
Interaction logic for TableGraphTab.xaml
            
TableGraphTab
        
### Methods


#### InitializeComponent
InitializeComponent

## Controls.Popups.FlatPopup
            
Interaction logic for FlatPopup.xaml
            
FlatPopup
        
### Methods


#### InitializeComponent
InitializeComponent

## Controls.Popups.Dialogs.InnerDialog
            
메인 윈도우 내부에 UserControl Dialog를 보여줍니다.
        
### Methods


#### Constructor
메인 윈도우 내부에 UserControl Dialog를 보여줍니다.
> ##### Parameters
> **content:** 보여줄 컨트롤 창

> **background:** 컨트롤 창의 배경을 설정, null로 설정시 White로 기본 지정합니다.


## Controls.Popups.Dialogs.MessageBoxPanel
            
Interaction logic for MessageBoxPanel.xaml
            
MessageBoxPanel
        
### Methods


#### GetResultAsync
result 결과를 EAP(Event-based Asynchronous Pattern) 대신에 TAP(Task-based Asynchronous Pattern)로 받습니다.
> ##### Return value
> 메세지 결과

#### InitializeComponent
InitializeComponent

## Controls.Popups.Dialogs.MessageBoxWindow
            
Interaction logic for MessageBoxWindow.xaml
            
MessageBoxWindow
        
### Methods


#### InitializeComponent
InitializeComponent

## Controls.Popups.Dialogs.SavedFileOpenWindow
            
Interaction logic for SavedFileOpenWindow.xaml
            
SavedFileOpenWindow
        
### Methods


#### InitializeComponent
InitializeComponent

## Controls.MetroProgressBar
            
MahApps.Metro Project UserControl A metrofied ProgressBar.
        
### Properties

#### EllipseDiameter
Gets/sets the diameter of the ellipses used in the indeterminate animation.
#### EllipseOffset
Gets/sets the offset of the ellipses used in the indeterminate animation.

## Controls.LoadingScreen
            
Interaction logic for LoadingScreen.xaml
            
LoadingScreen
        
### Methods


#### InitializeComponent
InitializeComponent

## Helpers.WindowLockHelper
            
MainWindow 화면 잠금 기능
            
        

## Novo.Core.Iris3Header
             
@brief IRIS3 PDU 헤더 IRIS3 PDU 헤더로서 20 octets 크기이다. IRIS3 PDU는 EMS와 장비간에 약속된 바이너리 규격으로서 다음과 같은 형태이다. @code IRIS3 PDU 일반 형식 +--------+---------------------+-----------------------+ | header | message 1 payload | message 2 payload | +--------+---------------------+-----------------------+ IRIS3 Request PDU 형식 1 +--------+------------+----------------+--------------+ | header | cmd_header | msg1 (str|bin) | msg2(opt) | +--------+------------+----------------+--------------+ header.msg_type := PTYPE_REQUEST header.msg1_style := PSTYLE_CMD (opt) header.msg2_style := ... IRIS3 Request PDU 형식 2 +--------+----------------------+---------------------+ | header | msg1(str|bin) | msg2(opt) | +--------+----------------------+---------------------+ header.msg_type := PTYPE_REQUEST header.msg1_style := PSTYLE_STRING | PSTYLE_BINARY | PSTYLE_BIN_CRS (opt) header.msg2_style := ... IRIS3 Response Packet Format +--------+---------------------+--------------------------+ | header | message 1 payload | message 2 payload(opt) | +--------+---------------------+--------------------------+ header.msg_type := PTYPE_RESPONSE header.msg1_style := PSTYLE_CALLA | PSTYLE_STRING | PSTYLE_BINARY | .. (opt) header.msg2_style := PSTYLE_BIN_STATUS, PSTYLE_BIN_CRS etc... IRIS3 Event Packet Format +--------+---------------------+--------------------------+ | header | message 1 payload | message 2 payload (opt) | +--------+---------------------+--------------------------+ header.msg_type := PTYPE_EVENT header.msg1_style := PSTYLE_CALLA | PSTYLE_STRING | PSTYLE_BINARY (opt) header.msg2_style := PSTYLE_BIN_STATUS, PSTYLE_BIN_CRS etc... IRIS3 Status Packet Format +--------+-------------------------------------------+ | header | message 1 payload (only binary) | +--------+-------------------------------------------+ header.msg_type := PTYPE_STATUS header.msg1_style := PSTYLE_BINARY header.msg2_style := PSTYPE_NONE header.msg2_length := 0 @endcode
        

## Services.Alarms.AlarmBuzzer
            
알람 소리를 내주는 클래스
        
### Methods


#### Constructor
알람 소리를 내주는 클래스

#### PlayOn(NCube.Services.Alarms.AlarmStatusType)
알람 소리를 재생합니다.
> ##### Parameters
> **sev:** 알람 경보 Type


#### PlayOn(System.String)
알람 소리를 재생합니다.
> ##### Parameters
> **filePath:** 파일 경로


## Services.ActionResultType
            
Action 수행 응답 body 타입
        
### Fields

#### None
응답 body가 없을때
#### Kai
응답 body가 kai 객체
#### Calla
응답 body가 calla 객체
#### Json
응답 body가 json 객체
#### Datatable
응답 body가 dataTable 객체 (sqlite용)

## Services.ActionResult
            
서비스 action 수행시 리턴 타입 Content는 Type 속성에 따라 달라진다.
        
### Fields

#### 
응답 body가 없을때
#### 
응답 body가 kai 객체
#### 
응답 body가 calla 객체
#### 
응답 body가 json 객체
#### 
응답 body가 dataTable 객체 (sqlite용)

## Services.Audit.DefaultAuditMessage
            
AUDIT 메시지. 기본은 STD.AUDIT.PUSH 프로시저 호출
        

## Services.Audit.JsonAuditMessage
            
AUDIT 메시지 (JSON 형식). 만약 JSON 형식의 요청이라면 참고바람
        

## Services.Audit.DefaultAuditServiceAction
            
AUDIT 수행 기본 action. STD.AUDIT.PUSH 명령어를 보내고 끝.
        

## Services.Audit.AuditServiceActionAsync
            
AUDIT 수행 기본 action (Async 버전). STD.AUDIT.PUSH 명령어를 보내고, 수행 완료되면 리턴.
        

## Services.Audit.JsonAuditServiceAction
            
AUDIT 수행 JSON action. JSON 형태로 audit push 요청을 보낸다
        

## Services.Audit.JsonAuditServiceActionAsync
            
AUDIT 수행 JSON action (Async 버전). JSON 형태로 audit push 요청을 보내고, 수행 완료되면 리턴.
        

## Services.Audit.AuditService
            
AUDIT 서비스 클래스.
        

## Services.Threading.TimedLock
            
Class provides a nice way of obtaining a lock that will time out with a cleaner syntax than using the whole Monitor.TryEnter() method.
            
Adapted from Ian Griffiths article http://www.interact-sw.co.uk/iangblog/2004/03/23/locking and incorporating suggestions by Marek Malowidzki as outlined in this blog post http://www.interact-sw.co.uk/iangblog/2004/05/12/timedlockstacktrace
            
            Instead of:
            
```

            lock(obj)
            {
                //Thread safe operation
            }
            
            do this:
            
            using(TimedLock.Lock(obj))
            {
                //Thread safe operations
            }
            
            or this:
            
            try
            {
                TimedLock timeLock = TimedLock.Lock(obj);
                //Thread safe operations
                timeLock.Dispose();
            }
            catch(LockTimeoutException e)
            {
                Console.WriteLine("Couldn't get a lock!");
                StackTrace otherStack = e.GetBlockingThreadStackTrace(5000);
                if(otherStack == null)
                {
                    Console.WriteLine("Couldn't get other stack!");
                }
                else
                {
                    Console.WriteLine("Stack trace of thread that owns lock!");
                }
            }
            ```
            
        
### Methods


#### Lock(System.Object)
Attempts to obtain a lock on the specified object for up to 10 seconds.
> ##### Parameters
> **o:** 

> ##### Return value
> 

#### Lock(System.Object,System.TimeSpan)
Attempts to obtain a lock on the specified object for up to the specified timeout.
> ##### Parameters
> **o:** 

> **timeout:** 

> ##### Return value
> 

#### Dispose
Disposes of this lock.

## Services.Threading.LockTimeoutException
            
Thrown when a lock times out.
        
### Methods


#### ReportStackTraceIfError(System.Object)
Sets the stack trace for the given lock target if an error occurred.
> ##### Parameters
> **lockTarget:** Lock target.


#### Constructor
Use this exception.
Creates a new instance.
> ##### Parameters
> **lockTarget:** Object we tried to lock.


#### GetBlockingStackTrace(System.Int32)
Stack trace of the thread that holds a lock on the object this lock is attempting to acquire when it fails.
> ##### Parameters
> **timeout:** Number of milliseconds to wait for the blocking stack trace.


#### Constructor
Creates a new instance.

#### Constructor
Constructor.
> ##### Parameters
> **message:** 


#### Constructor
Constructor.
> ##### Parameters
> **message:** 

> **innerException:** 


#### Constructor
Constructor.
> ##### Parameters
> **info:** 

> **context:** 


#### ToString
Returns a string representation of the exception.
> ##### Return value
> 

## Services.Threading.UndisposedLockException
            
This exception indicates that a user of the TimedLock struct failed to leave a Monitor. This could be the result of a deadlock or forgetting to use the using statement or a try finally block.
        
### Methods


#### Constructor
Constructor.
> ##### Parameters
> **message:** 


#### Constructor
Special constructor used for deserialization.
> ##### Parameters
> **info:** 

> **context:** 


## Services.Threading.OneShotTimerHelper
                    밀리초 대기 후, Action을 수행하게 해주는 타이머 헬퍼. 
            
                    @example 
                    public void Test()
                    {
                        // 생성자 직접 호출 방식 
                        new OneShotTimer(()=>{ }, 10);
               
                        // 헬퍼 클래스 사용하는 방식 
                        OneShotTimerHelper.Start(()=>{ }, 1000);
                        
                        // 헬퍼 클래스 사용하는 방식 (Stop이 필요한 경우)
                        var timer = OneShotTimerHelper.Start(()=>{ }, 1000);
                        timer.Stop();
                    }
            
                    @Author : Uk 
                    @Date : 2016-07-21 
        

## Services.Report.HohCellModel
            
DataTable의 Cell을 담는 데이터 클래스입니다.
        
### Fields

#### CommonFont
CellModel에 기본으로 지정된 폰트입니다. 글꼴 : "Segoe UI" 크기 : 10
### Properties

#### Value
Cell에 저장된 값
#### Font
Cell의 폰트

## Services.Report.HohColumn
            
Model을 DataTable로 변경하기 위한 클래스
        
### Properties

#### Header
Column의 헤더 이름
#### FieldName
입력하고자하는 Property 이름
#### WidthRatio
기본 값은 1입니다. 프린트에만 적용이 됩니다.

## Services.Report.HohDataColumn
            
DataTable의 DataColumn에 넓이 비율을 만들어주기 위한 클래스
        
### Properties

#### WidthRatio
프린트에 쓰일 넓이 비율
#### Font
Cell의 폰트

## Services.Report.HohReportPrinter
            
프린트를 만들기 위한 클래스
        
### Methods


#### Clear
초기화합니다.

#### Add(NCube.Services.Report.HohSheetModel)
프린트할 데이터를 추가합니다. Add한 순서대로 출력됩니다.
> ##### Parameters
> **HohSheetModel:** 출력할 HohSheetModel


#### ShowPreviewDialog
PreviewDialog를 보여줍니다.

#### CreateDocumentAsync(System.Threading.CancellationToken)
문서를 비동기로 생성합니다.
> ##### Parameters
> **token:** 취소 토큰

> ##### Return value
> 비동기 Task

## Services.Report.HohReportTemplate
            
프린트를 출력하기 위한 템플릿
        
### Fields

#### components
Required designer variable.
### Properties

#### TitleMargin
타이틀과 Content 사이 여백
### Methods


#### Constructor
Progress를 사용이 HohReportPrinter와 밀접하므로 충돌 방지를 위해 internal로 관리함
> ##### Parameters
> **progress:** 


#### InsertData(NCube.Services.Report.HohSheetModel,System.Threading.CancellationToken)
문서 내부에 표현할 데이터 값을 넣습니다. Task 취소시, OperationCanceledException 예외가 발생합니다.
> ##### Parameters
> **HohSheetModel:** 입력할 데이터

> **token:** 취소 토큰


#### TestView
테스트를 위한 뷰입니다.

#### Dispose(System.Boolean)
Clean up any resources being used.
> ##### Parameters
> **disposing:** true if managed resources should be disposed; otherwise, false.


#### InitializeComponent
Required method for Designer support - do not modify the contents of this method with the code editor.

## Services.Report.HohSheetControl
            
UI의 Control을 캡쳐하는 클래스입니다.
        
### Methods


#### Constructor
캡쳐하기 위한 컨트롤을 넣습니다.
> ##### Parameters
> **control:** 캡처할 Control 클래스


#### FindChild``1(System.Windows.DependencyObject,System.String)
Finds a Child of a given item in the visual tree. 참고 소스코드 : http://stackoverflow.com/questions/636383/how-can-i-find-wpf-controls-by-name-or-type
> ##### Parameters
> **parent:** A direct parent of the queried item.

> **childName:** x:Name or Name of child.

> ##### Return value
> The first parent item that matches the submitted type parameter. If not matching item can be found, a null parent is being returned.

## Services.Report.HohSheetModel
            
표로 넣기 위한 데이터
        
### Fields

#### CommonTitleFont
HohSheetData에 기본으로 지정된 폰트입니다. 글꼴 : "Segoe UI" 크기 : 12 스타일 : Bold
#### CommonHeaderCommentFont
HohSheetData에 기본으로 지정된 폰트입니다. 글꼴 : "Segoe UI" 크기 : 10

## Services.Report.HohSheetProgressArgs
            
Sheet 처리에 대한 이밴트값들
        
### Properties

#### CurrentRows
처리된 현재 Rows 값
#### CurrentImages
처리된 현재 Images 값

## Services.Report.HohSheetTable
            
List를 Table로 변경하는 클래스
        
### Fields

#### TableTypes.GridControl
일반적인 테이블 형태
#### TableTypes.TreeKey
Tree로 표현된 경우, Tree를 각각의 컬럼으로 표시
#### TableTypes.TreeKeyCombineView
Tree로 표현된 경우, Tree를 하나의 컬럼으로 표시
### Methods


#### Constructor
List를 Table로 변경시켜주는 클래스
> ##### Parameters
> **itemsSource:** 출력할 List

> **tableType:** 출력할 타입

> **keyField:** Key의 Property 이름

> **parentKeyField:** ParentKey의 Property 이름

> **treeField:** Tree일 경우, Tree 구조를 결정하는 Key Property이름

> **treeHeader:** Tree Key를 표에 출력할 이름


#### BuildDataTableAsync
Table 데이터로 변환합니다.
> ##### Return value
> 변환된 DataTable

#### BuildDataTableAsync(System.Threading.CancellationToken)
Table 데이터로 변환합니다.
> ##### Parameters
> **token:** 취소

> ##### Return value
> 변환된 DataTable

## Services.Report.HohSpreadSheet
            
데이터 타입을 엑셀로 변환시켜주는 클래스 내부적으로 사용하는 클래스가 UI 쓰레드를 필요하므로, 반드시 코드 생성시에 UI 쓰레드 내에서 생성해야 합니다.
        
### Methods


#### Constructor
데이터 타입을 엑셀로 변환시켜주는 클래스

#### Add(NCube.Services.Report.HohSheetModel)
SpreadSheet에 HohSheetData를 추가합니다. 생성하려면 반드시 CreateSheet 혹은 CreateSheetAsync를 동작시켜야 합니다.
> ##### Parameters
> **HohSheetModel:** 추가하고자 하는 Sheet


#### CreateSheet(System.Threading.CancellationToken)
Sheet를 생성합니다.

#### CreateSheetAsync
Sheet를 비동기로 생성합니다.
> ##### Return value
> 

#### CreateSheetAsync(System.Threading.CancellationToken)
Sheet를 비동기로 생성합니다.
> ##### Parameters
> **token:** 취소 토큰

> ##### Return value
> 

## Properties.Resources
            
A strongly-typed resource class, for looking up localized strings, etc.
        
### Properties

#### ResourceManager
Returns the cached ResourceManager instance used by this class.
#### Culture
Overrides the current thread's CurrentUICulture property for all resource lookups using this strongly typed resource class.

## GeneratedInternalTypeHelper
            
GeneratedInternalTypeHelper
        
### Methods


#### CreateInstance(System.Type,System.Globalization.CultureInfo)
CreateInstance

#### GetPropertyValue(System.Reflection.PropertyInfo,System.Object,System.Globalization.CultureInfo)
GetPropertyValue

#### SetPropertyValue(System.Reflection.PropertyInfo,System.Object,System.Object,System.Globalization.CultureInfo)
SetPropertyValue

#### CreateDelegate(System.Type,System.Object,System.String)
CreateDelegate

#### AddEventHandler(System.Reflection.EventInfo,System.Object,System.Delegate)
AddEventHandler