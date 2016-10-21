# NCube.v2.0 #

##### Property NCube.Controls.Charts.CvLogChartModel.Name

 @brief IRIS3 PDU 헤더 IRIS3 PDU 헤더로서 20 octets 크기이다. IRIS3 PDU는 EMS와 장비간에 약속된 바이너리 규격으로서 다음과 같은 형태이다. @code IRIS3 PDU 일반 형식 +--------+---------------------+-----------------------+ | header | message 1 payload | message 2 payload | +--------+---------------------+-----------------------+ IRIS3 Request PDU 형식 1 +--------+------------+----------------+--------------+ | header | cmd_header | msg1 (str|bin) | msg2(opt) | +--------+------------+----------------+--------------+ header.msg_type := PTYPE_REQUEST header.msg1_style := PSTYLE_CMD (opt) header.msg2_style := ... IRIS3 Request PDU 형식 2 +--------+----------------------+---------------------+ | header | msg1(str|bin) | msg2(opt) | +--------+----------------------+---------------------+ header.msg_type := PTYPE_REQUEST header.msg1_style := PSTYLE_STRING | PSTYLE_BINARY | PSTYLE_BIN_CRS (opt) header.msg2_style := ... IRIS3 Response Packet Format +--------+---------------------+--------------------------+ | header | message 1 payload | message 2 payload(opt) | +--------+---------------------+--------------------------+ header.msg_type := PTYPE_RESPONSE header.msg1_style := PSTYLE_CALLA | PSTYLE_STRING | PSTYLE_BINARY | .. (opt) header.msg2_style := PSTYLE_BIN_STATUS, PSTYLE_BIN_CRS etc... IRIS3 Event Packet Format +--------+---------------------+--------------------------+ | header | message 1 payload | message 2 payload (opt) | +--------+---------------------+--------------------------+ header.msg_type := PTYPE_EVENT header.msg1_style := PSTYLE_CALLA | PSTYLE_STRING | PSTYLE_BINARY (opt) header.msg2_style := PSTYLE_BIN_STATUS, PSTYLE_BIN_CRS etc... IRIS3 Status Packet Format +--------+-------------------------------------------+ | header | message 1 payload (only binary) | +--------+-------------------------------------------+ header.msg_type := PTYPE_STATUS header.msg1_style := PSTYLE_BINARY header.msg2_style := PSTYPE_NONE header.msg2_length := 0 @endcode 




##### Property NCube.Controls.Charts.CvLogChartModel.UasPoints

 최대 값 리스트 




##### Property NCube.Controls.Charts.CvLogChartModel.SesPoints

 평균 값 리스트 




##### Property NCube.Controls.Charts.CvLogChartModel.EsPoints

 최소 값 리스트 




##### Property NCube.Controls.Charts.CvLogChartModel.CvPoints

 최소 값 리스트 




##### Method NCube.Controls.Charts.CvLogChartModel.#ctor(System.String,System.Collections.Generic.IEnumerable{DevExpress.Xpf.Charts.SeriesPoint},System.Collections.Generic.IEnumerable{DevExpress.Xpf.Charts.SeriesPoint},System.Collections.Generic.IEnumerable{DevExpress.Xpf.Charts.SeriesPoint},System.Collections.Generic.IEnumerable{DevExpress.Xpf.Charts.SeriesPoint})

 CategoryChartControl에 사용하기 위한 Model 

|Name | Description |
|-----|------|
|name: |차트를 표현할 이름|
|uasList: |최대 값|
|sesList: |평균 값|
|esList: |최소 값|



---
# Type NCube.Controls.Charts.EthLogChartModel

 CategoryChartControl에 사용하기 위한 Model 




##### Property NCube.Controls.Charts.EthLogChartModel.Name

 차트를 표현할 이름 CategoryChartControl에서는 콤보박스 Item에 표시됨 




##### Property NCube.Controls.Charts.EthLogChartModel.RxFramePoints

 최대 값 리스트 




##### Property NCube.Controls.Charts.EthLogChartModel.RxFcsPoints

 최소 값 리스트 




##### Method NCube.Controls.Charts.EthLogChartModel.#ctor(System.String,System.Collections.Generic.IEnumerable{DevExpress.Xpf.Charts.SeriesPoint},System.Collections.Generic.IEnumerable{DevExpress.Xpf.Charts.SeriesPoint})

 CategoryChartControl에 사용하기 위한 Model 

|Name | Description |
|-----|------|
|name: |차트를 표현할 이름|
|rxFrameList: |최대 값|
|avrList: |평균 값|
|rxFcsList: |최소 값|



##### Property NCube.Controls.Charts.OtdrChartModel.Name

 차트를 표현할 이름 CategoryChartControl에서는 콤보박스 Item에 표시됨 




##### Property NCube.Controls.Charts.OtdrChartModel.BendPoints

 최대 값 리스트 




##### Property NCube.Controls.Charts.OtdrChartModel.ConnPoints

 평균 값 리스트 




##### Property NCube.Controls.Charts.OtdrChartModel.DistPoints

 최소 값 리스트 




##### Property NCube.Controls.Charts.OtdrChartModel.TotalPoints

 최소 값 리스트 




##### Method NCube.Controls.Charts.OtdrChartModel.#ctor(System.String,System.Collections.Generic.IEnumerable{DevExpress.Xpf.Charts.SeriesPoint},System.Collections.Generic.IEnumerable{DevExpress.Xpf.Charts.SeriesPoint},System.Collections.Generic.IEnumerable{DevExpress.Xpf.Charts.SeriesPoint},System.Collections.Generic.IEnumerable{DevExpress.Xpf.Charts.SeriesPoint})

 CategoryChartControl에 사용하기 위한 Model 

|Name | Description |
|-----|------|
|name: |차트를 표현할 이름|
|bendList: |최대 값|
|connList: |평균 값|
|distList: |최소 값|



---
# Type NCube.Controls.Charts.LogSeriesPoint

 SeriesPoint 값 이외에 실제 값을 저장하기 위한 용도로 사용하는 클래스 




##### Method NCube.Controls.Charts.LogSeriesPoint.#ctor(System.String,System.DateTime,System.Nullable{System.Double},System.String,System.Double)

 SeriesPoint 값 이외에 실제 값을 저장하기 위한 용도로 사용하는 클래스 

|Name | Description |
|-----|------|
|argument: |x축 실제 시간|
|value: |y축 실제 값|
|viewArgument: |보여질 x축 값|
|viewValue: |보여질 y축 값|



##### Method NCube.Controls.Charts.LogSeriesPoint.#ctor(System.String,System.DateTime,System.String)

 SeriesPoint 값 이외에 실제 값을 저장하기 위한 용도로 사용하는 클래스 Value가 null이므로 차트에 공백으로 표시됩니다. 

|Name | Description |
|-----|------|
|argument: |x축 실제 시간|
|viewArgument: |보여질 y축 값|



##### Property NCube.Controls.Charts.LogSeriesPoint.ActualDateTime

 출력값의 실제 시간 값 




##### Property NCube.Controls.Charts.LogSeriesPoint.ActualValue

 출력 값의 실제 Value 값 




---
# Type NCube.Controls.Charts.PieAreaChart

 PieAreaChart.xaml에 대한 상호 작용 논리 

 PieAreaChart 




##### Method NCube.Controls.Charts.PieAreaChart.InitializeComponent

 InitializeComponent 




---
# Type NCube.Controls.Charts.CvLogChartControl

 Interaction logic for CvLogChartControl.xaml 

 CvLogChartControl 




##### Property NCube.Controls.Charts.CvLogChartControl.MinViewValue

 Y축에 최소로 보여줄 값을 설정합니다, 




##### Property NCube.Controls.Charts.CvLogChartControl.UasValueBrush

 최대 값의 색을 설정 




##### Property NCube.Controls.Charts.CvLogChartControl.SesValueBrush

 평균 값의 색을 설정 




##### Property NCube.Controls.Charts.CvLogChartControl.EsValueBrush

 최소 값의 색을 설정 




##### Property NCube.Controls.Charts.CvLogChartControl.CvValueBrush

 최소 값의 색을 설정 




##### Property NCube.Controls.Charts.CvLogChartControl.Items

 현재 차트에 보여줄 Item들을 설정 




##### Property NCube.Controls.Charts.CvLogChartControl.CustomCrosshairTextAction

 크로스헤어의 출력 값을 수정합니다. 




##### Method NCube.Controls.Charts.CvLogChartControl.ShowChart

 현재 적용된 값을 이용해 차트를 표현합니다. 




##### Method NCube.Controls.Charts.CvLogChartControl.ShowChart(NCube.Controls.Charts.CvLogChartModel)

 현재 CvLogChartModel 적용된 값을 이용해 차트를 표현합니다. 

|Name | Description |
|-----|------|
|CvLogChartModel: |적용할 CvLogChartModel|



##### Method NCube.Controls.Charts.CvLogChartControl.ResetAxisX(DevExpress.Xpf.Charts.XYDiagram2D)

 X축을 초기로 리셋 




##### Method NCube.Controls.Charts.CvLogChartControl.RefreshLabel(DevExpress.Xpf.Charts.XYDiagram2D,DevExpress.Xpf.Charts.AxisX2D,System.String,System.String)

 현재 크기에 맞추어 라벨 위치를 초기화 시킵니다. 

|Name | Description |
|-----|------|
|maxArg: |최대 Argument 값|
|minArg: |최소 Argment 값|



##### Method NCube.Controls.Charts.CvLogChartControl.LookUpEditBase_OnSelectedIndexChanged(System.Object,System.Windows.RoutedEventArgs)

 콤보박스 Item이 변경되었을 때 동작합니다. 

|Name | Description |
|-----|------|
|sender: ||
|e: ||



##### Method NCube.Controls.Charts.CvLogChartControl.InitSeries(DevExpress.Xpf.Charts.XYSeries@,System.String,System.Collections.Generic.IEnumerable{DevExpress.Xpf.Charts.SeriesPoint},System.Windows.Media.SolidColorBrush)

 그래프 선을 초기화 시킵니다. 

|Name | Description |
|-----|------|
|line: ||
|crosshairName: ||
|list: ||
|brush: ||



##### Method NCube.Controls.Charts.CvLogChartControl.InitStrackBarSeries(DevExpress.Xpf.Charts.XYSeries@,System.String,System.Collections.Generic.IEnumerable{DevExpress.Xpf.Charts.SeriesPoint},System.Windows.Media.SolidColorBrush)

 그래프 선을 초기화 시킵니다. 

|Name | Description |
|-----|------|
|line: ||
|crosshairName: ||
|list: ||
|brush: ||



##### Method NCube.Controls.Charts.CvLogChartControl.SetChart2Range(System.Int32,System.Int32)

 2번쨰 차트의 Y Range를 설정합니다. 

|Name | Description |
|-----|------|
|min: |최소 값|
|max: |최대 값|



##### Field NCube.Controls.Charts.CvLogChartControl._enableZoom

 Trackbar 이밴트와 Zoom 이밴트의 충돌을 막기 위한 용도 




##### Method NCube.Controls.Charts.CvLogChartControl.InitializeComponent

 InitializeComponent 




---
# Type NCube.Controls.Charts.EthLogChartControl

 Interaction logic for EthLogChartControl.xaml 

 EthLogChartControl 




##### Property NCube.Controls.Charts.EthLogChartControl.MinViewValue

 Y축에 최소로 보여줄 값을 설정합니다, 




##### Property NCube.Controls.Charts.EthLogChartControl.RxFrameValueBrush

 최대 값의 색을 설정 




##### Property NCube.Controls.Charts.EthLogChartControl.RxFcsValueBrush

 최소 값의 색을 설정 




##### Property NCube.Controls.Charts.EthLogChartControl.Items

 현재 차트에 보여줄 Item들을 설정 




##### Property NCube.Controls.Charts.EthLogChartControl.CustomCrosshairTextAction

 크로스헤어의 출력 값을 수정합니다. 




##### Method NCube.Controls.Charts.EthLogChartControl.ShowChart

 현재 적용된 값을 이용해 차트를 표현합니다. 




##### Method NCube.Controls.Charts.EthLogChartControl.ShowChart(NCube.Controls.Charts.EthLogChartModel)

 현재 EthLogChartModel에 적용된 값을 이용해 차트를 표현합니다. 

|Name | Description |
|-----|------|
|chartModel: |적용할 EthLogChartModel|



##### Method NCube.Controls.Charts.EthLogChartControl.ResetAxisX(DevExpress.Xpf.Charts.XYDiagram2D)

 X축을 초기로 리셋 




##### Method NCube.Controls.Charts.EthLogChartControl.RefreshLabel(DevExpress.Xpf.Charts.XYDiagram2D,DevExpress.Xpf.Charts.AxisX2D,System.String,System.String)

 현재 크기에 맞추어 라벨 위치를 초기화 시킵니다. 

|Name | Description |
|-----|------|
|maxArg: |최대 Argument 값|
|minArg: |최소 Argment 값|



##### Method NCube.Controls.Charts.EthLogChartControl.LookUpEditBase_OnSelectedIndexChanged(System.Object,System.Windows.RoutedEventArgs)

 콤보박스 Item이 변경되었을 때 동작합니다. 

|Name | Description |
|-----|------|
|sender: ||
|e: ||



##### Method NCube.Controls.Charts.EthLogChartControl.InitSeries(DevExpress.Xpf.Charts.XYSeries@,System.String,System.Collections.Generic.IEnumerable{DevExpress.Xpf.Charts.SeriesPoint},System.Windows.Media.SolidColorBrush)

 그래프 선을 초기화 시킵니다. 

|Name | Description |
|-----|------|
|line: ||
|crosshairName: ||
|list: ||
|brush: ||



##### Method NCube.Controls.Charts.EthLogChartControl.InitBarSeries(DevExpress.Xpf.Charts.XYSeries@,System.String,System.Collections.Generic.IEnumerable{DevExpress.Xpf.Charts.SeriesPoint},System.Windows.Media.SolidColorBrush)

 그래프 선을 초기화 시킵니다. 

|Name | Description |
|-----|------|
|line: ||
|crosshairName: ||
|list: ||
|brush: ||



##### Field NCube.Controls.Charts.EthLogChartControl._enableZoom

 Trackbar 이밴트와 Zoom 이밴트의 충돌을 막기 위한 용도 




##### Method NCube.Controls.Charts.EthLogChartControl.InitializeComponent

 InitializeComponent 




---
# Type NCube.Controls.Charts.OtdrLogChartControl

 Interaction logic for OtdrLogChartControl.xaml 

 OtdrLogChartControl 




##### Property NCube.Controls.Charts.OtdrLogChartControl.MinViewValue

 Y축에 최소로 보여줄 값을 설정합니다, 




##### Property NCube.Controls.Charts.OtdrLogChartControl.BendValueBrush

 최대 값의 색을 설정 




##### Property NCube.Controls.Charts.OtdrLogChartControl.ConnValueBrush

 평균 값의 색을 설정 




##### Property NCube.Controls.Charts.OtdrLogChartControl.DistValueBrush

 최소 값의 색을 설정 




##### Property NCube.Controls.Charts.OtdrLogChartControl.TotalValueBrush

 OTDR 값의 색을 설정 




##### Property NCube.Controls.Charts.OtdrLogChartControl.Items

 현재 차트에 보여줄 Item들을 설정 




##### Property NCube.Controls.Charts.OtdrLogChartControl.CustomCrosshairTextAction

 크로스헤어의 출력 값을 수정합니다. 




##### Method NCube.Controls.Charts.OtdrLogChartControl.ShowChart

 현재 적용된 값을 이용해 차트를 표현합니다. 




##### Method NCube.Controls.Charts.OtdrLogChartControl.ShowChart(NCube.Controls.Charts.OtdrChartModel)

 현재 OtdrChartModel 적용된 값을 이용해 차트를 표현합니다. 

|Name | Description |
|-----|------|
|OtdrLogChartModel: |적용할 OtdrChartModel|



##### Method NCube.Controls.Charts.OtdrLogChartControl.ResetAxisX(DevExpress.Xpf.Charts.XYDiagram2D)

 X축을 초기로 리셋 




##### Method NCube.Controls.Charts.OtdrLogChartControl.RefreshLabel(DevExpress.Xpf.Charts.XYDiagram2D,DevExpress.Xpf.Charts.AxisX2D,System.String,System.String)

 현재 크기에 맞추어 라벨 위치를 초기화 시킵니다. 

|Name | Description |
|-----|------|
|maxArg: |최대 Argument 값|
|minArg: |최소 Argment 값|



##### Method NCube.Controls.Charts.OtdrLogChartControl.LookUpEditBase_OnSelectedIndexChanged(System.Object,System.Windows.RoutedEventArgs)

 콤보박스 Item이 변경되었을 때 동작합니다. 

|Name | Description |
|-----|------|
|sender: ||
|e: ||



##### Method NCube.Controls.Charts.OtdrLogChartControl.InitSeries(DevExpress.Xpf.Charts.XYSeries@,System.String,System.Collections.Generic.IEnumerable{DevExpress.Xpf.Charts.SeriesPoint},System.Windows.Media.SolidColorBrush)

 그래프 선을 초기화 시킵니다. 

|Name | Description |
|-----|------|
|line: ||
|crosshairName: ||
|list: ||
|brush: ||



##### Field NCube.Controls.Charts.OtdrLogChartControl._enableZoom

 Trackbar 이밴트와 Zoom 이밴트의 충돌을 막기 위한 용도 




##### Method NCube.Controls.Charts.OtdrLogChartControl.InitializeComponent

 InitializeComponent 




---
# Type NCube.Controls.Charts.OtdrSeriesPoint

 SeriesPoint 값 이외에 실제 값을 저장하기 위한 용도로 사용하는 클래스 




##### Method NCube.Controls.Charts.OtdrSeriesPoint.#ctor(System.Double,System.Nullable{System.Double},System.Double)

 SeriesPoint 값 이외에 실제 값을 저장하기 위한 용도로 사용하는 클래스 

|Name | Description |
|-----|------|
|argument: |x축 실제 시간|
|value: |y축 실제 값|
|viewArgument: |보여질 x축 값|
|viewValue: |보여질 y축 값|



##### Property NCube.Controls.Charts.OtdrSeriesPoint.ActualArgument

 출력값의 실제 시간 값 




##### Property NCube.Controls.Charts.OtdrSeriesPoint.ActualValue

 출력 값의 실제 Value 값 




---
# Type NCube.Controls.Charts.OtdrTestChartControl

 Interaction logic for OtdrTestChartControl.xaml 

 OtdrTestChartControl 




##### Property NCube.Controls.Charts.OtdrTestChartControl.MinViewValue

 Y축에 최소로 보여줄 값을 설정합니다, 




##### Property NCube.Controls.Charts.OtdrTestChartControl.BendValueBrush

 최대 값의 색을 설정 




##### Property NCube.Controls.Charts.OtdrTestChartControl.ConnValueBrush

 평균 값의 색을 설정 




##### Property NCube.Controls.Charts.OtdrTestChartControl.DistValueBrush

 최소 값의 색을 설정 




##### Property NCube.Controls.Charts.OtdrTestChartControl.Items

 현재 차트에 보여줄 Item들을 설정 




##### Property NCube.Controls.Charts.OtdrTestChartControl.CustomCrosshairTextAction

 크로스헤어의 출력 값을 수정합니다. 




##### Method NCube.Controls.Charts.OtdrTestChartControl.ShowChart

 현재 적용된 값을 이용해 차트를 표현합니다. 




##### Method NCube.Controls.Charts.OtdrTestChartControl.ShowChart(NCube.Controls.Charts.OtdrChartModel)

 현재 OtdrChartModel에 적용된 값을 이용해 차트를 표현합니다. 

|Name | Description |
|-----|------|
|OtdrChartModel: |적용할 OtdrChartModel|



##### Method NCube.Controls.Charts.OtdrTestChartControl.ResetAxisX

 X축을 초기로 리셋 




##### Method NCube.Controls.Charts.OtdrTestChartControl.RefreshLabel(System.String,System.String)

 현재 크기에 맞추어 라벨 위치를 초기화 시킵니다. 

|Name | Description |
|-----|------|
|maxArg: |최대 Argument 값|
|minArg: |최소 Argment 값|



##### Method NCube.Controls.Charts.OtdrTestChartControl.LookUpEditBase_OnSelectedIndexChanged(System.Object,System.Windows.RoutedEventArgs)

 콤보박스 Item이 변경되었을 때 동작합니다. 

|Name | Description |
|-----|------|
|sender: ||
|e: ||



##### Method NCube.Controls.Charts.OtdrTestChartControl.InitSeries(DevExpress.Xpf.Charts.XYSeries@,System.String,System.Collections.Generic.IEnumerable{DevExpress.Xpf.Charts.SeriesPoint},System.Windows.Media.SolidColorBrush)

 그래프 선을 초기화 시킵니다. 

|Name | Description |
|-----|------|
|line: ||
|crosshairName: ||
|list: ||
|brush: ||



##### Field NCube.Controls.Charts.OtdrTestChartControl._enableZoom

 Trackbar 이밴트와 Zoom 이밴트의 충돌을 막기 위한 용도 




##### Method NCube.Controls.Charts.OtdrTestChartControl.InitializeComponent

 InitializeComponent 




---
# Type NCube.Controls.Charts.BaseChartSeriesPoint

 SeriesPoint 값 이외에 실제 값을 저장하기 위한 용도로 사용하는 클래스 




##### Method NCube.Controls.Charts.BaseChartSeriesPoint.#ctor(System.DateTime,System.Nullable{System.Double},System.String,System.Double)

 SeriesPoint 값 이외에 실제 값을 저장하기 위한 용도로 사용하는 클래스 

|Name | Description |
|-----|------|
|argument: |x축 실제 시간|
|value: |y축 실제 값|
|viewArgument: |보여질 x축 값|
|viewValue: |보여질 y축 값|



##### Method NCube.Controls.Charts.BaseChartSeriesPoint.#ctor(System.DateTime,System.String)

 SeriesPoint 값 이외에 실제 값을 저장하기 위한 용도로 사용하는 클래스 Value가 null이므로 차트에 공백으로 표시됩니다. 

|Name | Description |
|-----|------|
|argument: |x축 실제 시간|
|viewArgument: |보여질 y축 값|



##### Property NCube.Controls.Charts.BaseChartSeriesPoint.ActualDateTime

 출력값의 실제 시간 값 




##### Property NCube.Controls.Charts.BaseChartSeriesPoint.ActualValue

 출력 값의 실제 Value 값 




---
# Type NCube.Controls.Charts.RealTimeLineSeries2D

 RealTime 용도로 최적화된 Series 클래스 




##### Property NCube.Controls.Charts.RealTimeLineSeries2D.MaxCount

 실시간 그래프에 최대로 그릴 점들의 갯수 




##### Property NCube.Controls.Charts.RealTimeLineSeries2D.RealTimePoints

 실시간 그래프 데이터 




##### Method NCube.Controls.Charts.RealTimeLineSeries2D.#ctor

 RealTime 용도로 최적화된 Series 클래스 




---
# Type NCube.Controls.Charts.RealTimeLinePointModel

 RealTimeLineSeries2D 에 사용할 데이터 클래스 




##### Method NCube.Controls.Charts.RealTimeLinePointModel.#ctor(System.DateTime,System.Nullable{System.Double})

 RealTimeLineSeries2D 에 사용할 데이터 클래스 

|Name | Description |
|-----|------|
|argument: |X축 시간 값|
|value: |Y축 Value 값|



---
# Type NCube.Controls.Charts.CategoryChartControl

 Interaction logic for CategoryChartControl.xaml 

 CategoryChartControl 




##### Property NCube.Controls.Charts.CategoryChartControl.MinViewValue

 Y축에 최소로 보여줄 값을 설정합니다, 




##### Property NCube.Controls.Charts.CategoryChartControl.MaxValueBrush

 최대 값의 색을 설정 




##### Property NCube.Controls.Charts.CategoryChartControl.AverageValueBrush

 평균 값의 색을 설정 




##### Property NCube.Controls.Charts.CategoryChartControl.MinValueBrush

 최소 값의 색을 설정 




##### Property NCube.Controls.Charts.CategoryChartControl.Items

 현재 차트에 보여줄 Item들을 설정 




##### Property NCube.Controls.Charts.CategoryChartControl.CustomCrosshairTextAction

 크로스헤어의 출력 값을 수정합니다. 




##### Method NCube.Controls.Charts.CategoryChartControl.ShowChart

 현재 적용된 값을 이용해 차트를 표현합니다. 




##### Method NCube.Controls.Charts.CategoryChartControl.ShowChart(NCube.Controls.Charts.CategoryChartModel)

 현재 categoryChartModel에 적용된 값을 이용해 차트를 표현합니다. 

|Name | Description |
|-----|------|
|categoryChartModel: |적용할 CategoryChartModel|



##### Method NCube.Controls.Charts.CategoryChartControl.ResetAxisX

 X축을 초기로 리셋 




##### Method NCube.Controls.Charts.CategoryChartControl.RefreshLabel(System.String,System.String)

 현재 크기에 맞추어 라벨 위치를 초기화 시킵니다. 

|Name | Description |
|-----|------|
|maxArg: |최대 Argument 값|
|minArg: |최소 Argment 값|



##### Method NCube.Controls.Charts.CategoryChartControl.LookUpEditBase_OnSelectedIndexChanged(System.Object,System.Windows.RoutedEventArgs)

 콤보박스 Item이 변경되었을 때 동작합니다. 

|Name | Description |
|-----|------|
|sender: ||
|e: ||



##### Method NCube.Controls.Charts.CategoryChartControl.InitSeries(DevExpress.Xpf.Charts.XYSeries@,System.String,System.Collections.Generic.IEnumerable{DevExpress.Xpf.Charts.SeriesPoint},System.Windows.Media.SolidColorBrush)

 그래프 선을 초기화 시킵니다. 

|Name | Description |
|-----|------|
|line: ||
|crosshairName: ||
|list: ||
|brush: ||



##### Field NCube.Controls.Charts.CategoryChartControl._enableZoom

 Trackbar 이밴트와 Zoom 이밴트의 충돌을 막기 위한 용도 




##### Method NCube.Controls.Charts.CategoryChartControl.InitializeComponent

 InitializeComponent 




---
# Type NCube.Controls.Charts.CategoryChartModel

 CategoryChartControl에 사용하기 위한 Model 




##### Property NCube.Controls.Charts.CategoryChartModel.Name

 차트를 표현할 이름 CategoryChartControl에서는 콤보박스 Item에 표시됨 




##### Property NCube.Controls.Charts.CategoryChartModel.MaxPoints

 최대 값 리스트 




##### Property NCube.Controls.Charts.CategoryChartModel.AvrPoints

 평균 값 리스트 




##### Property NCube.Controls.Charts.CategoryChartModel.MinPoints

 최소 값 리스트 




##### Method NCube.Controls.Charts.CategoryChartModel.#ctor(System.String,System.Collections.Generic.IEnumerable{DevExpress.Xpf.Charts.SeriesPoint},System.Collections.Generic.IEnumerable{DevExpress.Xpf.Charts.SeriesPoint},System.Collections.Generic.IEnumerable{DevExpress.Xpf.Charts.SeriesPoint})

 CategoryChartControl에 사용하기 위한 Model 

|Name | Description |
|-----|------|
|name: |차트를 표현할 이름|
|maxList: |최대 값|
|avrList: |평균 값|
|minList: |최소 값|



---
# Type NCube.Controls.Charts.RealTimeChartControl

 Interaction logic for RealTimeChartControl.xaml 

 RealTimeChartControl 




##### Property NCube.Controls.Charts.RealTimeChartControl.ThresholdViewType

 Threshold를 표현할 방법을 선택합니다. 




##### Property NCube.Controls.Charts.RealTimeChartControl.ValueViewType

 차트 상에 표현되는 Data Type (아직 Runtime 상에서 변경되지 않습니다.) 




##### Property NCube.Controls.Charts.RealTimeChartControl.IsNoDataVisibility

 No Data로 그래프를 숨길지 여부를 결정합니다. 




##### Property NCube.Controls.Charts.RealTimeChartControl.AlwaysShowZeroLevel

 차트를 0에 고정할 것인지 아닌지 결정합니다. 




##### Property NCube.Controls.Charts.RealTimeChartControl.AutoSideMargins

 Y축 범위 위/아래로 margin을 자동으로 넣어줄 것인지를 결정합니다. 




##### Property NCube.Controls.Charts.RealTimeChartControl.CustomCrosshairTextAction

 크로스헤어의 출력 값을 수정합니다. 




##### Property NCube.Controls.Charts.RealTimeChartControl.HighBiasValue

 표현할 그래프 데이터에서 HighBiasValue 값 아래일 시, Y축을 기준으로 HighBiasValue 값을 고정시킴 




##### Property NCube.Controls.Charts.RealTimeChartControl.LowBiasValue

 표현할 그래프 데이터에서 LowBiasValue 값 높을 시, Y축을 기준으로 LowBiasValue 값을 고정시킴 




##### Method NCube.Controls.Charts.RealTimeChartControl.SetThresholdMax(System.Nullable{System.Double})

 상위 임계치 값을 설정합니다. 

|Name | Description |
|-----|------|
|d: ||



##### Method NCube.Controls.Charts.RealTimeChartControl.SetThresholdMin(System.Nullable{System.Double})

 최소 임계치 값을 설정합니다. 

|Name | Description |
|-----|------|
|d: ||



##### Method NCube.Controls.Charts.RealTimeChartControl.RefreshSeriesPoints

 Series를 다시 표현합니다. HighBiasValue, LowBiasValue 값이 변경되었을 때 그래프 상에 보여질 ViewPoint가 변경되도록 합니다. 




##### Method NCube.Controls.Charts.RealTimeChartControl.InitView

 현재 차트 화면을 초기화 시킵니다. 




##### Method NCube.Controls.Charts.RealTimeChartControl.RefreshAxisXLabel(System.String)

 X축 라벨을 정리합니다. 

|Name | Description |
|-----|------|
|newestTimeStr: |최신 시간 값|



##### Method NCube.Controls.Charts.RealTimeChartControl.InitializeComponent

 InitializeComponent 




---
# Type NCube.Controls.Charts.RealTimeChartModel

 RealTimeChartControl 에 사용할 모델 




##### Method NCube.Controls.Charts.RealTimeChartModel.#ctor(System.DateTime)

 /// RealTimeChartControl 에 사용할 모델 

|Name | Description |
|-----|------|
|time: |X축 시간|



---
# Type NCube.Controls.DisableControls

 한번에 여러 컨트롤을 비활성화 시켜주는 헬퍼 클래스 




---
# Type NCube.Controls.PageViews.MmiMsgBoxPageView

 MmiMsgBoxPageView 




##### Method NCube.Controls.PageViews.MmiMsgBoxPageView.InitializeComponent

 InitializeComponent 




---
# Type NCube.Controls.PageViews.RdlRebootConfirmPopupPageView

 RdlRebootConfirmPopupPageView 




##### Method NCube.Controls.PageViews.RdlRebootConfirmPopupPageView.InitializeComponent

 InitializeComponent 




---
# Type NCube.Controls.PageViews.ConfirmFlyPageView

 ConfirmFlyPageView 




##### Method NCube.Controls.PageViews.ConfirmFlyPageView.InitializeComponent

 InitializeComponent 




---
# Type NCube.Controls.PageViews.InputErrorFlyPageView

 InputErrorFlyPageView 




##### Method NCube.Controls.PageViews.InputErrorFlyPageView.InitializeComponent

 InitializeComponent 




---
# Type NCube.Controls.PageViews.InputNameFlyPageView

 InputNameFlyPageView 




##### Method NCube.Controls.PageViews.InputNameFlyPageView.InitializeComponent

 InitializeComponent 




---
# Type NCube.Controls.PageViews.OkFlyPageView

 OkFlyPageView 




##### Method NCube.Controls.PageViews.OkFlyPageView.InitializeComponent

 InitializeComponent 




---
# Type NCube.Controls.PageViews.UnderConstructionFlyPageView

 UnderConstructionFlyPageView 




##### Method NCube.Controls.PageViews.UnderConstructionFlyPageView.InitializeComponent

 InitializeComponent 




---
# Type NCube.Controls.PageViews.InitSysColdConfirmPopupPageView

 InitSysColdConfirmPopupPageView 




##### Method NCube.Controls.PageViews.InitSysColdConfirmPopupPageView.InitializeComponent

 InitializeComponent 




---
# Type NCube.Controls.PageViews.SysCfgRestoreConfirmPopupPageView

 SysCfgRestoreConfirmPopupPageView 




##### Method NCube.Controls.PageViews.SysCfgRestoreConfirmPopupPageView.InitializeComponent

 InitializeComponent 




---
# Type NCube.Controls.PageViews.MsgBoxPopupPageView

 MsgBoxPopupPageView 




##### Method NCube.Controls.PageViews.MsgBoxPopupPageView.InitializeComponent

 InitializeComponent 




---
# Type NCube.Controls.ProgressRingHolder

 ProgressRing을 간단히 사용할 수 있게 도와주는 헬퍼 클래스 




---
# Type NCube.Controls.Samples.SampleBox

 Interaction logic for SampleBox.xaml 

 SampleBox 




##### Method NCube.Controls.Samples.SampleBox.InitializeComponent

 InitializeComponent 




---
# Type NCube.Controls.ScreenLock

 투명하게 화면 잠금해주는 컨트롤 




---
# Type NCube.Controls.Windows.ThemeWindow

 Interaction logic for Window1.xaml 

 ThemeWindow 




##### Method NCube.Controls.Windows.ThemeWindow.InitializeComponent

 InitializeComponent 




---
# Type NCube.Controls.Buttons.AlarmClearButtons

 AlarmClearButtons 




##### Event NCube.Controls.Buttons.AlarmClearButtons.ClickClearRls

 해제된 보고 삭제 




##### Event NCube.Controls.Buttons.AlarmClearButtons.ClickClearAll

 전체 삭제 




##### Method NCube.Controls.Buttons.AlarmClearButtons.InitializeComponent

 InitializeComponent 




---
# Type NCube.Controls.Buttons.FilterOnOffButton

 FilterOnOffButton 




##### Event NCube.Controls.Buttons.FilterOnOffButton.Click

 Click 




##### Method NCube.Controls.Buttons.FilterOnOffButton.InitializeComponent

 InitializeComponent 




---
# Type NCube.Controls.Buttons.OpenCloseButtons

 OpenCloseButtons 




##### Property NCube.Controls.Buttons.OpenCloseButtons.FilePath

 파일 경로 




##### Method NCube.Controls.Buttons.OpenCloseButtons.InitializeComponent

 InitializeComponent 




---
# Type NCube.Controls.Buttons.FlatButton

 Interaction logic for FlatButton.xaml 

 FlatButton 




##### Property NCube.Controls.Buttons.FlatButton.ItemBackground

 ItemBackground 




##### Property NCube.Controls.Buttons.FlatButton.ItemForeground

 ItemForeground 




##### Property NCube.Controls.Buttons.FlatButton.ProgressValue

 ProgressValue 




##### Method NCube.Controls.Buttons.FlatButton.#ctor

 FlatButton 




##### Method NCube.Controls.Buttons.FlatButton.OnThemeChanged(System.Windows.DependencyObject,DevExpress.Xpf.Core.ThemeChangedRoutedEventArgs)

 Runtime 상에서 Theme가 변경시에 동작 

|Name | Description |
|-----|------|
|sender: ||
|e: ||



##### Method NCube.Controls.Buttons.FlatButton.ColorConvert(System.Int32)

 색상의 알파값을 변화시킵니다. 

|Name | Description |
|-----|------|
|convertValue: |변화시키고자 하는 알파값|
**Returns**: 




---
# Type NCube.Controls.Buttons.FlatButton.ControlStatus

 ControlStatus 




##### Property NCube.Controls.Buttons.FlatButton.Status

 버튼 상태 




##### Method NCube.Controls.Buttons.FlatButton.InitializeComponent

 InitializeComponent 




---
# Type NCube.Controls.AlarmCountControl

 Interaction logic for AlarmCountTemplate.xaml 

 AlarmCountControl 




##### Property NCube.Controls.AlarmCountControl.IsHeaderVisiable

 알람 Count위 Header를 표시할지 말지 결정합니다. 




##### Method NCube.Controls.AlarmCountControl.InitializeComponent

 InitializeComponent 




---
# Type NCube.Controls.GSAlarmCountControl

 Interaction logic for WorkingAlarmCountPanel.xaml 

 GSAlarmCountControl 




##### Method NCube.Controls.GSAlarmCountControl.InitializeComponent

 InitializeComponent 




---
# Type NCube.Controls.GSGroupControl

 Interaction logic for WorkingGroupTemplate.xaml 

 GSGroupControl 




##### Method NCube.Controls.GSGroupControl.InitializeComponent

 InitializeComponent 




---
# Type NCube.Controls.GSNodeControl

 Interaction logic for WorkingNodeTemplate.xaml 

 GSNodeControl 




##### Method NCube.Controls.GSNodeControl.InitializeComponent

 InitializeComponent 




---
# Type NCube.Controls.Icons.ChartIcon

 Interaction logic for ChartIcon.xaml 

 ChartIcon 




##### Method NCube.Controls.Icons.ChartIcon.InitializeComponent

 InitializeComponent 




---
# Type NCube.Controls.Icons.LogIcon

 Interaction logic for LogIcon.xaml 

 LogIcon 




##### Method NCube.Controls.Icons.LogIcon.InitializeComponent

 InitializeComponent 




---
# Type NCube.Controls.Icons.NetworkIcon

 Interaction logic for NetworkIcon.xaml 

 NetworkIcon 




##### Method NCube.Controls.Icons.NetworkIcon.InitializeComponent

 InitializeComponent 




---
# Type NCube.Controls.Icons.OamIcon

 Interaction logic for OamIcon.xaml 

 OamIcon 




##### Method NCube.Controls.Icons.OamIcon.InitializeComponent

 InitializeComponent 




---
# Type NCube.Controls.Icons.ProgressChartIcon

 Interaction logic for ProgressChartIcon.xaml 

 ProgressChartIcon 




##### Method NCube.Controls.Icons.ProgressChartIcon.InitializeComponent

 InitializeComponent 




---
# Type NCube.Controls.Icons.WizardIcon

 Interaction logic for WizardIcon.xaml 

 WizardIcon 




##### Method NCube.Controls.Icons.WizardIcon.InitializeComponent

 InitializeComponent 




---
# Type NCube.Controls.LedControl

 LedControl 




##### Property NCube.Controls.LedControl.IsON

 LED ON/OFF 여부 




##### Method NCube.Controls.LedControl.InitializeComponent

 InitializeComponent 




---
# Type NCube.Controls.TableGraphTab

 Interaction logic for TableGraphTab.xaml 

 TableGraphTab 




##### Method NCube.Controls.TableGraphTab.InitializeComponent

 InitializeComponent 




---
# Type NCube.Controls.Popups.FlatPopup

 Interaction logic for FlatPopup.xaml 

 FlatPopup 




##### Method NCube.Controls.Popups.FlatPopup.InitializeComponent

 InitializeComponent 




---
# Type NCube.Controls.Popups.Dialogs.InnerDialog

 메인 윈도우 내부에 UserControl Dialog를 보여줍니다. 




##### Method NCube.Controls.Popups.Dialogs.InnerDialog.#ctor(System.Windows.Controls.Control,System.Windows.Media.Brush)

 메인 윈도우 내부에 UserControl Dialog를 보여줍니다. 

|Name | Description |
|-----|------|
|content: |보여줄 컨트롤 창|
|background: |컨트롤 창의 배경을 설정, null로 설정시 White로 기본 지정합니다.|



---
# Type NCube.Controls.Popups.Dialogs.MessageBoxPanel

 Interaction logic for MessageBoxPanel.xaml 

 MessageBoxPanel 




##### Event NCube.Controls.Popups.Dialogs.MessageBoxPanel.ResultEvent

 버튼 이밴트 후, 결과 값 이밴트 




##### Method NCube.Controls.Popups.Dialogs.MessageBoxPanel.GetResultAsync

 result 결과를 EAP(Event-based Asynchronous Pattern) 대신에 TAP(Task-based Asynchronous Pattern)로 받습니다. 

**Returns**: 메세지 결과




##### Method NCube.Controls.Popups.Dialogs.MessageBoxPanel.InitializeComponent

 InitializeComponent 




---
# Type NCube.Controls.Popups.Dialogs.MessageBoxWindow

 Interaction logic for MessageBoxWindow.xaml 

 MessageBoxWindow 




##### Event NCube.Controls.Popups.Dialogs.MessageBoxWindow.ResultEvent

 버튼 이밴트 후, 결과 값 이밴트 




##### Method NCube.Controls.Popups.Dialogs.MessageBoxWindow.InitializeComponent

 InitializeComponent 




---
# Type NCube.Controls.Popups.Dialogs.SavedFileOpenWindow

 Interaction logic for SavedFileOpenWindow.xaml 

 SavedFileOpenWindow 




##### Event NCube.Controls.Popups.Dialogs.SavedFileOpenWindow.ResultEvent

 버튼 이밴트 후, 결과 값 이밴트 




##### Method NCube.Controls.Popups.Dialogs.SavedFileOpenWindow.InitializeComponent

 InitializeComponent 




---
# Type NCube.Controls.MetroProgressBar

 MahApps.Metro Project UserControl A metrofied ProgressBar. [[|T:System.Windows.Controls.ProgressBar]]




##### Property NCube.Controls.MetroProgressBar.EllipseDiameter

 Gets/sets the diameter of the ellipses used in the indeterminate animation. 




##### Property NCube.Controls.MetroProgressBar.EllipseOffset

 Gets/sets the offset of the ellipses used in the indeterminate animation. 




---
# Type NCube.Controls.LoadingScreen

 Interaction logic for LoadingScreen.xaml 

 LoadingScreen 




##### Method NCube.Controls.LoadingScreen.InitializeComponent

 InitializeComponent 




##### Method NCube.Helpers.EncodingHelper.StringFromUtf8(System.String)

 managed UTF8 string -> managed UTF16 string 




##### Method NCube.Helpers.EncodingHelper.StringFromUtf8Ptr(System.IntPtr)

 unmanaged UTF8 bytes (null-terminated) -> managed UTF16 string 




---
# Type NCube.Helpers.WindowLockHelper

 MainWindow 화면 잠금 기능 




---
# Type NCube.Novo.Core.Iris3Header

 @brief IRIS3 PDU 헤더 IRIS3 PDU 헤더로서 20 octets 크기이다. IRIS3 PDU는 EMS와 장비간에 약속된 바이너리 규격으로서 다음과 같은 형태이다. @code IRIS3 PDU 일반 형식 +--------+---------------------+-----------------------+ | header | message 1 payload | message 2 payload | +--------+---------------------+-----------------------+ IRIS3 Request PDU 형식 1 +--------+------------+----------------+--------------+ | header | cmd_header | msg1 (str|bin) | msg2(opt) | +--------+------------+----------------+--------------+ header.msg_type := PTYPE_REQUEST header.msg1_style := PSTYLE_CMD (opt) header.msg2_style := ... IRIS3 Request PDU 형식 2 +--------+----------------------+---------------------+ | header | msg1(str|bin) | msg2(opt) | +--------+----------------------+---------------------+ header.msg_type := PTYPE_REQUEST header.msg1_style := PSTYLE_STRING | PSTYLE_BINARY | PSTYLE_BIN_CRS (opt) header.msg2_style := ... IRIS3 Response Packet Format +--------+---------------------+--------------------------+ | header | message 1 payload | message 2 payload(opt) | +--------+---------------------+--------------------------+ header.msg_type := PTYPE_RESPONSE header.msg1_style := PSTYLE_CALLA | PSTYLE_STRING | PSTYLE_BINARY | .. (opt) header.msg2_style := PSTYLE_BIN_STATUS, PSTYLE_BIN_CRS etc... IRIS3 Event Packet Format +--------+---------------------+--------------------------+ | header | message 1 payload | message 2 payload (opt) | +--------+---------------------+--------------------------+ header.msg_type := PTYPE_EVENT header.msg1_style := PSTYLE_CALLA | PSTYLE_STRING | PSTYLE_BINARY (opt) header.msg2_style := PSTYLE_BIN_STATUS, PSTYLE_BIN_CRS etc... IRIS3 Status Packet Format +--------+-------------------------------------------+ | header | message 1 payload (only binary) | +--------+-------------------------------------------+ header.msg_type := PTYPE_STATUS header.msg1_style := PSTYLE_BINARY header.msg2_style := PSTYPE_NONE header.msg2_length := 0 @endcode 




##### Property NCube.Services.Account.ILoginUserModel.IsLoggedIn

 로그인 성공 여부 




##### Property NCube.Services.Account.ILoginUserModel.UserAPInfo

 User Access Point Info (사용자 액세스 지점 정보) : OS 버전, OS 이름, 컴퓨터 이름 




##### Property NCube.Services.Account.ILoginUserModel.UserIP

 로그인 접속 IP 




##### Property NCube.Services.Account.ILoginUserModel.Account

 로그인 계정 문자열 




##### Property NCube.Services.Account.ILoginUserModel.Password

 로그인 암호 문자열 (Plain Text 형태) 




##### Property NCube.Services.Account.ILoginUserModel.UserID

 로그인 계정의 고유한 내부 ID 




##### Property NCube.Services.Account.ILoginUserModel.Level

 로그인 레벨 문자열 : 'Aministrator', 'Operator', 'Monitor', 'Server' 등의 문자열. Application마다 다를 수 있다. 




##### Property NCube.Services.Account.ILoginUserModel.LevelEnum

 로그인 레벨 숫자값 : 'Server'=0, 'Aministrator'=1, 'Operator'=2, 'Monitor'=3 Application마다 다를 수 있다. 




##### Property NCube.Services.Account.ILoginUserModel.Name

 로그인 운용자 정보 : 이름 




##### Property NCube.Services.Account.ILoginUserModel.Email

 로그인 운용자 정보 : 이메일 주소 




##### Property NCube.Services.Account.ILoginUserModel.Mobile

 로그인 운용자 정보 : 핸드폰 번호 




##### Property NCube.Services.Account.ILoginUserModel.Phone

 로그인 운용자 정보 : 일반 전화 번호 




##### Property NCube.Services.Account.ILoginUserModel.Division

 로그인 운용자 정보 : 소속 부서 




##### Property NCube.Services.Account.ILoginUserModel.Description

 로그인 운용자 정보 : 기타 정보 




---
# Type NCube.Services.Alarms.AlarmBuzzer

 알람 소리를 내주는 클래스 




##### Method NCube.Services.Alarms.AlarmBuzzer.#ctor

 알람 소리를 내주는 클래스 




##### Method NCube.Services.Alarms.AlarmBuzzer.PlayOn(NCube.Services.Alarms.AlarmStatusType)

 알람 소리를 재생합니다. 

|Name | Description |
|-----|------|
|sev: |알람 경보 Type|



##### Method NCube.Services.Alarms.AlarmBuzzer.PlayOn(System.String)

 알람 소리를 재생합니다. 

|Name | Description |
|-----|------|
|filePath: |파일 경로|



---
# Type NCube.Services.ActionResultType

 Action 수행 응답 body 타입 




##### Field NCube.Services.ActionResultType.None

 응답 body가 없을때 




##### Field NCube.Services.ActionResultType.Kai

 응답 body가 kai 객체 




##### Field NCube.Services.ActionResultType.Calla

 응답 body가 calla 객체 




##### Field NCube.Services.ActionResultType.Json

 응답 body가 json 객체 




##### Field NCube.Services.ActionResultType.Datatable

 응답 body가 dataTable 객체 (sqlite용) 




---
# Type NCube.Services.ActionResult

 서비스 action 수행시 리턴 타입 Content는 Type 속성에 따라 달라진다. 




---
# Type NCube.Services.Audit.DefaultAuditMessage

 AUDIT 메시지. 기본은 STD.AUDIT.PUSH 프로시저 호출 




---
# Type NCube.Services.Audit.JsonAuditMessage

 AUDIT 메시지 (JSON 형식). 만약 JSON 형식의 요청이라면 참고바람 




---
# Type NCube.Services.Audit.DefaultAuditServiceAction

 AUDIT 수행 기본 action. STD.AUDIT.PUSH 명령어를 보내고 끝. 




---
# Type NCube.Services.Audit.AuditServiceActionAsync

 AUDIT 수행 기본 action (Async 버전). STD.AUDIT.PUSH 명령어를 보내고, 수행 완료되면 리턴. 




---
# Type NCube.Services.Audit.JsonAuditServiceAction

 AUDIT 수행 JSON action. JSON 형태로 audit push 요청을 보낸다 




---
# Type NCube.Services.Audit.JsonAuditServiceActionAsync

 AUDIT 수행 JSON action (Async 버전). JSON 형태로 audit push 요청을 보내고, 수행 완료되면 리턴. 




---
# Type NCube.Services.Audit.AuditService

 AUDIT 서비스 클래스. 




---
# Type NCube.Services.Threading.TimedLock

 Class provides a nice way of obtaining a lock that will time out with a cleaner syntax than using the whole Monitor.TryEnter() method. 



> Adapted from Ian Griffiths article http://www.interact-sw.co.uk/iangblog/2004/03/23/locking and incorporating suggestions by Marek Malowidzki as outlined in this blog post http://www.interact-sw.co.uk/iangblog/2004/05/12/timedlockstacktrace 

##### Example:  Instead of: 

######  code

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






##### Method NCube.Services.Threading.TimedLock.Lock(System.Object)

 Attempts to obtain a lock on the specified object for up to 10 seconds. 

|Name | Description |
|-----|------|
|o: ||
**Returns**: 




##### Method NCube.Services.Threading.TimedLock.Lock(System.Object,System.TimeSpan)

 Attempts to obtain a lock on the specified object for up to the specified timeout. 

|Name | Description |
|-----|------|
|o: ||
|timeout: ||
**Returns**: 




##### Method NCube.Services.Threading.TimedLock.Dispose

 Disposes of this lock. 




---
# Type NCube.Services.Threading.LockTimeoutException

 Thrown when a lock times out. 




##### Method NCube.Services.Threading.LockTimeoutException.ReportStackTraceIfError(System.Object)

 Sets the stack trace for the given lock target if an error occurred. 

|Name | Description |
|-----|------|
|lockTarget: |Lock target.|



##### Method NCube.Services.Threading.LockTimeoutException.#ctor(System.Object)

 Creates a new [[|T:NCube.Services.Threading.LockTimeoutException]] instance. 



>Use this exception.

|Name | Description |
|-----|------|
|lockTarget: |Object we tried to lock.|



##### Method NCube.Services.Threading.LockTimeoutException.GetBlockingStackTrace(System.Int32)

 Stack trace of the thread that holds a lock on the object this lock is attempting to acquire when it fails. 

|Name | Description |
|-----|------|
|timeout: |Number of milliseconds to wait for the blocking stack trace.|



##### Method NCube.Services.Threading.LockTimeoutException.#ctor

 Creates a new [[|T:NCube.Services.Threading.LockTimeoutException]] instance. 




##### Method NCube.Services.Threading.LockTimeoutException.#ctor(System.String)

 Constructor. 

|Name | Description |
|-----|------|
|message: ||



##### Method NCube.Services.Threading.LockTimeoutException.#ctor(System.String,System.Exception)

 Constructor. 

|Name | Description |
|-----|------|
|message: ||
|innerException: ||



##### Method NCube.Services.Threading.LockTimeoutException.#ctor(System.Runtime.Serialization.SerializationInfo,System.Runtime.Serialization.StreamingContext)

 Constructor. 

|Name | Description |
|-----|------|
|info: ||
|context: ||



##### Method NCube.Services.Threading.LockTimeoutException.ToString

 Returns a string representation of the exception. 

**Returns**: 




---
# Type NCube.Services.Threading.UndisposedLockException

 This exception indicates that a user of the TimedLock struct failed to leave a Monitor. This could be the result of a deadlock or forgetting to use the using statement or a try finally block. 




##### Method NCube.Services.Threading.UndisposedLockException.#ctor(System.String)

 Constructor. 

|Name | Description |
|-----|------|
|message: ||



##### Method NCube.Services.Threading.UndisposedLockException.#ctor(System.Runtime.Serialization.SerializationInfo,System.Runtime.Serialization.StreamingContext)

 Special constructor used for deserialization. 

|Name | Description |
|-----|------|
|info: ||
|context: ||



---
# Type NCube.Services.Threading.OneShotTimerHelper

 밀리초 대기 후, Action을 수행하게 해주는 타이머 헬퍼. @example public void Test() { // 생성자 직접 호출 방식 new OneShotTimer(()=>{ }, 10); // 헬퍼 클래스 사용하는 방식 OneShotTimerHelper.Start(()=>{ }, 1000); // 헬퍼 클래스 사용하는 방식 (Stop이 필요한 경우) var timer = OneShotTimerHelper.Start(()=>{ }, 1000); timer.Stop(); } @Author : Uk @Date : 2016-07-21 


##### Method NCube.Services.MetaFacade.MetaManager.TranRequestAsync(System.String,System.Byte[],System.Int32,System.Int32)

 metaTran 채널로 IRIS PDU 요청을 보낸다. ASYNC 버전 

|Name | Description |
|-----|------|
|addr_str: |문자열 형태의 meta address|
|req_pdu: |IRIS PDU|
|ctag: ||
|timeout: |타임아웃 기본 30초|
**Returns**:  Task<Tuple<bool, JArray, int>> Item1 : 수행 완료 여부, 성공이든 실패든 응답이 오면 true, 응답 자체가 안오고 타임아웃되면 false Item2 : 응답 데이터 테이블 Item3 : result code 값. 명령수행 성공시 0, 실패시 에러 코드를 의미한다 




##### Method NCube.Services.MetaFacade.MetaManager.TranRequestTL1Async(System.String,System.String,System.Int32,System.Int32)

 metaTran 채널로 TL1요청을 보낸다. ASYNC 버전 

|Name | Description |
|-----|------|
|addr_str: |문자열 형태의 meta address|
|req_pdu: |TL1 명령어 문자열|
|ctag: ||
|timeout: |타임아웃 기본 30초|
**Returns**:  Item1 : 수행 완료 여부, 성공이든 실패든 응답이 오면 true, 응답 자체가 안오고 타임아웃되면 false Item2 : 응답 데이터 테이블 Item3 : result code 값. 명령수행 성공시 0, 실패시 에러 코드를 의미한다 




---
# Type NCube.Services.Report.HohCellModel

 DataTable의 Cell을 담는 데이터 클래스입니다. 




##### Field NCube.Services.Report.HohCellModel.CommonFont

 CellModel에 기본으로 지정된 폰트입니다. 글꼴 : "Segoe UI" 크기 : 10 




##### Property NCube.Services.Report.HohCellModel.Value

 Cell에 저장된 값 




##### Property NCube.Services.Report.HohCellModel.Font

 Cell의 폰트 




---
# Type NCube.Services.Report.HohColumn

 Model을 DataTable로 변경하기 위한 클래스 




##### Property NCube.Services.Report.HohColumn.Header

 Column의 헤더 이름 




##### Property NCube.Services.Report.HohColumn.FieldName

 입력하고자하는 Property 이름 




##### Property NCube.Services.Report.HohColumn.WidthRatio

 기본 값은 1입니다. 프린트에만 적용이 됩니다. 




---
# Type NCube.Services.Report.HohDataColumn

 DataTable의 DataColumn에 넓이 비율을 만들어주기 위한 클래스 




##### Property NCube.Services.Report.HohDataColumn.WidthRatio

 프린트에 쓰일 넓이 비율 




##### Property NCube.Services.Report.HohDataColumn.Font

 Cell의 폰트 




---
# Type NCube.Services.Report.HohReportPrinter

 프린트를 만들기 위한 클래스 




##### Event NCube.Services.Report.HohReportPrinter.Progress

 HohSheet 처리시 처리 상태를 표현합니다. 주의 : Thread에 Unsafe 합니다. 




##### Method NCube.Services.Report.HohReportPrinter.Clear

 초기화합니다. 




##### Method NCube.Services.Report.HohReportPrinter.Add(NCube.Services.Report.HohSheetModel)

 프린트할 데이터를 추가합니다. Add한 순서대로 출력됩니다. 

|Name | Description |
|-----|------|
|HohSheetModel: |출력할 HohSheetModel|



##### Method NCube.Services.Report.HohReportPrinter.ShowPreviewDialog

 PreviewDialog를 보여줍니다. 




##### Method NCube.Services.Report.HohReportPrinter.CreateDocumentAsync(System.Threading.CancellationToken)

 문서를 비동기로 생성합니다. 

|Name | Description |
|-----|------|
|token: |취소 토큰|
**Returns**: 비동기 Task




---
# Type NCube.Services.Report.HohReportTemplate

 프린트를 출력하기 위한 템플릿 




##### Property NCube.Services.Report.HohReportTemplate.TitleMargin

 타이틀과 Content 사이 여백 




##### Method NCube.Services.Report.HohReportTemplate.#ctor(NCube.Services.Report.HohSheetProgress)

 Progress를 사용이 HohReportPrinter와 밀접하므로 충돌 방지를 위해 internal로 관리함 

|Name | Description |
|-----|------|
|progress: ||



##### Method NCube.Services.Report.HohReportTemplate.InsertData(NCube.Services.Report.HohSheetModel,System.Threading.CancellationToken)

 문서 내부에 표현할 데이터 값을 넣습니다. Task 취소시, OperationCanceledException 예외가 발생합니다. 

|Name | Description |
|-----|------|
|HohSheetModel: |입력할 데이터|
|token: |취소 토큰|



##### Method NCube.Services.Report.HohReportTemplate.TestView

 테스트를 위한 뷰입니다. 




##### Field NCube.Services.Report.HohReportTemplate.components

 Required designer variable. 




##### Method NCube.Services.Report.HohReportTemplate.Dispose(System.Boolean)

 Clean up any resources being used. 

|Name | Description |
|-----|------|
|disposing: |true if managed resources should be disposed; otherwise, false.|



##### Method NCube.Services.Report.HohReportTemplate.InitializeComponent

 Required method for Designer support - do not modify the contents of this method with the code editor. 




---
# Type NCube.Services.Report.HohSheetControl

 UI의 Control을 캡쳐하는 클래스입니다. 




##### Method NCube.Services.Report.HohSheetControl.#ctor(System.Windows.FrameworkElement)

 캡쳐하기 위한 컨트롤을 넣습니다. 

|Name | Description |
|-----|------|
|control: |캡처할 Control 클래스|



##### Method NCube.Services.Report.HohSheetControl.FindChild``1(System.Windows.DependencyObject,System.String)

 Finds a Child of a given item in the visual tree. 참고 소스코드 : http://stackoverflow.com/questions/636383/how-can-i-find-wpf-controls-by-name-or-type 

|Name | Description |
|-----|------|
|parent: |A direct parent of the queried item.|
|T: |The type of the queried item.|
|Name | Description |
|-----|------|
|childName: |x:Name or Name of child. |
**Returns**: The first parent item that matches the submitted type parameter. If not matching item can be found, a null parent is being returned.




---
# Type NCube.Services.Report.HohSheetModel

 표로 넣기 위한 데이터 




##### Field NCube.Services.Report.HohSheetModel.CommonTitleFont

 HohSheetData에 기본으로 지정된 폰트입니다. 글꼴 : "Segoe UI" 크기 : 12 스타일 : Bold 




##### Field NCube.Services.Report.HohSheetModel.CommonHeaderCommentFont

 HohSheetData에 기본으로 지정된 폰트입니다. 글꼴 : "Segoe UI" 크기 : 10 




##### Property NCube.Services.Report.HohSheetProgress.RowsCycle

 성능을 위해, 특정 Row갯수일 때만 Progressing 이밴트를 호출하기 위해 사용함 




##### Event NCube.Services.Report.HohSheetProgress.Progressing

 HohSheet 처리시 처리 상태를 표현합니다. 주의 : Thread에 Unsafe 합니다. 




##### Method NCube.Services.Report.HohSheetProgress.#ctor(System.Int32)

 진행률을 표시하기 위한 클래스 

|Name | Description |
|-----|------|
|rowsCycle: |진행시, 세알릴 row 개수|



---
# Type NCube.Services.Report.HohSheetProgressArgs

 Sheet 처리에 대한 이밴트값들 




##### Property NCube.Services.Report.HohSheetProgressArgs.CurrentRows

 처리된 현재 Rows 값 




##### Property NCube.Services.Report.HohSheetProgressArgs.CurrentImages

 처리된 현재 Images 값 




---
# Type NCube.Services.Report.HohSheetTable

 List를 Table로 변경하는 클래스 




##### Field NCube.Services.Report.HohSheetTable.TableTypes.GridControl

 일반적인 테이블 형태 




##### Field NCube.Services.Report.HohSheetTable.TableTypes.TreeKey

 Tree로 표현된 경우, Tree를 각각의 컬럼으로 표시 




##### Field NCube.Services.Report.HohSheetTable.TableTypes.TreeKeyCombineView

 Tree로 표현된 경우, Tree를 하나의 컬럼으로 표시 




##### Method NCube.Services.Report.HohSheetTable.#ctor(System.Collections.IEnumerable,NCube.Services.Report.HohSheetTable.TableTypes,System.String,System.String,System.String,System.String)

 List를 Table로 변경시켜주는 클래스 

|Name | Description |
|-----|------|
|itemsSource: |출력할 List|
|tableType: |출력할 타입|
|keyField: |Key의 Property 이름|
|parentKeyField: |ParentKey의 Property 이름|
|treeField: |Tree일 경우, Tree 구조를 결정하는 Key Property이름|
|treeHeader: |Tree Key를 표에 출력할 이름|



##### Method NCube.Services.Report.HohSheetTable.BuildDataTableAsync

 Table 데이터로 변환합니다. 

**Returns**: 변환된 DataTable




##### Method NCube.Services.Report.HohSheetTable.BuildDataTableAsync(System.Threading.CancellationToken)

 Table 데이터로 변환합니다. 

|Name | Description |
|-----|------|
|token: |취소|
**Returns**: 변환된 DataTable




---
# Type NCube.Services.Report.HohSpreadSheet

 데이터 타입을 엑셀로 변환시켜주는 클래스 내부적으로 사용하는 클래스가 UI 쓰레드를 필요하므로, 반드시 코드 생성시에 UI 쓰레드 내에서 생성해야 합니다. 




##### Event NCube.Services.Report.HohSpreadSheet.Progress

 HohSheet 처리시 처리 상태를 표현합니다. 주의 : Thread에 Unsafe 합니다. 




##### Method NCube.Services.Report.HohSpreadSheet.#ctor

 데이터 타입을 엑셀로 변환시켜주는 클래스 




##### Method NCube.Services.Report.HohSpreadSheet.Add(NCube.Services.Report.HohSheetModel)

 SpreadSheet에 HohSheetData를 추가합니다. 생성하려면 반드시 CreateSheet 혹은 CreateSheetAsync를 동작시켜야 합니다. 

|Name | Description |
|-----|------|
|HohSheetModel: |추가하고자 하는 Sheet|



##### Method NCube.Services.Report.HohSpreadSheet.CreateSheet(System.Threading.CancellationToken)

 Sheet를 생성합니다. 




##### Method NCube.Services.Report.HohSpreadSheet.CreateSheetAsync

 Sheet를 비동기로 생성합니다. 

**Returns**: 




##### Method NCube.Services.Report.HohSpreadSheet.CreateSheetAsync(System.Threading.CancellationToken)

 Sheet를 비동기로 생성합니다. 

|Name | Description |
|-----|------|
|token: |취소 토큰|
**Returns**: 




##### Method NCube.Assets.Images.StaticImage.MessageBoxImageToBitmapImage(System.Windows.MessageBoxImage)

 Dialog에 사용될 아이콘의 BitmapImage를 리턴합니다. 

|Name | Description |
|-----|------|
|boxImage: |DIalog에 적용된 MessageBoxImage 값|
**Returns**: 아이콘




---
# Type NCube.Properties.Resources

 A strongly-typed resource class, for looking up localized strings, etc. 




##### Property NCube.Properties.Resources.ResourceManager

 Returns the cached ResourceManager instance used by this class. 




##### Property NCube.Properties.Resources.Culture

 Overrides the current thread's CurrentUICulture property for all resource lookups using this strongly typed resource class. 




---
# Type XamlGeneratedNamespace.GeneratedInternalTypeHelper

 GeneratedInternalTypeHelper 




##### Method XamlGeneratedNamespace.GeneratedInternalTypeHelper.CreateInstance(System.Type,System.Globalization.CultureInfo)

 CreateInstance 




##### Method XamlGeneratedNamespace.GeneratedInternalTypeHelper.GetPropertyValue(System.Reflection.PropertyInfo,System.Object,System.Globalization.CultureInfo)

 GetPropertyValue 




##### Method XamlGeneratedNamespace.GeneratedInternalTypeHelper.SetPropertyValue(System.Reflection.PropertyInfo,System.Object,System.Object,System.Globalization.CultureInfo)

 SetPropertyValue 




##### Method XamlGeneratedNamespace.GeneratedInternalTypeHelper.CreateDelegate(System.Type,System.Object,System.String)

 CreateDelegate 




##### Method XamlGeneratedNamespace.GeneratedInternalTypeHelper.AddEventHandler(System.Reflection.EventInfo,System.Object,System.Delegate)

 AddEventHandler 






