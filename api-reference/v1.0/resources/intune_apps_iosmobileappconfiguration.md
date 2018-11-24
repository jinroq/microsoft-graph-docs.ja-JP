# <a name="iosmobileappconfiguration-resource-type"></a>iosMobileAppConfiguration リソースの種類

> **注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。

iOS モバイル アプリ構成に関する、プロパティ、継承済みのプロパティ、アクションが含まれています。

[managedDeviceMobileAppConfiguration](../resources/intune_apps_manageddevicemobileappconfiguration.md) から継承します

## <a name="methods"></a>メソッド
|メソッド|戻り値の型|説明|
|:---|:---|:---|
|[iosMobileAppConfigurations のリスト](../api/intune_apps_iosmobileappconfiguration_list.md)|[iosMobileAppConfiguration](../resources/intune_apps_iosmobileappconfiguration.md) コレクション|[iosMobileAppConfiguration](../resources/intune_apps_iosmobileappconfiguration.md) オブジェクトのプロパティとリレーションシップをリストします。|
|[iosMobileAppConfiguration の取得](../api/intune_apps_iosmobileappconfiguration_get.md) |[iosMobileAppConfiguration](../resources/intune_apps_iosmobileappconfiguration.md)|[iosMobileAppConfiguration](../resources/intune_apps_iosmobileappconfiguration.md) オブジェクトのプロパティとリレーションシップを読み取ります。|
|[iosMobileAppConfiguration の作成](../api/intune_apps_iosmobileappconfiguration_create.md)|[iosMobileAppConfiguration](../resources/intune_apps_iosmobileappconfiguration.md)|新しい [iosMobileAppConfiguration](../resources/intune_apps_iosmobileappconfiguration.md) オブジェクトを作成します。|
|[iosMobileAppConfiguration の削除](../api/intune_apps_iosmobileappconfiguration_delete.md)|なし|[iosMobileAppConfiguration](../resources/intune_apps_iosmobileappconfiguration.md) を削除します。|
|[iosMobileAppConfiguration の更新](../api/intune_apps_iosmobileappconfiguration_update.md)|[iosMobileAppConfiguration](../resources/intune_apps_iosmobileappconfiguration.md)|[iosMobileAppConfiguration](../resources/intune_apps_iosmobileappconfiguration.md) オブジェクトのプロパティを更新します。|

## <a name="properties"></a>プロパティ
|プロパティ|型|説明|
|:---|:---|:---|
|id|String|エンティティのキー。 [managedDeviceMobileAppConfiguration](../resources/intune_apps_manageddevicemobileappconfiguration.md) から継承済み|
|targetedMobileApps|String コレクション|関連するアプリ。 [managedDeviceMobileAppConfiguration](../resources/intune_apps_manageddevicemobileappconfiguration.md) から継承済み|
|createdDateTime|DateTimeOffset|オブジェクトが作成された DateTime。 [managedDeviceMobileAppConfiguration](../resources/intune_apps_manageddevicemobileappconfiguration.md) から継承済み|
|description|String|デバイス構成について管理者が提供した説明。 [managedDeviceMobileAppConfiguration](../resources/intune_apps_manageddevicemobileappconfiguration.md) から継承済み|
|lastModifiedDateTime|DateTimeOffset|オブジェクトが最後に変更された DateTime。 [managedDeviceMobileAppConfiguration](../resources/intune_apps_manageddevicemobileappconfiguration.md) から継承済み|
|displayName|String|デバイス構成について管理者が指定した名前。 [managedDeviceMobileAppConfiguration](../resources/intune_apps_manageddevicemobileappconfiguration.md) から継承済み|
|version|Int32|デバイス構成のバージョン。 [managedDeviceMobileAppConfiguration](../resources/intune_apps_manageddevicemobileappconfiguration.md) から継承済み|
|encodedSettingXml|Binary|mdm アプリ 構成 Base 64 バイナリ。|
|settings|[appConfigurationSettingItem](../resources/intune_apps_appconfigurationsettingitem.md) コレクション|アプリの構成設定アイテム。|

## <a name="relationships"></a>リレーションシップ
|リレーションシップ|型|説明|
|:---|:---|:---|
|assignments|[managedDeviceMobileAppConfigurationAssignment](../resources/intune_apps_manageddevicemobileappconfigurationassignment.md) コレクション|アプリ構成のグループ割り当てのリストです。 [managedDeviceMobileAppConfiguration](../resources/intune_apps_manageddevicemobileappconfiguration.md) から継承済み|
|deviceStatuses|[managedDeviceMobileAppConfigurationDeviceStatus](../resources/intune_apps_manageddevicemobileappconfigurationdevicestatus.md)コレクション|ManagedDeviceMobileAppConfigurationDeviceStatus のリストです。 [managedDeviceMobileAppConfiguration](../resources/intune_apps_manageddevicemobileappconfiguration.md) から継承済み|
|userStatuses|[managedDeviceMobileAppConfigurationUserStatus](../resources/intune_apps_manageddevicemobileappconfigurationuserstatus.md) コレクション|ManagedDeviceMobileAppConfigurationUserStatus のリストです。 [managedDeviceMobileAppConfiguration](../resources/intune_apps_manageddevicemobileappconfiguration.md) から継承済み|
|deviceStatusSummary|[managedDeviceMobileAppConfigurationDeviceSummary](../resources/intune_apps_manageddevicemobileappconfigurationdevicesummary.md)|アプリ構成のデバイス状態の要約です。 [managedDeviceMobileAppConfiguration](../resources/intune_apps_manageddevicemobileappconfiguration.md) から継承済み|
|userStatusSummary|[managedDeviceMobileAppConfigurationUserSummary](../resources/intune_apps_manageddevicemobileappconfigurationusersummary.md)|アプリ構成のユーザー状態の要約です。 [managedDeviceMobileAppConfiguration](../resources/intune_apps_manageddevicemobileappconfiguration.md) から継承済み|

## <a name="json-representation"></a>JSON 表記
以下は、リソースの JSON 表記です。
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.iosMobileAppConfiguration"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.iosMobileAppConfiguration",
  "id": "String (identifier)",
  "targetedMobileApps": [
    "String"
  ],
  "createdDateTime": "String (timestamp)",
  "description": "String",
  "lastModifiedDateTime": "String (timestamp)",
  "displayName": "String",
  "version": 1024,
  "encodedSettingXml": "binary",
  "settings": [
    {
      "@odata.type": "microsoft.graph.appConfigurationSettingItem",
      "appConfigKey": "String",
      "appConfigKeyType": "String",
      "appConfigKeyValue": "String"
    }
  ]
}
```



