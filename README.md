# VirtualDesktop.VRCFaceTracking
VRCFaceTracking module for Virtual Desktop


## パラメータースケーリング
- パラメータースケーリングの設定ファイル（`%AppData%\Virtual Desktop\ftParams.json`）で各パラメーターのスケーリングを設定できます
- ファイルが存在しない場合はこのレポジトリから`ftParams.json`をコピーして`%AppData%\Virtual Desktop\ftParams.json`に置いてください（パラメータースケーリング使わない場合は必要ありません）
- このファイルは浮動小数点数のJSON配列として構成され、各値は対応する表情パラメータのスケール係数を表します
- ファイルにある係数の順番は`Expressions.cs`にある`Expressions`列挙型の定義順に対応しています（BrowLowererLが0番、BrowLowererRが1番...というように）
- 編集する際は必ず`Expressions.cs`を参照してください