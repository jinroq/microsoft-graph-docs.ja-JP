# <a name="androidworkprofilecustomconfiguration-resource-type"></a>androidWorkProfileCustomConfiguration リソースの種類

> **注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。

Android の作業プロファイルのカスタム構成

[deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md) から継承します

## <a name="methods"></a>メソッド
|メソッド|戻り値の型|説明|
|:---|:---|:---|
|[ androidWorkProfileCustomConfigurationsをリストする](../api/intune_deviceconfig_androidworkprofilecustomconfiguration_list.md)|[androidWorkProfileCustomConfiguration](../resources/intune_deviceconfig_androidworkprofilecustomconfiguration.md) コレクション|[user](../resources/intune_deviceconfig_androidworkprofilecustomconfiguration.md) オブジェクトのプロパティとリレーションシップをリストします。|
|[AndroidWorkProfileCustomConfiguration を取得します](../api/intune_deviceconfig_androidworkprofilecustomconfiguration_get.md)|[androidWorkProfileCustomConfiguration](../resources/intune_deviceconfig_androidworkprofilecustomconfiguration.md)| [AndroidWorkProfileCustomConfiguration](../resources/intune_deviceconfig_androidworkprofilecustomconfiguration.md) オブジェクトのプロパティと関係を参照してください。|
|[AndroidWorkProfileCustomConfiguration を作成します](../api/intune_deviceconfig_androidworkprofilecustomconfiguration_create.md)|[androidWorkProfileCustomConfiguration](../resources/intune_deviceconfig_androidworkprofilecustomconfiguration.md)|新しい [androidWorkProfileCustomConfiguration](../resources/intune_deviceconfig_androidworkprofilecustomconfiguration.md) オブジェクトを作成します。|
|[AndroidWorkProfileCustomConfiguration を削除する](../api/intune_deviceconfig_androidworkprofilecustomconfiguration_delete.md)|なし|[androidWorkProfileCustomConfiguration](../resources/intune_deviceconfig_androidworkprofilecustomconfiguration.md) を削除します。|
|[AndroidWorkProfileCustomConfiguration を更新します](../api/intune_deviceconfig_androidworkprofilecustomconfiguration_update.md)|[androidWorkProfileCustomConfiguration](../resources/intune_deviceconfig_androidworkprofilecustomconfiguration.md)|[AndroidWorkProfileCustomConfiguration](../resources/intune_deviceconfig_androidworkprofilecustomconfiguration.md) オブジェクトのプロパティを更新します。|

## <a name="properties"></a>プロパティ
|プロパティ|型|説明|
|:---|:---|:---|
|ID|文字列|エンティティのキー。 [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md) から継承します|
|lastModifiedDateTime|DateTimeOffset|オブジェクトが最後に変更された DateTime。 [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md) から継承します|
|createdDateTime|DateTimeOffset|オブジェクトが作成された DateTime。 [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md) から継承します|
|説明|文字列|デバイス構成について管理者が提供した説明。 [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md) から継承します|
|displayName|文字列|デバイス構成について管理者が指定した名前。 [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md) から継承します|
|バージョン|Int32|デバイス構成のバージョン。 [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md) から継承します|
|omaSettings|[omaSetting](../resources/intune_deviceconfig_omasetting.md) コレクション|OMA 設定。 このコレクションには、最大で 500 個の要素を含めることができます。|

## <a name="relationships"></a>リレーションシップ
|リレーションシップ|型|説明|
|:---|:---|:---|
|割り当て|[deviceConfigurationAssignment](../resources/intune_deviceconfig_deviceconfigurationassignment.md) コレクション|デバイスの構成プロファイルの割り当てのリスト。 [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md) から継承します|
|deviceStatuses|[deviceConfigurationDeviceStatus](../resources/intune_deviceconfig_deviceconfigurationdevicestatus.md) コレクション|デバイスごとのデバイス構成のインストール状況。 [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md) から継承します|
|userStatuses|[deviceConfigurationUserStatus](../resources/intune_deviceconfig_deviceconfigurationuserstatus.md) コレクション|ユーザーごとのデバイス構成のインストール状況。 [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md) から継承します|
|deviceStatusOverview|[deviceConfigurationDeviceOverview](../resources/intune_deviceconfig_deviceconfigurationdeviceoverview.md)|デバイス構成のデバイス状態の概要 ([deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md) から継承)|
|userStatusOverview|[deviceConfigurationUserOverview](../resources/intune_deviceconfig_deviceconfigurationuseroverview.md)|デバイス構成のユーザー状態の概要 ([deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md) から継承)|
|deviceSettingStateSummaries|[settingStateDeviceSummary](../resources/intune_deviceconfig_settingstatedevicesummary.md) コレクション|デバイス構成設定状態のデバイスの要約 ([deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md) から継承)|

## <a name="json-representation"></a>JSON 表記
以下は、リソースの JSON 表記です。
<!--{
  "blockType": "resource",
  "baseType": "microsoft.graph.deviceConfiguration",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.androidWorkProfileCustomConfiguration"
}-->
``` json
{
  "@odata.type": "#microsoft.graph.androidWorkProfileCustomConfiguration",
  "id": "String (identifier)",
  "lastModifiedDateTime": "String (timestamp)",
  "createdDateTime": "String (timestamp)",
  "description": "String",
  "displayName": "String",
  "version": 1024,
  "omaSettings": [
    {
      "@odata.type": "microsoft.graph.omaSetting",
      "displayName": "String",
      "description": "String",
      "omaUri": "String",
      "value": 1024
    }
  ]
}
```







