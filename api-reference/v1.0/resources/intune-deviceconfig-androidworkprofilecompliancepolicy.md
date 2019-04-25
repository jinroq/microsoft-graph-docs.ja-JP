---
title: androidWorkProfileCompliancePolicy リソースの種類
description: このクラスには、Android ワークプロファイルのコンプライアンス設定が含まれています。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 5b73a4d5631646cdc5781d05b3b8b4758abf8b35
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32575150"
---
# <a name="androidworkprofilecompliancepolicy-resource-type"></a>androidWorkProfileCompliancePolicy リソースの種類

> **注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。

このクラスには、Android ワークプロファイルのコンプライアンス設定が含まれています。


[deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md) から継承します

## <a name="methods"></a>メソッド
|メソッド|戻り値の型|説明|
|:---|:---|:---|
|[リスト androidWorkProfileCompliancePolicies](../api/intune-deviceconfig-androidworkprofilecompliancepolicy-list.md)|[androidWorkProfileCompliancePolicy](../resources/intune-deviceconfig-androidworkprofilecompliancepolicy.md)コレクション|[androidWorkProfileCompliancePolicy](../resources/intune-deviceconfig-androidworkprofilecompliancepolicy.md)オブジェクトのプロパティとリレーションシップをリストします。|
|[androidWorkProfileCompliancePolicy を取得する](../api/intune-deviceconfig-androidworkprofilecompliancepolicy-get.md)|[androidWorkProfileCompliancePolicy](../resources/intune-deviceconfig-androidworkprofilecompliancepolicy.md)|[androidWorkProfileCompliancePolicy](../resources/intune-deviceconfig-androidworkprofilecompliancepolicy.md)オブジェクトのプロパティとリレーションシップを読み取ります。|
|[androidWorkProfileCompliancePolicy を作成する](../api/intune-deviceconfig-androidworkprofilecompliancepolicy-create.md)|[androidWorkProfileCompliancePolicy](../resources/intune-deviceconfig-androidworkprofilecompliancepolicy.md)|新しい[androidWorkProfileCompliancePolicy](../resources/intune-deviceconfig-androidworkprofilecompliancepolicy.md)オブジェクトを作成します。|
|[androidWorkProfileCompliancePolicy の削除](../api/intune-deviceconfig-androidworkprofilecompliancepolicy-delete.md)|なし|[androidWorkProfileCompliancePolicy](../resources/intune-deviceconfig-androidworkprofilecompliancepolicy.md)を削除します。|
|[androidWorkProfileCompliancePolicy の更新](../api/intune-deviceconfig-androidworkprofilecompliancepolicy-update.md)|[androidWorkProfileCompliancePolicy](../resources/intune-deviceconfig-androidworkprofilecompliancepolicy.md)|[androidWorkProfileCompliancePolicy](../resources/intune-deviceconfig-androidworkprofilecompliancepolicy.md)オブジェクトのプロパティを更新します。|

## <a name="properties"></a>プロパティ
|プロパティ|型|説明|
|:---|:---|:---|
|id|文字列型 (String)|エンティティのキー。 [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md) から継承します|
|createdDateTime|DateTimeOffset|オブジェクトが作成された DateTime。 [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md) から継承します|
|説明|String|管理者が指定した、デバイス構成についての説明。 [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md) から継承します|
|lastModifiedDateTime|DateTimeOffset|オブジェクトの最終更新の DateTime。 [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md) から継承します|
|displayName|String|管理者が指定した、デバイス構成の名前。 [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md) から継承します|
|version|Int32|デバイス構成のバージョン。 [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md) から継承します|
|passwordRequired|Boolean|デバイスのロックを解除するパスワードを要求します。|
|passwordMinimumLength|Int32|パスワードの最小文字数。 有効な値は 4 から 16 までです|
|passwordRequiredType|[androidrequiredpasswordtype](../resources/intune-deviceconfig-androidrequiredpasswordtype.md)|パスワードの文字の種類。 可能な値は、`deviceDefault`、`alphabetic`、`alphanumeric`、`alphanumericWithSymbols`、`lowSecurityBiometric`、`numeric`、`numericComplex`、`any` です。|
|passwordMinutesOfInactivityBeforeLock|Int32|パスワードが要求されるまでの非アクティブ時間 (分)。|
|passwordExpirationDays|Int32|パスワードの有効期限が切れるまでの日数。 有効な値は 1 から 365 までです|
|passwordPreviousPasswordBlockCount|Int32|禁止する、以前のパスワードの数です。 有効な値は 1 から 24 までです|
|securityPreventInstallAppsFromUnknownSources|Boolean|デバイスが不明なソースからのアプリのインストールを許可しないことを要求します。|
|securityDisableUsbDebugging|Boolean|Android デバイスでの USB デバッグを無効にします。|
|securityRequireVerifyApps|Boolean|Android の検証アプリ機能をオンにするよう要求します。|
|deviceThreatProtectionEnabled|Boolean|デバイスの脅威保護が有効になっていることを要求します。|
|deviceThreatProtectionRequiredSecurityLevel|[deviceThreatProtectionLevel](../resources/intune-deviceconfig-devicethreatprotectionlevel.md)|Mobile Threat Protection に、コンプライアンス違反をレポートするための最小のリスク レベルを要求します。 可能な値は、`unavailable`、`secured`、`low`、`medium`、`high`、`notSet` です。|
|securityBlockJailbrokenDevices|Boolean|デバイスの脱獄またはルート化を認めません。|
|osMinimumVersion|String|Android の最小バージョン。|
|osMaximumVersion|文字列型 (String)|Android の最大バージョン。|
|minAndroidSecurityPatchLevel|String|Android セキュリティ パッチの最小レベル。|
|storageRequireEncryption|Boolean|Android デバイスでの暗号化を要求します。|
|securityRequireSafetyNetAttestationBasicIntegrity|Boolean|デバイスが SafetyNet の基本整合性チェックに合格することを要求します。|
|securityRequireSafetyNetAttestationCertifiedDevice|Boolean|デバイスが SafetyNet の認定デバイス チェックに合格することを要求します。|
|securityRequireGooglePlayServices|Boolean|Google Play 開発者サービスがデバイスにインストールされて有効になっていることを要求します。|
|securityRequireUpToDateSecurityProviders|Boolean|デバイスに最新のセキュリティ プロバイダーが必要です。 デバイスで Google Play 開発者サービスが有効かつ最新の状態になっている必要があります。|
|securityRequireCompanyPortalAppIntegrity|Boolean|デバイスが会社のポータル クライアント アプリのランタイム整合性チェックに合格することを要求します。|

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
  "@odata.type": "microsoft.graph.androidWorkProfileCompliancePolicy"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.androidWorkProfileCompliancePolicy",
  "id": "String (identifier)",
  "createdDateTime": "String (timestamp)",
  "description": "String",
  "lastModifiedDateTime": "String (timestamp)",
  "displayName": "String",
  "version": 1024,
  "passwordRequired": true,
  "passwordMinimumLength": 1024,
  "passwordRequiredType": "String",
  "passwordMinutesOfInactivityBeforeLock": 1024,
  "passwordExpirationDays": 1024,
  "passwordPreviousPasswordBlockCount": 1024,
  "securityPreventInstallAppsFromUnknownSources": true,
  "securityDisableUsbDebugging": true,
  "securityRequireVerifyApps": true,
  "deviceThreatProtectionEnabled": true,
  "deviceThreatProtectionRequiredSecurityLevel": "String",
  "securityBlockJailbrokenDevices": true,
  "osMinimumVersion": "String",
  "osMaximumVersion": "String",
  "minAndroidSecurityPatchLevel": "String",
  "storageRequireEncryption": true,
  "securityRequireSafetyNetAttestationBasicIntegrity": true,
  "securityRequireSafetyNetAttestationCertifiedDevice": true,
  "securityRequireGooglePlayServices": true,
  "securityRequireUpToDateSecurityProviders": true,
  "securityRequireCompanyPortalAppIntegrity": true
}
```



