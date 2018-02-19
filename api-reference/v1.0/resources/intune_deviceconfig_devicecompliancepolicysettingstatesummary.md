# <a name="devicecompliancepolicysettingstatesummary-resource-type"></a>deviceCompliancePolicySettingStateSummary リソースの種類

> **注:**Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。

アカウント全体における、デバイス コンプライアンスのポリシー設定状態の要約です。
## <a name="methods"></a>メソッド
|メソッド|戻り値の型|説明|
|:---|:---|:---|
|[deviceCompliancePolicySettingStateSummaries のリスト](../api/intune_deviceconfig_devicecompliancepolicysettingstatesummary_list.md)|[deviceCompliancePolicySettingStateSummary](../resources/intune_deviceconfig_devicecompliancepolicysettingstatesummary.md) コレクション|[deviceCompliancePolicySettingStateSummary](../resources/intune_deviceconfig_devicecompliancepolicysettingstatesummary.md) オブジェクトのプロパティとリレーションシップをリストします。|
|[deviceCompliancePolicySettingStateSummary の取得](../api/intune_deviceconfig_devicecompliancepolicysettingstatesummary_get.md)|[deviceCompliancePolicySettingStateSummary](../resources/intune_deviceconfig_devicecompliancepolicysettingstatesummary.md)|[deviceCompliancePolicySettingStateSummary](../resources/intune_deviceconfig_devicecompliancepolicysettingstatesummary.md) オブジェクトのプロパティとリレーションシップを読み取ります。|
|[deviceCompliancePolicySettingStateSummary の作成](../api/intune_deviceconfig_devicecompliancepolicysettingstatesummary_create.md)|[deviceCompliancePolicySettingStateSummary](../resources/intune_deviceconfig_devicecompliancepolicysettingstatesummary.md)|新しい [deviceCompliancePolicySettingStateSummary](../resources/intune_deviceconfig_devicecompliancepolicysettingstatesummary.md) オブジェクトを作成します。|
|[deviceCompliancePolicySettingStateSummary の削除](../api/intune_deviceconfig_devicecompliancepolicysettingstatesummary_delete.md)|なし|[deviceCompliancePolicySettingStateSummary](../resources/intune_deviceconfig_devicecompliancepolicysettingstatesummary.md) を削除します。|
|[deviceCompliancePolicySettingStateSummary の更新](../api/intune_deviceconfig_devicecompliancepolicysettingstatesummary_update.md)|[deviceCompliancePolicySettingStateSummary](../resources/intune_deviceconfig_devicecompliancepolicysettingstatesummary.md)|[deviceCompliancePolicySettingStateSummary](../resources/intune_deviceconfig_devicecompliancepolicysettingstatesummary.md) オブジェクトのプロパティを更新します。|

## <a name="properties"></a>プロパティ
|プロパティ|型|説明|
|:---|:---|:---|
|setting|String|設定のクラス名とプロパティ名です。|
|settingName|String|設定の名前です。|
|platformType|String|設定のプラットフォームです。可能な値は、`android`、`iOS`、`macOS`、`windowsPhone81`、`windows81AndLater`、`windows10AndLater`、`all` です。|
|id|String|エンティティのキー。|
|unknownDeviceCount|Int32|不明なデバイスの数|
|notApplicableDeviceCount|Int32|該当しないデバイスの数|
|compliantDeviceCount|Int32|準拠デバイスの数|
|remediatedDeviceCount|Int32|修復済みデバイスの数|
|nonCompliantDeviceCount|Int32|準拠していないデバイスの数|
|errorDeviceCount|Int32|エラー デバイスの数|
|conflictDeviceCount|Int32|競合デバイスの数|

## <a name="relationships"></a>リレーションシップ
|リレーションシップ|型|説明|
|:---|:---|:---|
|deviceComplianceSettingStates|[deviceComplianceSettingState](../resources/intune_deviceconfig_devicecompliancesettingstate.md) コレクション|まだ文書化されていません|

## <a name="json-representation"></a>JSON 表記
以下は、リソースの JSON 表記です。
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.deviceCompliancePolicySettingStateSummary"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceCompliancePolicySettingStateSummary",
  "setting": "String",
  "settingName": "String",
  "platformType": "String",
  "id": "String (identifier)",
  "unknownDeviceCount": 1024,
  "notApplicableDeviceCount": 1024,
  "compliantDeviceCount": 1024,
  "remediatedDeviceCount": 1024,
  "nonCompliantDeviceCount": 1024,
  "errorDeviceCount": 1024,
  "conflictDeviceCount": 1024
}
```



