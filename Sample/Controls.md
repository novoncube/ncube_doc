# NCube 2.0

## Summary

### Controls
---
#### AlarmCountControl
![](Controls_AlarmCountControl.gif)
##### 컨트롤 목적
- 
##### 샘플 코드
```xaml
<nvctrl:AlarmCountControl Width="100" Height="50"
                              CriticalAlarmCount="4" MajorAlarmCount="5" MinorAlarmCount="3" Margin="20" IsHeaderVisiable="{Binding IsChecked, ElementName=TBTN_IsHeaderVisiable}"/>
``` 
```cs

```



---
#### GSGroupControl
![](Controls_GSGroupControl.gif)
##### 컨트롤 목적
- 
##### 샘플 코드
```xaml
<nvctrl:GSGroupControl Margin="10"
                               AlarmStatus="{Binding SelectedItem.Tag, ElementName=CB_AlarmStatusType}"
                               CriticalAlarmCount="4"
                               GroupName="{Binding Text, ElementName=TB_GroupName}"
                               IsVisiable="{Binding IsChecked, ElementName=TBTN_IsHeaderVisiable}"
                               MajorAlarmCount="5" MinorAlarmCount="3" />
``` 
```cs

```



---
#### GSNodeControl
![](Controls_GSNodeControl.gif)
##### 컨트롤 목적
- 
##### 샘플 코드
```xaml
<nvctrl:GSNodeControl AlarmStatus="{Binding SelectedItem.Tag, ElementName=CB_AlarmStatusType}"
                            CriticalAlarmCount="4"
                            IsVisiable="{Binding IsChecked, ElementName=TBTN_IsHeaderVisiable}"
                            MajorAlarmCount="5" MinorAlarmCount="3"
                            NodeName="{Binding Text, ElementName=TB_NodeName}" />
``` 
```cs

```



---
#### LedControl
![](Controls_LedControl.gif)
##### 컨트롤 목적
- 
##### 샘플 코드
```xaml
<nvctrl:LedControl IsON="{Binding IsChecked, ElementName=TBTN_IsOn}" Color="{Binding SelectedItem.Tag, ElementName=CB_SelectColor}" Margin="20"/>
``` 
```cs

```



---
#### MetroProgressBar
![](Controls_MetroProgressBar.gif)
##### 컨트롤 목적
- 
##### 샘플 코드
```xaml
<nvctrl:MetroProgressBar Width="100" Height="100"
                                 Margin="20"
                                 Foreground="{Binding SelectedItem.Tag, ElementName=CB_Background}"
                                 IsIndeterminate="{Binding IsChecked, ElementName=TBTN_IsIndeterminate}" />
``` 
```cs

```



---
#### ProgressRing
![](Controls_ProgressRing.gif)
##### 컨트롤 목적
- 
##### 샘플 코드
```xaml
<nvctrl:ProgressRing Width="50" Height="50"
                               IsActive="{Binding IsChecked, ElementName=TBTN_IsActive}" Foreground="{Binding SelectedItem.Tag, ElementName=CB_Background}" Margin="20"/>
``` 
```cs

```



---
#### TableGraphTab
![](Controls_TableGraphTab.gif)
##### 컨트롤 목적
- 
##### 샘플 코드
```xaml
<nvctrl:TableGraphTab FindClick="TableGraphTab_OnFindClick" GraphViewSelected="TableGraphTab_OnGraphViewSelected" TableViewSelected="TableGraphTab_OnTableViewSelected" Margin="20"/>
``` 
```cs
private void TableGraphTab_OnTableViewSelected(object sender, EventArgs e)
{
    TB_Show.Text = "OnTableViewSelected";
}

private void TableGraphTab_OnGraphViewSelected(object sender, EventArgs e)
{
    TB_Show.Text = "OnGraphViewSelected";
}

private void TableGraphTab_OnFindClick(object sender, EventArgs e)
{
    TB_Show.Text = "OnFindClick";
}
```