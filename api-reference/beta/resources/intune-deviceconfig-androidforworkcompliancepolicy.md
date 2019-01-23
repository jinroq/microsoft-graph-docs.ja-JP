---
title: androidForWorkCompliancePolicy リソースの種類
description: このクラスには、作業用のアプリの法令遵守の設定が含まれています。
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 5ef06d8dc052e1cc389c63148808e97dccdde5b1
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/23/2019
ms.locfileid: "29399319"
---
# <a name="androidforworkcompliancepolicy-resource-type"></a>androidForWorkCompliancePolicy リソースの種類

> **重要な:**[Microsoft Graph で/beta のバージョンの Api は予告なしに変更されることがあります。 実稼働アプリケーションでこれらの API を使用することは、サポートされていません。

> **注:** Intune の Microsoft グラフ API では、テナントの[Intune のアクティブなライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。

このクラスには、作業用のアプリの法令遵守の設定が含まれています。


[deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md) から継承します

## <a name="methods"></a>メソッド
|メソッド|戻り値の型|説明|
|:---|:---|:---|
|[リスト androidForWorkCompliancePolicies](../api/intune-deviceconfig-androidforworkcompliancepolicy-list.md)|[androidForWorkCompliancePolicy](../resources/intune-deviceconfig-androidforworkcompliancepolicy.md)コレクション|[AndroidForWorkCompliancePolicy](../resources/intune-deviceconfig-androidforworkcompliancepolicy.md)オブジェクトのプロパティと関係を一覧表示します。|
|[AndroidForWorkCompliancePolicy を取得します。](../api/intune-deviceconfig-androidforworkcompliancepolicy-get.md)|[androidForWorkCompliancePolicy](../resources/intune-deviceconfig-androidforworkcompliancepolicy.md)|[AndroidForWorkCompliancePolicy](../resources/intune-deviceconfig-androidforworkcompliancepolicy.md)オブジェクトのプロパティと関係を参照してください。|
|[AndroidForWorkCompliancePolicy を作成します。](../api/intune-deviceconfig-androidforworkcompliancepolicy-create.md)|[androidForWorkCompliancePolicy](../resources/intune-deviceconfig-androidforworkcompliancepolicy.md)|新しい[androidForWorkCompliancePolicy](../resources/intune-deviceconfig-androidforworkcompliancepolicy.md)オブジェクトを作成します。|
|[AndroidForWorkCompliancePolicy を削除します。](../api/intune-deviceconfig-androidforworkcompliancepolicy-delete.md)|なし|の[androidForWorkCompliancePolicy](../resources/intune-deviceconfig-androidforworkcompliancepolicy.md)を削除します。|
|[AndroidForWorkCompliancePolicy を更新します。](../api/intune-deviceconfig-androidforworkcompliancepolicy-update.md)|[androidForWorkCompliancePolicy](../resources/intune-deviceconfig-androidforworkcompliancepolicy.md)|[AndroidForWorkCompliancePolicy](../resources/intune-deviceconfig-androidforworkcompliancepolicy.md)オブジェクトのプロパティを更新します。|

## <a name="properties"></a>プロパティ
|プロパティ|型|説明|
|:---|:---|:---|
|roleScopeTagIds|String コレクション|このエンティティ インスタンスのスコープのタグのリストです。 [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md) から継承します|
|id|String|エンティティのキー。 [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md) から継承します|
|createdDateTime|DateTimeOffset|オブジェクトが作成された DateTime。 [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md) から継承します|
|説明|String|デバイス構成について管理者が提供した説明。 [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md) から継承します|
|lastModifiedDateTime|DateTimeOffset|オブジェクトが最後に変更された DateTime。 [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md) から継承します|
|displayName|String|デバイス構成について管理者が指定した名前。 [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md) から継承します|
|version|Int32|デバイス構成のバージョン。 [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md) から継承します|
|passwordRequired|Boolean|デバイスのロックを解除するパスワードを要求します。|
|passwordMinimumLength|Int32|パスワードの最小文字数。 有効な値は 4 から 16 までです|
|passwordRequiredType|[androidRequiredPasswordType](../resources/intune-deviceconfig-androidrequiredpasswordtype.md)|パスワード内の文字の種類です。 可能な値は、`deviceDefault`、`alphabetic`、`alphanumeric`、`alphanumericWithSymbols`、`lowSecurityBiometric`、`numeric`、`numericComplex`、`any` です。|
|passwordMinutesOfInactivityBeforeLock|Int32|パスワードが要求されるまでの非アクティブ時間 (分)。|
|passwordExpirationDays|Int32|パスワードの有効期限が切れるまでの日数。 有効な値は 1 から 365 までです|
|passwordPreviousPasswordBlockCount|Int32|禁止する、以前のパスワードの数。 有効な値は 1 から 24 までです|
|passwordSignInFailureCountBeforeFactoryReset|Int32|工場出荷時リセットする前に許容されるサインインの障害の数です。 有効な値 1 ~ 16|
|securityPreventInstallAppsFromUnknownSources|Boolean|デバイスが不明なソースからのアプリのインストールを許可しないことを要求します。|
|securityDisableUsbDebugging|Boolean|Android デバイスでの USB デバッグを無効にします。|
|securityRequireVerifyApps|Boolean|Android の検証アプリ機能をオンにするよう要求します。|
|deviceThreatProtectionEnabled|Boolean|デバイスの脅威保護が有効になっていることを要求します。|
|deviceThreatProtectionRequiredSecurityLevel|[deviceThreatProtectionLevel](../resources/intune-deviceconfig-devicethreatprotectionlevel.md)|Mobile Threat Protection に、コンプライアンス違反をレポートするための最小のリスク レベルを要求します。 可能な値は、`unavailable`、`secured`、`low`、`medium`、`high`、`notSet` です。|
|securityBlockJailbrokenDevices|Boolean|デバイスの脱獄またはルート化を認めません。|
|osMinimumVersion|String|Android の最小バージョン。|
|osMaximumVersion|String|Android の最大バージョン。|
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
|deviceStatuses|[deviceComplianceDeviceStatus](../resources/intune-deviceconfig-devicecompliancedevicestatus.md) コレクション|DeviceComplianceDeviceStatus のリスト。 [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md) から継承します|
|userStatuses|[deviceComplianceUserStatus](../resources/intune-deviceconfig-devicecomplianceuserstatus.md) コレクション|DeviceComplianceUserStatus のリスト。 [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md) から継承します|
|deviceStatusOverview|[deviceComplianceDeviceOverview](../resources/intune-deviceconfig-devicecompliancedeviceoverview.md)|デバイス コンプライアンスとデバイス状態の概要 ([deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md) から継承)|
|userStatusOverview|[deviceComplianceUserOverview](../resources/intune-deviceconfig-devicecomplianceuseroverview.md)|デバイス コンプライアンスのユーザー状態の概要 ([deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md) から継承)|
|deviceSettingStateSummaries|[settingStateDeviceSummary](../resources/intune-deviceconfig-settingstatedevicesummary.md) コレクション|コンプライアンス設定状態のデバイスの要約 ([deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md) から継承)|
|assignments|[deviceCompliancePolicyAssignment](../resources/intune-deviceconfig-devicecompliancepolicyassignment.md) コレクション|このコンプライアンス ポリシーの割り当てのコレクション。 [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md) から継承します|

## <a name="json-representation"></a>JSON 表記
以下は、リソースの JSON 表記です。
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.androidForWorkCompliancePolicy"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.androidForWorkCompliancePolicy",
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
  "passwordMinimumLength": 1024,
  "passwordRequiredType": "String",
  "passwordMinutesOfInactivityBeforeLock": 1024,
  "passwordExpirationDays": 1024,
  "passwordPreviousPasswordBlockCount": 1024,
  "passwordSignInFailureCountBeforeFactoryReset": 1024,
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




