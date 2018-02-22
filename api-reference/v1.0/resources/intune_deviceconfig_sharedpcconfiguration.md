# <a name="sharedpcconfiguration-resource-type"></a>sharedPCConfiguration リソース タイプ

> **注:**Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。

このトピックでは、sharedPCConfiguration リソースによって公開された、宣言されたメソッド、プロパティ、リレーションシップについて説明します。

[deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md) から継承します

## <a name="methods"></a>メソッド
|メソッド|戻り値の型|説明|
|:---|:---|:---|
|[List sharedPCConfiguration](../api/intune_deviceconfig_sharedpcconfiguration_list.md)|[sharedPCConfiguration](../resources/intune_deviceconfig_sharedpcconfiguration.md) コレクション|[sharedPCConfiguration](../resources/intune_deviceconfig_sharedpcconfiguration.md) オブジェクトのプロパティとリレーションシップをリストします。|
|[Get sharedPCConfiguration](../api/intune_deviceconfig_sharedpcconfiguration_get.md)|[sharedPCConfiguration](../resources/intune_deviceconfig_sharedpcconfiguration.md)|[sharedPCConfiguration](../resources/intune_deviceconfig_sharedpcconfiguration.md) オブジェクトのプロパティとリレーションシップを読み取ります。|
|[Create sharedPCConfiguration](../api/intune_deviceconfig_sharedpcconfiguration_create.md)|[sharedPCConfiguration](../resources/intune_deviceconfig_sharedpcconfiguration.md)|新しい [sharedPCConfiguration](../resources/intune_deviceconfig_sharedpcconfiguration.md) オブジェクトを作成します。|
|[Delete sharedPCConfiguration](../api/intune_deviceconfig_sharedpcconfiguration_delete.md)|なし|[sharedPCConfiguration](../resources/intune_deviceconfig_sharedpcconfiguration.md) を削除します。|
|[Update sharedPCConfiguration](../api/intune_deviceconfig_sharedpcconfiguration_update.md)|[sharedPCConfiguration](../resources/intune_deviceconfig_sharedpcconfiguration.md)|[sharedPCConfiguration](../resources/intune_deviceconfig_sharedpcconfiguration.md) オブジェクトのプロパティを更新します。|

## <a name="properties"></a>プロパティ
|プロパティ|型|説明|
|:---|:---|:---|
|id|String|エンティティのキー。 [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md) から継承します|
|lastModifiedDateTime|DateTimeOffset|オブジェクトの最終更新の DateTime。 [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md) から継承します|
|createdDateTime|DateTimeOffset|オブジェクトが作成された DateTime。 [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md) から継承します|
|description|String|デバイス構成について管理者が提供した説明です。 [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md) から継承します|
|displayName|String|デバイス構成について管理者が指定した名前です。 [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md) から継承します|
|version|Int32|デバイス構成のバージョン。 [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md) から継承します|
|accountManagerPolicy|[sharedPCAccountManagerPolicy](../resources/intune_deviceconfig_sharedpcaccountmanagerpolicy.md)|共有の PC 上でアカウントを管理する方法を指定します。 disableAccountManager が false の場合にのみ適用されます。|
|allowedAccounts|String|共有の PC で使用できるアカウントの種類を示します。 可能な値は、`guest`、`domain` です。|
|allowLocalStorage|Boolean|共有の PC でローカル ストレージを許可するかどうかを指定します。|
|disableAccountManager|Boolean|共有 PC モードのアカウント マネージャーを無効にします。|
|disableEduPolicies|Boolean|既定の共有 PC 教育環境ポリシーを無効にするかどうかを指定します。 Windows 10 RS2 以降では、このポリシーは Enabled を true に設定しなくても適用されます。|
|disablePowerPolicies|Boolean|既定の共有 PC 電源ポリシーを無効にするかどうかを指定します。|
|disableSignInOnResume|Boolean|デバイスがスリープ モードから再開するたびにサインインを求める設定を無効にします。|
|enabled|Boolean|共有 PC モードを有効にし、共有 PC のポリシーを適用します。|
|idleTimeBeforeSleepInSeconds|Int32|PC がスリープ状態になるまでにデバイスがアイドル状態を続ける時間を秒単位で指定します。 この値を 0 に設定すると、スリープ タイムアウトは発生しなくなります。|
|kioskAppDisplayName|String|SetKioskAppUserModelId で指定されたアプリを起動するサインイン画面に表示されるアカウントの表示テキストを指定します。 KioskAppUserModelId が設定されている場合にのみ適用されます。|
|kioskAppUserModelId|String|割り当てられたアクセスで使用するアプリのアプリケーション ユーザー モデル ID を指定します。|
|maintenanceStartTime|TimeOfDay|毎日のメンテナンス時間の開始時刻を指定します。|

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
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.sharedPCConfiguration"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.sharedPCConfiguration",
  "id": "String (identifier)",
  "lastModifiedDateTime": "String (timestamp)",
  "createdDateTime": "String (timestamp)",
  "description": "String",
  "displayName": "String",
  "version": 1024,
  "accountManagerPolicy": {
    "@odata.type": "microsoft.graph.sharedPCAccountManagerPolicy",
    "accountDeletionPolicy": "String",
    "cacheAccountsAboveDiskFreePercentage": 1024,
    "inactiveThresholdDays": 1024,
    "removeAccountsBelowDiskFreePercentage": 1024
  },
  "allowedAccounts": "String",
  "allowLocalStorage": true,
  "disableAccountManager": true,
  "disableEduPolicies": true,
  "disablePowerPolicies": true,
  "disableSignInOnResume": true,
  "enabled": true,
  "idleTimeBeforeSleepInSeconds": 1024,
  "kioskAppDisplayName": "String",
  "kioskAppUserModelId": "String",
  "maintenanceStartTime": "String (time of day)"
}
```



