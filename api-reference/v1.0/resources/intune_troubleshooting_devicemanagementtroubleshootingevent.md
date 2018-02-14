# <a name="devicemanagementtroubleshootingevent-resource-type"></a>deviceManagementTroubleshootingEvent リソースの種類

> **注:**Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。

一般エラーを表すイベント。
## <a name="methods"></a>メソッド
|メソッド|戻り値の型|説明|
|:---|:---|:---|
|[List deviceManagementTroubleshootingEvents](../api/intune_troubleshooting_devicemanagementtroubleshootingevent_list.md)|[deviceManagementTroubleshootingEvent](../resources/intune_troubleshooting_devicemanagementtroubleshootingevent.md) コレクション|[deviceManagementTroubleshootingEvent](../resources/intune_troubleshooting_devicemanagementtroubleshootingevent.md) オブジェクトのプロパティとリレーションシップをリストします。|
|[Get deviceManagementTroubleshootingEvent](../api/intune_troubleshooting_devicemanagementtroubleshootingevent_get.md)|[deviceManagementTroubleshootingEvent](../resources/intune_troubleshooting_devicemanagementtroubleshootingevent.md)|[deviceManagementTroubleshootingEvent](../resources/intune_troubleshooting_devicemanagementtroubleshootingevent.md) オブジェクトのプロパティとリレーションシップを読み取ります。|
|[Create deviceManagementTroubleshootingEvent](../api/intune_troubleshooting_devicemanagementtroubleshootingevent_create.md)|[deviceManagementTroubleshootingEvent](../resources/intune_troubleshooting_devicemanagementtroubleshootingevent.md)|新しい [deviceManagementTroubleshootingEvent](../resources/intune_troubleshooting_devicemanagementtroubleshootingevent.md) オブジェクトを作成します。|
|[Delete deviceManagementTroubleshootingEvent](../api/intune_troubleshooting_devicemanagementtroubleshootingevent_delete.md)|なし|[deviceManagementTroubleshootingEvent](../resources/intune_troubleshooting_devicemanagementtroubleshootingevent.md) を削除します。|
|[Update deviceManagementTroubleshootingEvent](../api/intune_troubleshooting_devicemanagementtroubleshootingevent_update.md)|[deviceManagementTroubleshootingEvent](../resources/intune_troubleshooting_devicemanagementtroubleshootingevent.md)|[deviceManagementTroubleshootingEvent](../resources/intune_troubleshooting_devicemanagementtroubleshootingevent.md) オブジェクトのプロパティを更新します。|

## <a name="properties"></a>プロパティ
|プロパティ|型|説明|
|:---|:---|:---|
|id|文字列型 (String)|オブジェクトの UUID|
|eventDateTime|DateTimeOffset|インシデントが発生した時間。|
|correlationId|文字列型 (String)|サービスのエラーをトレースするための ID。|

## <a name="relationships"></a>リレーションシップ
なし
## <a name="json-representation"></a>JSON 表記
以下は、リソースの JSON 表記です。
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.deviceManagementTroubleshootingEvent"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceManagementTroubleshootingEvent",
  "id": "String (identifier)",
  "eventDateTime": "String (timestamp)",
  "correlationId": "String"
}
```



