# <a name="resetpasscodeactionresult-resource-type"></a>resetPasscodeActionResult リソースの種類

> **注:**Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。

パスコードのリセット アクションの結果

[deviceActionResult](../resources/intune_devices_deviceactionresult.md) からの継承

## <a name="properties"></a>プロパティ
|プロパティ|型|説明|
|:---|:---|:---|
|actionName|文字列型 (String)|[deviceActionResult](../resources/intune_devices_deviceactionresult.md) から継承されるアクション名|
|actionState|文字列型 (String)|[deviceActionResult](../resources/intune_devices_deviceactionresult.md) から継承されるアクションの状態。可能な値: `none`、`pending`、`canceled`、`active`、`done`、`failed`、`notSupported`。|
|startDateTime|DateTimeOffset|アクションが開始された時刻。[deviceActionResult](../resources/intune_devices_deviceactionresult.md) から継承。|
|lastUpdatedDateTime|DateTimeOffset|アクション状態の最終更新時刻。[deviceActionResult](../resources/intune_devices_deviceactionresult.md) から継承|
|passcode|文字列型 (String)|デバイス用に新たに生成されたパスコード |

## <a name="relationships"></a>リレーションシップ
なし
## <a name="json-representation"></a>JSON 表記
以下は、リソースの JSON 表記です。
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.resetPasscodeActionResult"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.resetPasscodeActionResult",
  "actionName": "String",
  "actionState": "String",
  "startDateTime": "String (timestamp)",
  "lastUpdatedDateTime": "String (timestamp)",
  "passcode": "String"
}
```



