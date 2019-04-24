---
title: macOSCompliancePolicy リソースの種類
description: このクラスには、Mac OS のコンプライアンス設定が含まれています。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 716cb1382a92d70a26cdd591b7c51a67f144ebee
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32460542"
---
# <a name="macoscompliancepolicy-resource-type"></a>macOSCompliancePolicy リソースの種類

> **重要:** ベータ版の Microsoft Graph api は変更される可能性があります。運用環境での使用はサポートされていません。

> **注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。

このクラスには、Mac OS のコンプライアンス設定が含まれています。


[deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md) から継承します

## <a name="methods"></a>メソッド
|メソッド|戻り値の型|説明|
|:---|:---|:---|
|[macOSCompliancePolicies のリスト](../api/intune-deviceconfig-macoscompliancepolicy-list.md)|[macOSCompliancePolicy](../resources/intune-deviceconfig-macoscompliancepolicy.md) コレクション|[managedAppPolicy](../resources/intune-deviceconfig-macoscompliancepolicy.md) オブジェクトのプロパティとリレーションシップをリストします。|
|[macOSCompliancePolicy の取得](../api/intune-deviceconfig-macoscompliancepolicy-get.md)|[macOSCompliancePolicy](../resources/intune-deviceconfig-macoscompliancepolicy.md)|[macOSCompliancePolicy](../resources/intune-deviceconfig-macoscompliancepolicy.md) オブジェクトのプロパティとリレーションシップを読み取ります。|
|[macOSCompliancePolicy の作成](../api/intune-deviceconfig-macoscompliancepolicy-create.md)|[macOSCompliancePolicy](../resources/intune-deviceconfig-macoscompliancepolicy.md)|新しい [macOSCompliancePolicy](../resources/intune-deviceconfig-macoscompliancepolicy.md) オブジェクトを作成します。|
|[macOSCompliancePolicy の削除](../api/intune-deviceconfig-macoscompliancepolicy-delete.md)|なし|[macOSCompliancePolicy](../resources/intune-deviceconfig-macoscompliancepolicy.md) を削除します。|
|[macOSCompliancePolicy の更新](../api/intune-deviceconfig-macoscompliancepolicy-update.md)|[macOSCompliancePolicy](../resources/intune-deviceconfig-macoscompliancepolicy.md)|[macOSCompliancePolicy](../resources/intune-deviceconfig-macoscompliancepolicy.md) オブジェクトのプロパティを更新します。|

## <a name="properties"></a>プロパティ
|プロパティ|型|説明|
|:---|:---|:---|
|roleScopeTagIds|String collection|このエンティティインスタンスの範囲タグのリスト。 [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md) から継承します|
|id|文字列型 (String)|エンティティのキー。 [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md) から継承します|
|createdDateTime|DateTimeOffset|オブジェクトが作成された DateTime。 [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md) から継承します|
|説明|String|管理者が指定した、デバイス構成についての説明。 [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md) から継承します|
|lastModifiedDateTime|DateTimeOffset|オブジェクトの最終更新の DateTime。 [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md) から継承します|
|displayName|String|管理者が指定した、デバイス構成の名前。 [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md) から継承します|
|version|Int32|デバイス構成のバージョン。 [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md) から継承します|
|passwordRequired|Boolean|パスワードを要求するかどうかを指定します。|
|passwordBlockSimple|Boolean|単純なパスワードをブロックするかどうかを示します。|
|passwordExpirationDays|Int32|パスワードの有効期限が切れるまでの日数。 有効な値は 1 から 65535 までです|
|passwordMinimumLength|Int32|パスワードの最小の長さ。 有効な値は 4 から 14 までです|
|passwordMinutesOfInactivityBeforeLock|Int32|パスワードが要求されるまでの非アクティブ時間 (分)。|
|passwordPreviousPasswordBlockCount|Int32|禁止する、以前のパスワードの数です。 有効な値は 1 から 24 までです|
|passwordMinimumCharacterSetCount|Int32|パスワードに必要な文字セットの数。|
|passwordRequiredType|[requiredpasswordtype](../resources/intune-deviceconfig-requiredpasswordtype.md)|必要なパスワードの種類。 可能な値は、`deviceDefault`、`alphanumeric`、`numeric` です。|
|osMinimumVersion|String|最小 os バージョン。|
|osMaximumVersion|String|最大 os バージョン。|
|osminimumbuildversion|String|最小 os ビルドバージョン。|
|osmaximumbuildversion|String|最大 os ビルドバージョン。|
|systemIntegrityProtectionEnabled|Boolean|デバイスでシステム整合性の保護が有効になっている必要があります。|
|deviceThreatProtectionEnabled|Boolean|デバイスの脅威保護が有効になっていることを要求します。|
|deviceThreatProtectionRequiredSecurityLevel|[deviceThreatProtectionLevel](../resources/intune-deviceconfig-devicethreatprotectionlevel.md)|Mobile Threat Protection に、コンプライアンス違反をレポートするための最小のリスク レベルを要求します。 可能な値は、`unavailable`、`secured`、`low`、`medium`、`high`、`notSet` です。|
|storageRequireEncryption|Boolean|Mac OS デバイスでの暗号化を要求します。|
|gatekeeperAllowedAppSource|[macOSGatekeeperAppSources](../resources/intune-deviceconfig-macosgatekeeperappsources.md)|macOS デバイスからどのダウンロード場所のアプリを実行できるかを決定する、システムおよびプライバシー設定。 可能な値は、`notConfigured`、`macAppStore`、`macAppStoreAndIdentifiedDevelopers`、`anywhere` です。|
|firewallEnabled|Boolean|ファイアウォールを有効にするかどうかを指定します。|
|firewallBlockAllIncoming|Boolean|[着信接続をすべてブロックする] オプションに対応しています。|
|firewallEnableStealthMode|Boolean|[ステルスモードを有効にする] に相当します。|

## <a name="relationships"></a>リレーションシップ
|リレーションシップ|型|説明|
|:---|:---|:---|
|scheduledActionsForRule|[deviceComplianceScheduledActionForRule](../resources/intune-deviceconfig-devicecompliancescheduledactionforrule.md) コレクション|このルールのスケジュール済みのアクションのリスト ([deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md) から継承)|
|deviceStatuses|[deviceComplianceDeviceStatus](../resources/intune-deviceconfig-devicecompliancedevicestatus.md) コレクション|DeviceComplianceDeviceStatus のリストです。 [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md) から継承します|
|userStatuses|[deviceComplianceUserStatus](../resources/intune-deviceconfig-devicecomplianceuserstatus.md) コレクション|DeviceComplianceUserStatus のリストです。 [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md) から継承します|
|deviceStatusOverview|[deviceComplianceDeviceOverview](../resources/intune-deviceconfig-devicecompliancedeviceoverview.md)|デバイス コンプライアンスのデバイス状態の概要 ([deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md) から継承)|
|userStatusOverview|[deviceComplianceUserOverview](../resources/intune-deviceconfig-devicecomplianceuseroverview.md)|デバイス コンプライアンスのユーザー状態の概要 ([deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md) から継承)|
|deviceSettingStateSummaries|[settingStateDeviceSummary](../resources/intune-deviceconfig-settingstatedevicesummary.md) コレクション|コンプライアンス設定状態のデバイスの要約 ([deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md) から継承)|
|assignments|[deviceCompliancePolicyAssignment](../resources/intune-deviceconfig-devicecompliancepolicyassignment.md) コレクション|このコンプライアンス ポリシーの割り当てのコレクションです。 [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md) から継承します|

## <a name="json-representation"></a>JSON 表記
以下は、リソースの JSON 表記です。
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.macOSCompliancePolicy"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.macOSCompliancePolicy",
  "roleScopeTagIds": [
    "String"
  ],
  "id": "String (identifier)",
  "createdDateTime": "String (timestamp)",
  "description": "String",
  "lastModifiedDateTime": "String (timestamp)",
  "displayName": "String",
  "version": 1024,
  "passwordRequired": true,
  "passwordBlockSimple": true,
  "passwordExpirationDays": 1024,
  "passwordMinimumLength": 1024,
  "passwordMinutesOfInactivityBeforeLock": 1024,
  "passwordPreviousPasswordBlockCount": 1024,
  "passwordMinimumCharacterSetCount": 1024,
  "passwordRequiredType": "String",
  "osMinimumVersion": "String",
  "osMaximumVersion": "String",
  "osMinimumBuildVersion": "String",
  "osMaximumBuildVersion": "String",
  "systemIntegrityProtectionEnabled": true,
  "deviceThreatProtectionEnabled": true,
  "deviceThreatProtectionRequiredSecurityLevel": "String",
  "storageRequireEncryption": true,
  "gatekeeperAllowedAppSource": "String",
  "firewallEnabled": true,
  "firewallBlockAllIncoming": true,
  "firewallEnableStealthMode": true
}
```





