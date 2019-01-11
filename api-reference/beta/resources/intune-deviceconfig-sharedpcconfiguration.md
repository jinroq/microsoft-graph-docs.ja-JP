---
title: sharedPCConfiguration リソース タイプ
description: このトピックでは、sharedPCConfiguration リソースによって公開された、宣言されたメソッド、プロパティ、リレーションシップについて説明します。
localization_priority: Normal
ms.openlocfilehash: 8671d4a5241439eaec12e09e250eff1b2caa4592
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/11/2019
ms.locfileid: "27831137"
---
# <a name="sharedpcconfiguration-resource-type"></a>sharedPCConfiguration リソース タイプ

> **重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。 実稼働アプリケーションでの、これらの API の使用はサポートされていません。

> **注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。

このトピックでは、sharedPCConfiguration リソースによって公開された、宣言されたメソッド、プロパティ、リレーションシップについて説明します。

[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します

## <a name="methods"></a>メソッド
|メソッド|戻り値の型|説明|
|:---|:---|:---|
|[List sharedPCConfiguration](../api/intune-deviceconfig-sharedpcconfiguration-list.md)|[sharedPCConfiguration](../resources/intune-deviceconfig-sharedpcconfiguration.md) コレクション|[sharedPCConfiguration](../resources/intune-deviceconfig-sharedpcconfiguration.md) オブジェクトのプロパティとリレーションシップをリストします。|
|[Get sharedPCConfiguration](../api/intune-deviceconfig-sharedpcconfiguration-get.md)|[sharedPCConfiguration](../resources/intune-deviceconfig-sharedpcconfiguration.md)|[sharedPCConfiguration](../resources/intune-deviceconfig-sharedpcconfiguration.md) オブジェクトのプロパティとリレーションシップを読み取ります。|
|[Create sharedPCConfiguration](../api/intune-deviceconfig-sharedpcconfiguration-create.md)|[sharedPCConfiguration](../resources/intune-deviceconfig-sharedpcconfiguration.md)|新しい [sharedPCConfiguration](../resources/intune-deviceconfig-sharedpcconfiguration.md) オブジェクトを作成します。|
|[Delete sharedPCConfiguration](../api/intune-deviceconfig-sharedpcconfiguration-delete.md)|なし|[sharedPCConfiguration](../resources/intune-deviceconfig-sharedpcconfiguration.md) を削除します。|
|[Update sharedPCConfiguration](../api/intune-deviceconfig-sharedpcconfiguration-update.md)|[sharedPCConfiguration](../resources/intune-deviceconfig-sharedpcconfiguration.md)|[sharedPCConfiguration](../resources/intune-deviceconfig-sharedpcconfiguration.md) オブジェクトのプロパティを更新します。|

## <a name="properties"></a>プロパティ
|プロパティ|種類|説明|
|:---|:---|:---|
|ID|String|エンティティのキー。 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します|
|lastModifiedDateTime|DateTimeOffset|オブジェクトが最後に変更された DateTime。 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します|
|roleScopeTagIds|String コレクション|このエンティティ インスタンスのスコープのタグのリストです。 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します|
|supportsScopeTags|ブール型|デバイスの構成を基になるスコープのタグの割り当てをサポートしているかどうかを示します。 この値が false であり、エンティティをスコープ指定されたユーザーには表示されませんがある場合、ScopeTags プロパティに割り当てることは許可されていません。 これは、Silverlight で作成されたレガシ ポリシーに対して発生し、削除して、Azure ポータル内のポリシーを再作成することで解決できます。 このプロパティは読み取りのみ可能です。 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します|
|createdDateTime|DateTimeOffset|オブジェクトが作成された DateTime。 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します|
|説明|String|デバイス構成について管理者が提供した説明。 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します|
|displayName|String|デバイス構成について管理者が指定した名前。 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します|
|version|Int32|デバイス構成のバージョン。 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します|
|accountManagerPolicy|[sharedPCAccountManagerPolicy](../resources/intune-deviceconfig-sharedpcaccountmanagerpolicy.md)|共有の PC 上でアカウントを管理する方法を指定します。 disableAccountManager が false の場合にのみ適用されます。|
|allowedAccounts|[sharedPCAllowedAccountType](../resources/intune-deviceconfig-sharedpcallowedaccounttype.md)|共有の PC で使用できるアカウントの種類を示します。 可能な値は、`guest`、`domain` です。|
|localStorage|[有効化](../resources/intune-shared-enablement.md)|共有の PC でローカル ストレージを許可するかどうかを指定します。 可能な値は、`notConfigured`、`enabled`、`disabled` です。|
|allowLocalStorage|Boolean|共有の PC でローカル ストレージを許可するかどうかを指定します。|
|setAccountManager|[有効化](../resources/intune-shared-enablement.md)|共有 PC モードのアカウント マネージャーを無効にします。 可能な値は、`notConfigured`、`enabled`、`disabled` です。|
|disableAccountManager|Boolean|共有 PC モードのアカウント マネージャーを無効にします。|
|setEduPolicies|[有効化](../resources/intune-shared-enablement.md)|PC 教育環境の既定の共有ポリシー構成かどうか、有効、無効としないことを指定します。 Windows 10 RS2 以降では、このポリシーは Enabled を true に設定しなくても適用されます。 可能な値は、`notConfigured`、`enabled`、`disabled` です。|
|disableEduPolicies|Boolean|既定の共有 PC 教育環境ポリシーを無効にするかどうかを指定します。 Windows 10 RS2 以降では、このポリシーは Enabled を true に設定しなくても適用されます。|
|setPowerPolicies|[有効化](../resources/intune-shared-enablement.md)|かどうか既定の共有の PC の電源ポリシーが有効または無効にするを指定します。 可能な値は、`notConfigured`、`enabled`、`disabled` です。|
|disablePowerPolicies|Boolean|既定の共有 PC 電源ポリシーを無効にするかどうかを指定します。|
|signInOnResume|[有効化](../resources/intune-shared-enablement.md)|署名するための要件を指定のときに、デバイスのスリープ状態スリープ モードから。 可能な値は、`notConfigured`、`enabled`、`disabled` です。|
|disableSignInOnResume|Boolean|デバイスがスリープ モードから再開するたびにサインインを求める設定を無効にします。|
|enabled|Boolean|共有 PC モードを有効にし、共有 PC のポリシーを適用します。|
|idleTimeBeforeSleepInSeconds|Int32|PC がスリープ状態になるまでにデバイスがアイドル状態を続ける時間を秒単位で指定します。 この値を 0 に設定すると、スリープ タイムアウトは発生しなくなります。|
|kioskAppDisplayName|String|SetKioskAppUserModelId で指定されたアプリを起動するサインイン画面に表示されるアカウントの表示テキストを指定します。 KioskAppUserModelId が設定されている場合にのみ適用されます。|
|kioskAppUserModelId|String|割り当てられたアクセスで使用するアプリのアプリケーション ユーザー モデル ID を指定します。|
|maintenanceStartTime|TimeOfDay|毎日のメンテナンス時間の開始時刻を指定します。|

## <a name="relationships"></a>リレーションシップ
|リレーションシップ|型|説明|
|:---|:---|:---|
|groupAssignments|[deviceConfigurationGroupAssignment](../resources/intune-deviceconfig-deviceconfigurationgroupassignment.md)コレクション|デバイスの構成プロファイルのグループ割り当てのリストです。 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します|
|assignments|[deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md) コレクション|デバイスの構成プロファイルの割り当てのリスト。 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します|
|deviceStatuses|[deviceConfigurationDeviceStatus](../resources/intune-deviceconfig-deviceconfigurationdevicestatus.md) コレクション|デバイスごとのデバイス構成のインストール状況。 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します|
|userStatuses|[deviceConfigurationUserStatus](../resources/intune-deviceconfig-deviceconfigurationuserstatus.md) コレクション|ユーザーごとのデバイス構成のインストール状態です。 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します|
|deviceStatusOverview|[deviceConfigurationDeviceOverview](../resources/intune-deviceconfig-deviceconfigurationdeviceoverview.md)|デバイス構成のデバイス状態の概要 ([deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承)|
|userStatusOverview|[deviceConfigurationUserOverview](../resources/intune-deviceconfig-deviceconfigurationuseroverview.md)|デバイス構成のユーザー状態の概要 ([deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承)|
|deviceSettingStateSummaries|[settingStateDeviceSummary](../resources/intune-deviceconfig-settingstatedevicesummary.md) コレクション|デバイス構成設定状態のデバイスの要約 ([deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承)|

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
  "roleScopeTagIds": [
    "String"
  ],
  "supportsScopeTags": true,
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
  "localStorage": "String",
  "allowLocalStorage": true,
  "setAccountManager": "String",
  "disableAccountManager": true,
  "setEduPolicies": "String",
  "disableEduPolicies": true,
  "setPowerPolicies": "String",
  "disablePowerPolicies": true,
  "signInOnResume": "String",
  "disableSignInOnResume": true,
  "enabled": true,
  "idleTimeBeforeSleepInSeconds": 1024,
  "kioskAppDisplayName": "String",
  "kioskAppUserModelId": "String",
  "maintenanceStartTime": "String (time of day)"
}
```





