# <a name="enrollmenttroubleshootingevent-resource-type"></a>enrollmentTroubleshootingEvent リソースの種類

> **注:**Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。

登録エラーを表すイベント。

[deviceManagementTroubleshootingEvent](../resources/intune_troubleshooting_devicemanagementtroubleshootingevent.md) からの継承

## <a name="methods"></a>メソッド
|メソッド|戻り値の型|説明|
|:---|:---|:---|
|[List enrollmentTroubleshootingEvents](../api/intune_troubleshooting_enrollmenttroubleshootingevent_list.md)|[enrollmentTroubleshootingEvent](../resources/intune_troubleshooting_enrollmenttroubleshootingevent.md) コレクション|[enrollmentTroubleshootingEvent](../resources/intune_troubleshooting_enrollmenttroubleshootingevent.md) オブジェクトのプロパティとリレーションシップをリストします。|
|[Get enrollmentTroubleshootingEvent](../api/intune_troubleshooting_enrollmenttroubleshootingevent_get.md)|[enrollmentTroubleshootingEvent](../resources/intune_troubleshooting_enrollmenttroubleshootingevent.md)|[enrollmentTroubleshootingEvent](../resources/intune_troubleshooting_enrollmenttroubleshootingevent.md) オブジェクトのプロパティとリレーションシップを読み取ります。|
|[Create enrollmentTroubleshootingEvent](../api/intune_troubleshooting_enrollmenttroubleshootingevent_create.md)|[enrollmentTroubleshootingEvent](../resources/intune_troubleshooting_enrollmenttroubleshootingevent.md)|新しい [enrollmentTroubleshootingEvent](../resources/intune_troubleshooting_enrollmenttroubleshootingevent.md) オブジェクトを作成します。|
|[Delete enrollmentTroubleshootingEvent](../api/intune_troubleshooting_enrollmenttroubleshootingevent_delete.md)|なし|[enrollmentTroubleshootingEvent](../resources/intune_troubleshooting_enrollmenttroubleshootingevent.md) を削除します。|
|[Update enrollmentTroubleshootingEvent](../api/intune_troubleshooting_enrollmenttroubleshootingevent_update.md)|[enrollmentTroubleshootingEvent](../resources/intune_troubleshooting_enrollmenttroubleshootingevent.md)|[enrollmentTroubleshootingEvent](../resources/intune_troubleshooting_enrollmenttroubleshootingevent.md) オブジェクトのプロパティを更新します。|

## <a name="properties"></a>プロパティ
|プロパティ|型|説明|
|:---|:---|:---|
|id|文字列型 (String)|オブジェクトの UUID。[deviceManagementTroubleshootingEvent](../resources/intune_troubleshooting_devicemanagementtroubleshootingevent.md) から継承|
|eventDateTime|DateTimeOffset|インシデントが発生した時間。 [deviceManagementTroubleshootingEvent](../resources/intune_troubleshooting_devicemanagementtroubleshootingevent.md) からの継承|
|correlationId|文字列型 (String)|サービスのエラーをトレースするための ID。 [deviceManagementTroubleshootingEvent](../resources/intune_troubleshooting_devicemanagementtroubleshootingevent.md) からの継承|
|managedDeviceIdentifier|文字列型 (String)|Intune によって作成または収集されるデバイス識別子。|
|operatingSystem|文字列型 (String)|オペレーティング システム。|
|osVersion|文字列型 (String)|OS バージョン。|
|userId|文字列型 (String)|デバイスを登録しようとするユーザーの識別子。|
|deviceId|文字列型 (String)|Azure AD デバイス識別子。|
|enrollmentType|文字列型 (String)|登録の種類。 可能な値: `unknown`、`userEnrollment`、`deviceEnrollmentManager`、`appleBulkWithUser`、`appleBulkWithoutUser`、`windowsAzureADJoin`、`windowsBulkUserless`、`windowsAutoEnrollment`、`windowsBulkAzureDomainJoin`、`windowsCoManagement`。|
|failureCategory|文字列型 (String)|高レベルのエラー カテゴリ。 可能な値: `unknown`、`authentication`、`authorization`、`accountValidation`、`userValidation`、`deviceNotSupported`、`inMaintenance`、`badRequest`、`featureNotSupported`、`enrollmentRestrictionsEnforced`、`clientDisconnected`。|
|failureReason|文字列型 (String)|詳細なエラーの理由:|

## <a name="relationships"></a>リレーションシップ
なし
## <a name="json-representation"></a>JSON 表記
以下は、リソースの JSON 表記です。
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.enrollmentTroubleshootingEvent"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.enrollmentTroubleshootingEvent",
  "id": "String (identifier)",
  "eventDateTime": "String (timestamp)",
  "correlationId": "String",
  "managedDeviceIdentifier": "String",
  "operatingSystem": "String",
  "osVersion": "String",
  "userId": "String",
  "deviceId": "String",
  "enrollmentType": "String",
  "failureCategory": "String",
  "failureReason": "String"
}
```



