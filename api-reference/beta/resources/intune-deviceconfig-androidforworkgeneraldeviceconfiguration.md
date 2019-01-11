---
title: androidForWorkGeneralDeviceConfiguration リソースの種類
description: Android の作業の一般的なデバイス構成します。
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 445b5eabcc695a8c6d265e9ea2a5d8abb3e904a6
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/11/2019
ms.locfileid: "27860040"
---
# <a name="androidforworkgeneraldeviceconfiguration-resource-type"></a>androidForWorkGeneralDeviceConfiguration リソースの種類

> **重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。 実稼働アプリケーションでの、これらの API の使用はサポートされていません。

> **注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。

Android の作業の一般的なデバイス構成します。

[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します

## <a name="methods"></a>メソッド
|メソッド|戻り値の型|説明|
|:---|:---|:---|
|[リスト androidForWorkGeneralDeviceConfigurations](../api/intune-deviceconfig-androidforworkgeneraldeviceconfiguration-list.md)|[androidForWorkGeneralDeviceConfiguration](../resources/intune-deviceconfig-androidforworkgeneraldeviceconfiguration.md)コレクション|[AndroidForWorkGeneralDeviceConfiguration](../resources/intune-deviceconfig-androidforworkgeneraldeviceconfiguration.md)オブジェクトのプロパティと関係を一覧表示します。|
|[AndroidForWorkGeneralDeviceConfiguration を取得します。](../api/intune-deviceconfig-androidforworkgeneraldeviceconfiguration-get.md)|[androidForWorkGeneralDeviceConfiguration](../resources/intune-deviceconfig-androidforworkgeneraldeviceconfiguration.md)|[AndroidForWorkGeneralDeviceConfiguration](../resources/intune-deviceconfig-androidforworkgeneraldeviceconfiguration.md)オブジェクトのプロパティと関係を参照してください。|
|[AndroidForWorkGeneralDeviceConfiguration を作成します。](../api/intune-deviceconfig-androidforworkgeneraldeviceconfiguration-create.md)|[androidForWorkGeneralDeviceConfiguration](../resources/intune-deviceconfig-androidforworkgeneraldeviceconfiguration.md)|新しい[androidForWorkGeneralDeviceConfiguration](../resources/intune-deviceconfig-androidforworkgeneraldeviceconfiguration.md)オブジェクトを作成します。|
|[AndroidForWorkGeneralDeviceConfiguration を削除します。](../api/intune-deviceconfig-androidforworkgeneraldeviceconfiguration-delete.md)|なし|の[androidForWorkGeneralDeviceConfiguration](../resources/intune-deviceconfig-androidforworkgeneraldeviceconfiguration.md)を削除します。|
|[AndroidForWorkGeneralDeviceConfiguration を更新します。](../api/intune-deviceconfig-androidforworkgeneraldeviceconfiguration-update.md)|[androidForWorkGeneralDeviceConfiguration](../resources/intune-deviceconfig-androidforworkgeneraldeviceconfiguration.md)|[AndroidForWorkGeneralDeviceConfiguration](../resources/intune-deviceconfig-androidforworkgeneraldeviceconfiguration.md)オブジェクトのプロパティを更新します。|

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
|passwordBlockFingerprintUnlock|Boolean|指紋によるロック解除を禁止するかどうかを示します。|
|passwordBlockTrustAgents|Boolean|Smart Lock や他の信頼エージェントをブロックするかどうかを示します。|
|passwordExpirationDays|Int32|パスワードの有効期限が切れるまでの日数。 有効な値は 1 から 365 までです|
|passwordMinimumLength|Int32|パスワードの最小の長さ。 有効な値は 4 から 16 までです|
|passwordMinutesOfInactivityBeforeScreenTimeout|Int32|画面がタイムアウトになるまでの非アクティブ時間 (分)。|
|passwordPreviousPasswordBlockCount|Int32|ブロックする、以前のパスワードの数。 有効な値は 0 から 24 までです|
|passwordSignInFailureCountBeforeFactoryReset|Int32|出荷時の設定にリセットされるまでの、失敗が許可されるサインインの回数。 有効な値は 4 から 11 までです|
|passwordRequiredType|[androidForWorkRequiredPasswordType](../resources/intune-deviceconfig-androidforworkrequiredpasswordtype.md)|必要なパスワードの種類。 可能な値は、`deviceDefault`、`lowSecurityBiometric`、`required`、`atLeastNumeric`、`numericComplex`、`atLeastAlphabetic`、`atLeastAlphanumeric`、`alphanumericWithSymbols` です。|
|workProfileDataSharingType|[androidForWorkCrossProfileDataSharingType](../resources/intune-deviceconfig-androidforworkcrossprofiledatasharingtype.md)|共有するデータの種類を許可します。 可能な値は、`deviceDefault`、`preventAny`、`allowPersonalToWork`、`noRestrictions` です。|
|workProfileBlockNotificationsWhileDeviceLocked|ブール型|デバイスがロックされているときに通知をブロックするかどうかを示します。|
|workProfileBlockAddingAccounts|ブール型|作業プロファイル内のアカウントを追加または削除したり、ユーザーをブロックします。|
|workProfileBluetoothEnableContactSharing|ブール型|企業の連絡先にアクセスするための bluetooth デバイスを使用できます。|
|workProfileBlockScreenCapture|ブール型|作業プロファイルで、画面の取り込みをブロックします。|
|workProfileBlockCrossProfileCallerId|ブール型|ブロックでは、作業プロファイル呼び出し元 ID を表示個人プロファイルにします。|
|workProfileBlockCamera|ブール型|ブロック プロファイル カメラが動作します。|
|workProfileBlockCrossProfileContactsSearch|ブール型|個人プロファイルでは、作業プロファイルの連絡先可用性ブロックです。|
|workProfileBlockCrossProfileCopyPaste|ブール型|プロファイルのコピーと貼り付けが有効になっている間の設定を許可しない場合を示すブール値です。|
|workProfileDefaultAppPermissionPolicy|[androidForWorkDefaultAppPermissionPolicyType](../resources/intune-deviceconfig-androidforworkdefaultapppermissionpolicytype.md)|必要なパスワードの種類。 可能な値は、`deviceDefault`、`prompt`、`autoGrant`、`autoDeny` です。|
|workProfilePasswordBlockFingerprintUnlock|ブール型|指紋をブロックするかどうかを示す作業プロファイルのロックを解除します。|
|workProfilePasswordBlockTrustAgents|ブール型|スマート ロックと作業プロファイルを他の信頼のエージェントをブロックするかどうかを示します。|
|workProfilePasswordExpirationDays|Int32|日前作業プロファイルのパスワードに、の有効期限が切れます。 有効な値は 1 から 365 までです|
|workProfilePasswordMinimumLength|Int32|作業プロファイル パスワードの最小長。 有効な値は 4 から 16 までです|
|workProfilePasswordMinNumericCharacters|Int32|プロファイル パスワードの作業に必要な数字の最小数です。 有効な値 1 ~ 10|
|workProfilePasswordMinNonLetterCharacters|Int32|プロファイル パスワードの作業に必要なアルファベット以外の文字数の最小値です。 有効な値 1 ~ 10|
|workProfilePasswordMinLetterCharacters|Int32|プロファイル パスワードの作業で必要な文字数の最小値。 有効な値 1 ~ 10|
|workProfilePasswordMinLowerCaseCharacters|Int32|作業プロファイルのパスワードに必要な小文字の文字数の最小値です。 有効な値 1 ~ 10|
|workProfilePasswordMinUpperCaseCharacters|Int32|プロファイル パスワードの作業に必要な大文字の文字数の最小値。 有効な値 1 ~ 10|
|workProfilePasswordMinSymbolCharacters|Int32|プロファイル パスワードの作業で必要なシンボル数の最小値です。 有効な値 1 ~ 10|
|workProfilePasswordMinutesOfInactivityBeforeScreenTimeout|Int32|画面がタイムアウトになるまでの非アクティブ時間 (分)。|
|workProfilePasswordPreviousPasswordBlockCount|Int32|ブロックする前の作業プロファイル パスワードの数です。 有効な値は 0 から 24 までです|
|workProfilePasswordSignInFailureCountBeforeFactoryReset|Int32|作業プロファイルが削除されるまでに許容される障害および削除されたすべての企業データの記号の数です。 有効な値は 4 から 11 までです|
|workProfilePasswordRequiredType|[androidForWorkRequiredPasswordType](../resources/intune-deviceconfig-androidforworkrequiredpasswordtype.md)|必要な作業プロファイル パスワードの種類です。 可能な値は、`deviceDefault`、`lowSecurityBiometric`、`required`、`atLeastNumeric`、`numericComplex`、`atLeastAlphabetic`、`atLeastAlphanumeric`、`alphanumericWithSymbols` です。|
|workProfileRequirePassword|ブール型|パスワードが必要な作業プロファイルを|
|securityRequireVerifyApps|Boolean|Android の検証アプリ機能をオンにするよう要求します。|
|vpnAlwaysOnPackageIdentifier|String|常時接続で VPN には、ロックダウン モードを有効にします。|
|vpnEnableAlwaysOnLockdownMode|ブール型|常時接続で VPN には、ロックダウン モードを有効にします。|

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
  "@odata.type": "microsoft.graph.androidForWorkGeneralDeviceConfiguration"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.androidForWorkGeneralDeviceConfiguration",
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
  "passwordBlockFingerprintUnlock": true,
  "passwordBlockTrustAgents": true,
  "passwordExpirationDays": 1024,
  "passwordMinimumLength": 1024,
  "passwordMinutesOfInactivityBeforeScreenTimeout": 1024,
  "passwordPreviousPasswordBlockCount": 1024,
  "passwordSignInFailureCountBeforeFactoryReset": 1024,
  "passwordRequiredType": "String",
  "workProfileDataSharingType": "String",
  "workProfileBlockNotificationsWhileDeviceLocked": true,
  "workProfileBlockAddingAccounts": true,
  "workProfileBluetoothEnableContactSharing": true,
  "workProfileBlockScreenCapture": true,
  "workProfileBlockCrossProfileCallerId": true,
  "workProfileBlockCamera": true,
  "workProfileBlockCrossProfileContactsSearch": true,
  "workProfileBlockCrossProfileCopyPaste": true,
  "workProfileDefaultAppPermissionPolicy": "String",
  "workProfilePasswordBlockFingerprintUnlock": true,
  "workProfilePasswordBlockTrustAgents": true,
  "workProfilePasswordExpirationDays": 1024,
  "workProfilePasswordMinimumLength": 1024,
  "workProfilePasswordMinNumericCharacters": 1024,
  "workProfilePasswordMinNonLetterCharacters": 1024,
  "workProfilePasswordMinLetterCharacters": 1024,
  "workProfilePasswordMinLowerCaseCharacters": 1024,
  "workProfilePasswordMinUpperCaseCharacters": 1024,
  "workProfilePasswordMinSymbolCharacters": 1024,
  "workProfilePasswordMinutesOfInactivityBeforeScreenTimeout": 1024,
  "workProfilePasswordPreviousPasswordBlockCount": 1024,
  "workProfilePasswordSignInFailureCountBeforeFactoryReset": 1024,
  "workProfilePasswordRequiredType": "String",
  "workProfileRequirePassword": true,
  "securityRequireVerifyApps": true,
  "vpnAlwaysOnPackageIdentifier": "String",
  "vpnEnableAlwaysOnLockdownMode": true
}
```





