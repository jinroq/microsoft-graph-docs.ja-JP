# <a name="iosupdateconfiguration-resource-type"></a>iosUpdateConfiguration リソースの種類

> **注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。

iOS 更新構成では、iOS の更新をインストールする、一週間のうちの時間枠を構成できます。

[deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md) から継承します

## <a name="methods"></a>メソッド
|メソッド|戻り値の型|説明|
|:---|:---|:---|
|[iosUpdateConfigurations のリスト](../api/intune_deviceconfig_iosupdateconfiguration_list.md)|[iosUpdateConfiguration](../resources/intune_deviceconfig_iosupdateconfiguration.md) コレクション|[iosUpdateConfiguration](../resources/intune_deviceconfig_iosupdateconfiguration.md) オブジェクトのプロパティとリレーションシップをリストします。|
|[iosUpdateConfiguration の取得](../api/intune_deviceconfig_iosupdateconfiguration_get.md)|[iosUpdateConfiguration](../resources/intune_deviceconfig_iosupdateconfiguration.md)|[iosUpdateConfiguration](../resources/intune_deviceconfig_iosupdateconfiguration.md) オブジェクトのプロパティとリレーションシップを読み取ります。|
|[iosUpdateConfiguration の作成](../api/intune_deviceconfig_iosupdateconfiguration_create.md)|[iosUpdateConfiguration](../resources/intune_deviceconfig_iosupdateconfiguration.md)|新しい [iosUpdateConfiguration](../resources/intune_deviceconfig_iosupdateconfiguration.md) オブジェクトを作成します。|
|[iosUpdateConfiguration の削除](../api/intune_deviceconfig_iosupdateconfiguration_delete.md)|なし|[iosUpdateConfiguration](../resources/intune_deviceconfig_iosupdateconfiguration.md) を削除します。|
|[iosUpdateConfiguration の更新](../api/intune_deviceconfig_iosupdateconfiguration_update.md)|[iosUpdateConfiguration](../resources/intune_deviceconfig_iosupdateconfiguration.md)|[iosUpdateConfiguration](../resources/intune_deviceconfig_iosupdateconfiguration.md) オブジェクトのプロパティを更新します。|

## <a name="properties"></a>プロパティ
|プロパティ|タイプ|説明|
|:---|:---|:---|
|ID|文字列|エンティティのキー。 [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md) から継承します|
|lastModifiedDateTime|DateTimeOffset|オブジェクトが最後に変更された DateTime。 [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md) から継承します|
|createdDateTime|DateTimeOffset|オブジェクトが作成された DateTime。 [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md) から継承します|
|説明|文字列|デバイス構成について管理者が提供した説明。 [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md) から継承します|
|displayName|文字列|デバイス構成について管理者が指定した名前。 [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md) から継承します|
|バージョン|Int32|デバイス構成のバージョン。 [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md) から継承します|
|activeHoursStart|TimeOfDay|アクティブ時間の開始 (アクティブ時間は、更新のインストールが実施されない時間枠のことです)|
|activeHoursEnd|TimeOfDay|アクティブ時間の終了 (アクティブ時間は、更新のインストールが実施されない時間枠のことです)|
|scheduledInstallDays|[dayOfWeek 列挙型](../resources/intune_deviceconfig_dayofweek.md)コレクション|アクティブ時間が設定されている曜日。 このコレクションには、最大で 7 個の要素を含めることができます。|
|utcTimeOffsetInMinutes|Int32|分単位で示す、UTC タイム オフセット|

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
  "keyProperty": "id",
  "baseType": "microsoft.graph.deviceConfiguration",
  "@odata.type": "microsoft.graph.iosUpdateConfiguration"
}-->
``` json
{
  "@odata.type": "#microsoft.graph.iosUpdateConfiguration",
  "id": "String (identifier)",
  "lastModifiedDateTime": "String (timestamp)",
  "createdDateTime": "String (timestamp)",
  "description": "String",
  "displayName": "String",
  "version": 1024,
  "activeHoursStart": "String (time of day)",
  "activeHoursEnd": "String (time of day)",
  "scheduledInstallDays": [
    "String"
  ],
  "utcTimeOffsetInMinutes": 1024
}
```



