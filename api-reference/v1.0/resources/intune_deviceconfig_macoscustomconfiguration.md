# <a name="macoscustomconfiguration-resource-type"></a>macOSCustomConfiguration リソースの種類

> **注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。

このトピックでは、macOSCustomConfiguration リソースによって公開された、宣言されたメソッド、プロパティ、リレーションシップについて説明します。

[deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md) から継承します

## <a name="methods"></a>メソッド
|メソッド|戻り値の型|説明|
|:---|:---|:---|
|[macOSCustomConfigurations のリスト](../api/intune_deviceconfig_macoscustomconfiguration_list.md)|[macOSCustomConfiguration](../resources/intune_deviceconfig_macoscustomconfiguration.md) コレクション|[macOSCustomConfiguration](../resources/intune_deviceconfig_macoscustomconfiguration.md) オブジェクトのプロパティとリレーションシップをリストします。|
|[macOSCustomConfiguration の取得](../api/intune_deviceconfig_macoscustomconfiguration_get.md)|[macOSCustomConfiguration](../resources/intune_deviceconfig_macoscustomconfiguration.md)|[macOSCustomConfiguration](../resources/intune_deviceconfig_macoscustomconfiguration.md) オブジェクトのプロパティとリレーションシップを読み取ります。|
|[macOSCustomConfiguration の作成](../api/intune_deviceconfig_macoscustomconfiguration_create.md)|[macOSCustomConfiguration](../resources/intune_deviceconfig_macoscustomconfiguration.md)|新しい [macOSCustomConfiguration](../resources/intune_deviceconfig_macoscustomconfiguration.md) オブジェクトを作成します。|
|[macOSCustomConfiguration の削除](../api/intune_deviceconfig_macoscustomconfiguration_delete.md)|なし|[macOSCustomConfiguration](../resources/intune_deviceconfig_macoscustomconfiguration.md) を削除します。|
|[macOSCustomConfiguration の更新](../api/intune_deviceconfig_macoscustomconfiguration_update.md)|[macOSCustomConfiguration](../resources/intune_deviceconfig_macoscustomconfiguration.md)|[macOSCustomConfiguration](../resources/intune_deviceconfig_macoscustomconfiguration.md) オブジェクトのプロパティを更新します。|

## <a name="properties"></a>プロパティ
|プロパティ|タイプ|説明|
|:---|:---|:---|
|id|文字列|エンティティのキー。 [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md) から継承します|
|lastModifiedDateTime|DateTimeOffset|オブジェクトが最後に変更された DateTime。 [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md) から継承します|
|createdDateTime|DateTimeOffset|オブジェクトが作成された DateTime。 [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md) から継承します|
|説明|文字列|デバイス構成について管理者が提供した説明。 [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md) から継承します|
|displayName|文字列|デバイス構成について管理者が指定した名前。 [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md) から継承します|
|version|Int32|デバイス構成のバージョン。 [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md) から継承します|
|payloadName|文字列|ユーザーに表示される名前。|
|payloadFileName|文字列|ペイロード ファイル名 (*.mobileconfig | *.xml)。|
|payload|バイナリ|ペイロード。 (UTF8 でエンコードされたバイト配列)|

## <a name="relationships"></a>リレーションシップ
|リレーションシップ|型|説明|
|:---|:---|:---|
|assignments|[deviceConfigurationAssignment](../resources/intune_deviceconfig_deviceconfigurationassignment.md) コレクション|デバイスの構成プロファイルの割り当てのリスト。 [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md) から継承します|
|deviceStatuses|[deviceConfigurationDeviceStatus](../resources/intune_deviceconfig_deviceconfigurationdevicestatus.md) コレクション|デバイスごとのデバイス構成のインストール状況。 [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md) から継承します|
|userStatuses|[deviceConfigurationUserStatus](../resources/intune_deviceconfig_deviceconfigurationuserstatus.md) コレクション|ユーザーごとのデバイス構成のインストール状況。 [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md) から継承します|
|deviceStatusOverview|[deviceConfigurationDeviceOverview](../resources/intune_deviceconfig_deviceconfigurationdeviceoverview.md)|デバイス構成のデバイス状態の概要 ([deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md) から継承)|
|userStatusOverview|[deviceConfigurationUserOverview](../resources/intune_deviceconfig_deviceconfigurationuseroverview.md)|デバイス構成のユーザー状態の概要 ([deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md) から継承)|
|deviceSettingStateSummaries|[settingStateDeviceSummary](../resources/intune_deviceconfig_settingstatedevicesummary.md) コレクション|デバイス構成設定状態のデバイスの要約 ([deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md) から継承)|

## <a name="json-representation"></a>JSON 表記
以下は、リソースの JSON 表記です。
<!--{
  "blockType": "resource",
  "keyProperty": "id",
  "baseType": "microsoft.graph.deviceConfiguration",
  "@odata.type": "microsoft.graph.macOSCustomConfiguration"
}-->
``` json
{
  "@odata.type": "#microsoft.graph.macOSCustomConfiguration",
  "id": "String (identifier)",
  "lastModifiedDateTime": "String (timestamp)",
  "createdDateTime": "String (timestamp)",
  "description": "String",
  "displayName": "String",
  "version": 1024,
  "payloadName": "String",
  "payloadFileName": "String",
  "payload": "binary"
}
```



