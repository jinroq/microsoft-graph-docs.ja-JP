# <a name="devicemanagement-resource-type"></a>deviceManagement リソースの種類

> **注:**Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。

すべてのデバイス管理機能のコンテナーとして機能する単一のエンティティです。
## <a name="methods"></a>メソッド
|メソッド|戻り値の型|説明|
|:---|:---|:---|
|[deviceManagement の取得](../api/intune_deviceconfig_devicemanagement_get.md)|[deviceManagement](../resources/intune_deviceconfig_devicemanagement.md)|[deviceManagement](../resources/intune_deviceconfig_devicemanagement.md) オブジェクトのプロパティとリレーションシップを読み取ります。|
|[deviceManagement の更新](../api/intune_deviceconfig_devicemanagement_update.md)|[deviceManagement](../resources/intune_deviceconfig_devicemanagement.md)|[deviceManagement](../resources/intune_deviceconfig_devicemanagement.md) オブジェクトのプロパティを更新します。|

## <a name="properties"></a>プロパティ
|プロパティ|型|説明|
|:---|:---|:---|
|id|String|一意識別子|
|settings|[deviceManagementSettings](../resources/intune_deviceconfig_devicemanagementsettings.md)|アカウント レベルの設定です。|

## <a name="relationships"></a>リレーションシップ
|リレーションシップ|型|説明|
|:---|:---|:---|
|deviceConfigurations|[deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md) コレクション|デバイス構成です。|
|deviceCompliancePolicies|[deviceCompliancePolicy](../resources/intune_deviceconfig_devicecompliancepolicy.md) コレクション|デバイス コンプライアンス ポリシーです。|
|softwareUpdateStatusSummary|[softwareUpdateStatusSummary](../resources/intune_deviceconfig_softwareupdatestatussummary.md)|ソフトウェア更新状態の概要です。|
|deviceCompliancePolicyDeviceStateSummary|[deviceCompliancePolicyDeviceStateSummary](../resources/intune_deviceconfig_devicecompliancepolicydevicestatesummary.md)|このアカウントのデバイス コンプライアンスの状態の要約です。|
|deviceCompliancePolicySettingStateSummaries|[deviceCompliancePolicySettingStateSummary](../resources/intune_deviceconfig_devicecompliancepolicysettingstatesummary.md) コレクション|このアカウントにおける、コンプライアンス ポリシーの設定の状態の要約です。|
|deviceConfigurationDeviceStateSummaries|[deviceConfigurationDeviceStateSummary](../resources/intune_deviceconfig_deviceconfigurationdevicestatesummary.md)|このアカウントにおける、デバイス構成のデバイス状態の要約です。|
|iosUpdateStatuses|[iosUpdateDeviceStatus](../resources/intune_deviceconfig_iosupdatedevicestatus.md) コレクション|このアカウントにおける、iOS ソフトウェアの更新のインストール状態です。|

## <a name="json-representation"></a>JSON 表記
以下は、リソースの JSON 表記です。
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.deviceManagement"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceManagement",
  "id": "String (identifier)",
  "settings": {
    "@odata.type": "microsoft.graph.deviceManagementSettings",
    "deviceComplianceCheckinThresholdDays": 1024,
    "isScheduledActionEnabled": true,
    "secureByDefault": true
  }
}
```



