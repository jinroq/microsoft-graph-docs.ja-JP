---
title: windows10CompliancePolicy リソース タイプ
description: このクラスには、Windows 10 のコンプライアンス設定が含まれています。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: bd6b02332eb56a7f52cd16c678fd5f0702d5a0a0
ms.sourcegitcommit: f58ff560fa02ac95e296375c143b0922fb6a425c
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 03/19/2019
ms.locfileid: "30572356"
---
# <a name="windows10compliancepolicy-resource-type"></a>windows10CompliancePolicy リソース タイプ

> **重要:** ベータ版の Microsoft Graph api は変更される可能性があります。運用環境での使用はサポートされていません。

> **注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。

このクラスには、Windows 10 のコンプライアンス設定が含まれています。


[deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md) から継承します

## <a name="methods"></a>メソッド
|メソッド|戻り値の型|説明|
|:---|:---|:---|
|[List windows10CompliancePolicies](../api/intune-deviceconfig-windows10compliancepolicy-list.md)|[windows10CompliancePolicy](../resources/intune-deviceconfig-windows10compliancepolicy.md) コレクション|[windows10CompliancePolicy](../resources/intune-deviceconfig-windows10compliancepolicy.md) オブジェクトのプロパティとリレーションシップをリストします。|
|[Get windows10CompliancePolicy](../api/intune-deviceconfig-windows10compliancepolicy-get.md)|[windows10CompliancePolicy](../resources/intune-deviceconfig-windows10compliancepolicy.md)|[windows10CompliancePolicy](../resources/intune-deviceconfig-windows10compliancepolicy.md) オブジェクトのプロパティとリレーションシップを読み取ります。|
|[Create windows10CompliancePolicy](../api/intune-deviceconfig-windows10compliancepolicy-create.md)|[windows10CompliancePolicy](../resources/intune-deviceconfig-windows10compliancepolicy.md)|新しい [windows10CompliancePolicy](../resources/intune-deviceconfig-windows10compliancepolicy.md) オブジェクトを作成します。|
|[Delete windows10CompliancePolicy](../api/intune-deviceconfig-windows10compliancepolicy-delete.md)|なし|[windows10CompliancePolicy](../resources/intune-deviceconfig-windows10compliancepolicy.md) を削除します。|
|[Update windows10CompliancePolicy](../api/intune-deviceconfig-windows10compliancepolicy-update.md)|[windows10CompliancePolicy](../resources/intune-deviceconfig-windows10compliancepolicy.md)|[windows10CompliancePolicy](../resources/intune-deviceconfig-windows10compliancepolicy.md) オブジェクトのプロパティを更新します。|

## <a name="properties"></a>プロパティ
|プロパティ|型|説明|
|:---|:---|:---|
|roleScopeTagIds|String collection|このエンティティインスタンスの範囲タグのリスト。 [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md) から継承します|
|id|文字列型 (String)|エンティティのキー。 [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md) から継承します|
|createdDateTime|DateTimeOffset|オブジェクトが作成された DateTime。 [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md) から継承します|
|description|String|管理者が指定した、デバイス構成についての説明。 [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md) から継承します|
|lastModifiedDateTime|DateTimeOffset|オブジェクトの最終更新の DateTime。 [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md) から継承します|
|displayName|String|管理者が指定した、デバイス構成の名前。 [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md) から継承します|
|version|Int32|デバイス構成のバージョン。 [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md) から継承します|
|passwordRequired|Boolean|Windows デバイスのロックを解除するパスワードを要求します。|
|passwordBlockSimple|Boolean|単純なパスワードをブロックするかどうかを示します。|
|passwordRequiredToUnlockFromIdle|Boolean|アイドル デバイスのロックを解除するパスワードを要求します。|
|passwordMinutesOfInactivityBeforeLock|Int32|パスワードが要求されるまでの非アクティブ時間 (分)。|
|passwordExpirationDays|Int32|パスワードの有効期限 (日数)。|
|passwordMinimumLength|Int32|パスワードの最小文字数。|
|passwordMinimumCharacterSetCount|Int32|パスワードに必要な文字セットの数。|
|passwordRequiredType|[requiredpasswordtype](../resources/intune-deviceconfig-requiredpasswordtype.md)|必要なパスワードの種類。 可能な値は、`deviceDefault`、`alphanumeric`、`numeric` です。|
|passwordPreviousPasswordBlockCount|Int32|再使用を禁止する、以前のパスワードの数。|
|requireHealthyDeviceReport|Boolean|デバイスが Windows デバイス正常性構成証明によって正常と報告されることを要求します。|
|osMinimumVersion|String|Windows 10 の最小バージョン。|
|osMaximumVersion|文字列型 (String)|Windows 10 の最大バージョン。|
|mobileOsMinimumVersion|String|Windows Phone の最小バージョン。|
|mobileOsMaximumVersion|String|Windows Phone の最大バージョン。|
|earlyLaunchAntiMalwareDriverEnabled|Boolean|デバイスが Windows デバイス正常性構成証明によって正常と報告される (早期起動マルウェア対策ドライバーが有効である) ことを要求します。|
|bitLockerEnabled|Boolean|デバイスが Windows デバイス正常性構成証明によって正常と報告される (BitLocker が有効である) ことを要求します。|
|secureBootEnabled|Boolean|デバイスが Windows デバイス正常性構成証明によって正常と報告される (セキュア ブートが有効である) ことを要求します。|
|codeIntegrityEnabled|Boolean|デバイスが Windows デバイス正常性構成証明によって正常と報告されることを要求します。|
|storageRequireEncryption|Boolean|Windows デバイス上での暗号化を要求します。|
|activeFirewallRequired|Boolean|Windows デバイスでアクティブなファイアウォールが必要です。|
|defenderenabled|Boolean|windows デバイスで windows Defender マルウェア対策を必須にする。|
|defenderversion|String|windows デバイスで windows Defender マルウェア対策の最小バージョンが必要です。|
|signatureOutOfDate|Boolean|windows デバイスで windows Defender マルウェア対策の署名が最新の状態になっていることを要求します。|
|rtpenabled|Boolean|windows デバイスで windows Defender マルウェア対策のリアルタイム保護を必要とします。|
|antivirusRequired|Boolean|windows Decurity Center に登録されているウイルス対策ソリューション (Symantec、Windows Defender など) を必要とします。|
|antiSpywareRequired|Boolean|windows Decurity Center に登録されているスパイウェア対策ソリューションで、オンおよび監視する必要があります (Symantec、Windows Defender など)。|
|validOperatingSystemBuildRanges|[operatingSystemVersionRange](../resources/intune-deviceconfig-operatingsystemversionrange.md)コレクション|Windows デバイス上の有効なオペレーティングシステムのビルド範囲。 このコレクションには、最大で 10000 個の要素を含めることができます。|
|deviceThreatProtectionEnabled|Boolean|デバイスの脅威保護が有効になっていることを要求します。|
|deviceThreatProtectionRequiredSecurityLevel|[deviceThreatProtectionLevel](../resources/intune-deviceconfig-devicethreatprotectionlevel.md)|デバイスの脅威保護で、コンプライアンス違反を報告するために最低限必要となるリスクレベル。 可能な値は `unavailable`、`secured`、`low`、`medium`、`high`、`notSet` です。|
|configurationManagerComplianceRequired|Boolean|Intune コンプライアンスの状態を考慮に入れて SCCM コンプライアンスの状態を考慮する必要があります。|
|tpmRequired|Boolean|トラステッドプラットフォームモジュール (TPM) が存在することを要求します。|

## <a name="relationships"></a>関係
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
  "@odata.type": "microsoft.graph.windows10CompliancePolicy"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.windows10CompliancePolicy",
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
  "passwordRequiredToUnlockFromIdle": true,
  "passwordMinutesOfInactivityBeforeLock": 1024,
  "passwordExpirationDays": 1024,
  "passwordMinimumLength": 1024,
  "passwordMinimumCharacterSetCount": 1024,
  "passwordRequiredType": "String",
  "passwordPreviousPasswordBlockCount": 1024,
  "requireHealthyDeviceReport": true,
  "osMinimumVersion": "String",
  "osMaximumVersion": "String",
  "mobileOsMinimumVersion": "String",
  "mobileOsMaximumVersion": "String",
  "earlyLaunchAntiMalwareDriverEnabled": true,
  "bitLockerEnabled": true,
  "secureBootEnabled": true,
  "codeIntegrityEnabled": true,
  "storageRequireEncryption": true,
  "activeFirewallRequired": true,
  "defenderEnabled": true,
  "defenderVersion": "String",
  "signatureOutOfDate": true,
  "rtpEnabled": true,
  "antivirusRequired": true,
  "antiSpywareRequired": true,
  "validOperatingSystemBuildRanges": [
    {
      "@odata.type": "microsoft.graph.operatingSystemVersionRange",
      "description": "String",
      "lowestVersion": "String",
      "highestVersion": "String"
    }
  ],
  "deviceThreatProtectionEnabled": true,
  "deviceThreatProtectionRequiredSecurityLevel": "String",
  "configurationManagerComplianceRequired": true,
  "tpmRequired": true
}
```




