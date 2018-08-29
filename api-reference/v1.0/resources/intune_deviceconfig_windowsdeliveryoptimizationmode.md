# <a name="windowsdeliveryoptimizationmode-enum-type"></a>windowsDeliveryOptimizationMode 列挙型

> **注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。

ピア配布の配信最適化モード
## <a name="members"></a>メンバー
|メンバー|値|説明|
|:---|:---|:---|
|userDefined|0|設定するユーザーを許可します。|
|httpOnly|1|HTTPのみ、ピアリングなし|
|httpWithPeeringNat|2|OS の既定値 – 同じネットワーク アドレス変換器の背後にあるピアリングとブレンドされた http|
|httpWithPeeringPrivateGroup|3|プライベート グループ全体でピアリングとブレンドされた http|
|httpWithInternetPeering|4|インターネットのピアリングとブレンドされた http|
|simpleDownload|99|ピアリングのない単純なダウンロード モード|
|bypassMode|100|バイパス モードにします。 配信の最適化を使用せず、代わりに BITS を使用|



