---
title: ハードウェア情報リソースの種類
description: 特定のデバイスのハードウェア情報。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 0c751b6601c296b01be91792105325e10a52ea2f
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32522483"
---
# <a name="hardwareinformation-resource-type"></a>ハードウェア情報リソースの種類

> **重要:** ベータ版の Microsoft Graph api は変更される可能性があります。運用環境での使用はサポートされていません。

> **注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。

特定のデバイスのハードウェア情報。

## <a name="properties"></a>プロパティ
|プロパティ|型|説明|
|:---|:---|:---|
|シリアル番号|String|シリアル番号です。|
|totalStorageSpace|Int64|デバイスの記憶領域の合計。|
|freeStorageSpace|Int64|デバイスの記憶域スペースを解放します。|
|imei|String|IMEI|
|meid|String|MEID|
|manufacturer|String|デバイスのメーカー|
|model|String|デバイスのモデル|
|phoneNumber|String|デバイスの電話番号|
|subscriberCarrier|String|デバイスのサブスクライバーキャリア|
|cellulartechnology|String|デバイスの携帯電話テクノロジ|
|wifiMac|String|デバイスの WiFi MAC アドレス|
|operatingSystemLanguage|String|デバイスのオペレーティングシステムの言語|
|isSupervised|ブール型|デバイスの監視モード|
|isEncrypted|Boolean|デバイスの暗号化の状態|
|isSharedDevice|ブール型|共有 iPad|
|sharedDeviceCachedUsers|[sharedAppleDeviceUser](../resources/intune-devices-sharedappledeviceuser.md)コレクション|共有 Apple デバイス上のすべてのユーザー|
|tpmSpecificationVersion|String|仕様バージョンを指定する文字列。|
|operatingSystemEdition|String|OS のエディションを指定する文字列。|
|deviceFullQualifiedDomainName|String|デバイスの完全修飾ドメイン名を返します (存在する場合)。 デバイスがドメインに参加していない場合は、空の文字列が返されます。 |
|deviceGuardVirtualizationBasedSecurityHardwareRequirementState|[deviceGuardVirtualizationBasedSecurityHardwareRequirementState](../resources/intune-devices-deviceguardvirtualizationbasedsecurityhardwarerequirementstate.md)|仮想化ベースのセキュリティハードウェア要件の状態。 可能な値は、`meetHardwareRequirements`、`secureBootRequired`、`dmaProtectionRequired`、`hyperVNotSupportedForGuestVM`、`hyperVNotAvailable` です。|
|deviceGuardVirtualizationBasedSecurityState|[deviceGuardVirtualizationBasedSecurityState](../resources/intune-devices-deviceguardvirtualizationbasedsecuritystate.md)|仮想化ベースのセキュリティの状態。 . 可能な値は、`running`、`rebootRequired`、`require64BitArchitecture`、`notLicensed`、`notConfigured`、`doesNotMeetHardwareRequirements`、`other` です。|
|deviceGuardLocalSystemAuthorityCredentialGuardState|[deviceGuardLocalSystemAuthorityCredentialGuardState](../resources/intune-devices-deviceguardlocalsystemauthoritycredentialguardstate.md)|ローカルシステム権限 (LSA) credential guard の状態。 . 可能な値は、`running`、`rebootRequired`、`notLicensed`、`notConfigured`、`virtualizationBasedSecurityNotRunning` です。|

## <a name="relationships"></a>リレーションシップ
なし

## <a name="json-representation"></a>JSON 表記
以下は、リソースの JSON 表記です。
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.hardwareInformation"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.hardwareInformation",
  "serialNumber": "String",
  "totalStorageSpace": 1024,
  "freeStorageSpace": 1024,
  "imei": "String",
  "meid": "String",
  "manufacturer": "String",
  "model": "String",
  "phoneNumber": "String",
  "subscriberCarrier": "String",
  "cellularTechnology": "String",
  "wifiMac": "String",
  "operatingSystemLanguage": "String",
  "isSupervised": true,
  "isEncrypted": true,
  "isSharedDevice": true,
  "sharedDeviceCachedUsers": [
    {
      "@odata.type": "microsoft.graph.sharedAppleDeviceUser",
      "userPrincipalName": "String",
      "dataToSync": true,
      "dataQuota": 1024,
      "dataUsed": 1024
    }
  ],
  "tpmSpecificationVersion": "String",
  "operatingSystemEdition": "String",
  "deviceFullQualifiedDomainName": "String",
  "deviceGuardVirtualizationBasedSecurityHardwareRequirementState": "String",
  "deviceGuardVirtualizationBasedSecurityState": "String",
  "deviceGuardLocalSystemAuthorityCredentialGuardState": "String"
}
```





