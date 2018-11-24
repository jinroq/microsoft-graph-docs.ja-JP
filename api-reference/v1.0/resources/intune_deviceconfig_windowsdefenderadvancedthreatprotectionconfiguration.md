# <a name="windowsdefenderadvancedthreatprotectionconfiguration-resource-type"></a>windowsDefenderAdvancedThreatProtectionConfiguration リソースの種類

> **注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。

Windows Defender AdvancedThreatProtection 構成です。

[deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md) から継承します

## <a name="methods"></a>メソッド
|メソッド|戻り値の型|説明|
|:---|:---|:---|
|[windowsDefenderAdvancedThreatProtectionConfigurations のリスト](../api/intune_deviceconfig_windowsdefenderadvancedthreatprotectionconfiguration_list.md)|[windowsDefenderAdvancedThreatProtectionConfiguration](../resources/intune_deviceconfig_windowsdefenderadvancedthreatprotectionconfiguration.md) コレクション|[windowsDefenderAdvancedThreatProtectionConfiguration](../resources/intune_deviceconfig_windowsdefenderadvancedthreatprotectionconfiguration.md) オブジェクトのプロパティとリレーションシップをリストします。|
|[windowsDefenderAdvancedThreatProtectionConfiguration の取得](../api/intune_deviceconfig_windowsdefenderadvancedthreatprotectionconfiguration_get.md)|[windowsDefenderAdvancedThreatProtectionConfiguration](../resources/intune_deviceconfig_windowsdefenderadvancedthreatprotectionconfiguration.md)|[windowsDefenderAdvancedThreatProtectionConfiguration](../resources/intune_deviceconfig_windowsdefenderadvancedthreatprotectionconfiguration.md) オブジェクトのプロパティとリレーションシップを読み取ります。|
|[windowsDefenderAdvancedThreatProtectionConfiguration の作成](../api/intune_deviceconfig_windowsdefenderadvancedthreatprotectionconfiguration_create.md)|[windowsDefenderAdvancedThreatProtectionConfiguration](../resources/intune_deviceconfig_windowsdefenderadvancedthreatprotectionconfiguration.md)|新しい [windowsDefenderAdvancedThreatProtectionConfigurations](../resources/intune_deviceconfig_windowsdefenderadvancedthreatprotectionconfiguration.md) オブジェクトを作成します。|
|[windowsDefenderAdvancedThreatProtectionConfiguration の削除](../api/intune_deviceconfig_windowsdefenderadvancedthreatprotectionconfiguration_delete.md)|なし|[windowsDefenderAdvancedThreatProtectionConfiguration](../resources/intune_deviceconfig_windowsdefenderadvancedthreatprotectionconfiguration.md) を削除します。|
|[windowsDefenderAdvancedThreatProtectionConfiguration の更新](../api/intune_deviceconfig_windowsdefenderadvancedthreatprotectionconfiguration_update.md)|[windowsDefenderAdvancedThreatProtectionConfiguration](../resources/intune_deviceconfig_windowsdefenderadvancedthreatprotectionconfiguration.md)|[windowsDefenderAdvancedThreatProtectionConfiguration](../resources/intune_deviceconfig_windowsdefenderadvancedthreatprotectionconfiguration.md) オブジェクトのプロパティを更新します。|

## <a name="properties"></a>プロパティ
|プロパティ|型|説明|
|:---|:---|:---|
|id|String|エンティティのキー。 [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md) から継承します|
|lastModifiedDateTime|DateTimeOffset|オブジェクトが最後に変更された DateTime。 [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md) から継承します|
|createdDateTime|DateTimeOffset|オブジェクトが作成された DateTime。 [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md) から継承します|
|description|String|デバイス構成について管理者が提供した説明。 [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md) から継承します|
|displayName|String|デバイス構成について管理者が指定した名前。 [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md) から継承します|
|version|Int32|デバイス構成のバージョン。 [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md) から継承します|
|allowSampleSharing|Boolean|Windows Defender AdvancedThreatProtection の「サンプルの共有を許可する」ルール|
|enableExpeditedTelemetryReporting|Boolean|Windows Defender Advanced Threat Protection テレメトリ レポートの頻度を高めます。|

## <a name="relationships"></a>リレーションシップ
|リレーションシップ|型|説明|
|:---|:---|:---|
|assignments|[deviceConfigurationAssignment](../resources/intune_deviceconfig_deviceconfigurationassignment.md) コレクション|デバイスの構成プロファイルの割り当てのリスト。 [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md) から継承します|
|deviceStatuses|[deviceConfigurationDeviceStatus](../resources/intune_deviceconfig_deviceconfigurationdevicestatus.md) コレクション|デバイスごとのデバイス構成のインストール状況。 [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md) から継承します|
|userStatuses|[deviceConfigurationUserStatus](../resources/intune_deviceconfig_deviceconfigurationuserstatus.md) コレクション|ユーザーごとのデバイス構成のインストール状態です。 [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md) から継承します|
|deviceStatusOverview|[deviceConfigurationDeviceOverview](../resources/intune_deviceconfig_deviceconfigurationdeviceoverview.md)|デバイス構成のデバイス状態の概要 ([deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md) から継承)|
|userStatusOverview|[deviceConfigurationUserOverview](../resources/intune_deviceconfig_deviceconfigurationuseroverview.md)|デバイス構成のユーザー状態の概要 ([deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md) から継承)|
|deviceSettingStateSummaries|[settingStateDeviceSummary](../resources/intune_deviceconfig_settingstatedevicesummary.md) コレクション|デバイス構成設定状態のデバイスの要約 ([deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md) から継承)|

## <a name="json-representation"></a>JSON 表記
以下は、リソースの JSON 表記です。
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.windowsDefenderAdvancedThreatProtectionConfiguration"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.windowsDefenderAdvancedThreatProtectionConfiguration",
  "id": "String (identifier)",
  "lastModifiedDateTime": "String (timestamp)",
  "createdDateTime": "String (timestamp)",
  "description": "String",
  "displayName": "String",
  "version": 1024,
  "allowSampleSharing": true,
  "enableExpeditedTelemetryReporting": true
}
```



