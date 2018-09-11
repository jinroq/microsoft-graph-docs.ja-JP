# <a name="defendercloudblockleveltype-enum-type"></a>defenderCloudBlockLevelType 列挙型

> **注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。

クラウド ブロック レベルの使用可能な値
## <a name="members"></a>メンバー
|メンバー|値|説明|
|:---|:---|:---|
|notConfigured|0|既定値、規定の Windows Defender アンチウイルス ソフトウェアのブロック レベルを使用、正規ファイルを検出するリスクを増大させることなく強力な検出性能を提供|
|high|1|"高" は強力な検出レベルを適用します。|
|highPlus|2|"高 +" は、高レベルを使用し、追加の保護手段を適用します。|
|zeroTolerance|3|"ゼロ容認" は、すべての不明な実行ファイルをブロックします。|








