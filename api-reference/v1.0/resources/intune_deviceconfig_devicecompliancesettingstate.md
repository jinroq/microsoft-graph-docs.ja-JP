# <a name="devicecompliancesettingstate-resource-type"></a>deviceComplianceSettingState リソース タイプ

> **注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。

特定のデバイスに関する、デバイスのコンプライアンスの設定状態です。
## <a name="methods"></a>メソッド
|メソッド|戻り値の型|説明|
|:---|:---|:---|
|[deviceComplianceSettingStates のリスト](../api/intune_deviceconfig_devicecompliancesettingstate_list.md)|[deviceComplianceSettingState](../resources/intune_deviceconfig_devicecompliancesettingstate.md) コレクション|[deviceComplianceSettingState](../resources/intune_deviceconfig_devicecompliancesettingstate.md) オブジェクトのプロパティとリレーションシップをリストします。|
|[deviceComplianceSettingState の取得](../api/intune_deviceconfig_devicecompliancesettingstate_get.md)|[deviceComplianceSettingState](../resources/intune_deviceconfig_devicecompliancesettingstate.md)|[deviceComplianceSettingState](../resources/intune_deviceconfig_devicecompliancesettingstate.md) オブジェクトのプロパティとリレーションシップを読み取ります。|
|[deviceComplianceSettingState の作成](../api/intune_deviceconfig_devicecompliancesettingstate_create.md)|[deviceComplianceSettingState](../resources/intune_deviceconfig_devicecompliancesettingstate.md)|新しい [deviceComplianceSettingState](../resources/intune_deviceconfig_devicecompliancesettingstate.md) オブジェクトを作成します。|
|[deviceComplianceSettingState の削除](../api/intune_deviceconfig_devicecompliancesettingstate_delete.md)|なし|[deviceComplianceSettingState](../resources/intune_deviceconfig_devicecompliancesettingstate.md) を削除します。|
|[deviceComplianceSettingState の更新](../api/intune_deviceconfig_devicecompliancesettingstate_update.md)|[deviceComplianceSettingState](../resources/intune_deviceconfig_devicecompliancesettingstate.md)|[deviceComplianceSettingState](../resources/intune_deviceconfig_devicecompliancesettingstate.md) オブジェクトのプロパティを更新します。|

## <a name="properties"></a>プロパティ
|プロパティ|タイプ|説明|
|:---|:---|:---|
|ID|文字列|エンティティのキー|
|setting|文字列|設定のクラス名とプロパティ名。|
|settingName|文字列|レポートされている設定名。|
|deviceId|文字列|レポートされているデバイス ID。|
|deviceName|文字列|レポートされているデバイス名。|
|userId|文字列|レポートされているユーザー ID|
|userEmail|文字列|レポートされているユーザーのメール アドレス。|
|userName|文字列|レポートされているユーザー名|
|userPrincipalName|文字列|レポートされているユーザーの PrincipalName|
|deviceModel|文字列|レポートされているデバイス モデル|
|状態|[complianceStatus](../resources/intune_shared_compliancestatus.md)|設定のコンプライアンスの状態です。 可能な値は、`unknown`、`notApplicable`、`compliant`、`remediated`、`nonCompliant`、`error`、`conflict` です。|
|complianceGracePeriodExpirationDateTime|DateTimeOffset|デバイス コンプライアンスの猶予期間が過ぎる DateTime|

## <a name="relationships"></a>リレーションシップ
なし
## <a name="json-representation"></a>JSON 表記
以下は、リソースの JSON 表記です。
<!--{
  "blockType": "resource",
  "keyProperty": "id",
  "baseType": "microsoft.graph.entity",
  "@odata.type": "microsoft.graph.deviceComplianceSettingState"
}-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceComplianceSettingState",
  "id": "String (identifier)",
  "setting": "String",
  "settingName": "String",
  "deviceId": "String",
  "deviceName": "String",
  "userId": "String",
  "userEmail": "String",
  "userName": "String",
  "userPrincipalName": "String",
  "deviceModel": "String",
  "state": "String",
  "complianceGracePeriodExpirationDateTime": "String (timestamp)"
}
```



