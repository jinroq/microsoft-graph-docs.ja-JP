---
title: hardwareInformation リソースの種類
description: 特定のデバイスのハードウェア情報です。
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 32b6d0e637c477265a6d23f39e531ca89c7e490c
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/23/2019
ms.locfileid: "29394825"
---
# <a name="hardwareinformation-resource-type"></a>hardwareInformation リソースの種類

> **重要な:**[Microsoft Graph で/beta のバージョンの Api は予告なしに変更されることがあります。 実稼働アプリケーションでこれらの API を使用することは、サポートされていません。

> **注:** Intune の Microsoft グラフ API では、テナントの[Intune のアクティブなライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。

特定のデバイスのハードウェア情報です。

## <a name="properties"></a>プロパティ
|プロパティ|型|説明|
|:---|:---|:---|
|シリアル番号|String|シリアル番号です。|
|totalStorageSpace|Int64|デバイスの合計容量。|
|freeStorageSpace|Int64|デバイスの空き容量。|
|imei|String|IMEI|
|meid|String|MEID|
|manufacturer|String|デバイスのメーカー|
|model|String|デバイスのモデル|
|phoneNumber|String|デバイスの電話番号|
|subscriberCarrier|String|デバイスのサブスクライバーのキャリア|
|cellularTechnology|String|デバイスの携帯電話のテクノロジー|
|wifiMac|String|デバイスの WiFi の MAC アドレス|
|operatingSystemLanguage|String|デバイスのオペレーティング システムの言語|
|isSupervised|Boolean|デバイスのコールを管理モード|
|isEncrypted|Boolean|デバイスの暗号化の状態|
|isSharedDevice|Boolean|IPad の共有|
|sharedDeviceCachedUsers|[sharedAppleDeviceUser](../resources/intune-devices-sharedappledeviceuser.md)コレクション|共有の Apple デバイス上のすべてのユーザー|
|tpmSpecificationVersion|String|仕様のバージョンを指定する文字列。|
|operatingSystemEdition|String|OS のエディションを指定する文字列。|
|deviceFullQualifiedDomainName|String|(存在する場合) は、デバイスの完全修飾ドメイン名を返します。 デバイスがドメインに参加していない場合は、空の文字列を返します。 |
|deviceGuardVirtualizationBasedSecurityHardwareRequirementState|[deviceGuardVirtualizationBasedSecurityHardwareRequirementState](../resources/intune-devices-deviceguardvirtualizationbasedsecurityhardwarerequirementstate.md)|仮想化ベースのセキュリティ ハードウェアの要件の状態です。 可能な値は、`meetHardwareRequirements`、`secureBootRequired`、`dmaProtectionRequired`、`hyperVNotSupportedForGuestVM`、`hyperVNotAvailable` です。|
|deviceGuardVirtualizationBasedSecurityState|[deviceGuardVirtualizationBasedSecurityState](../resources/intune-devices-deviceguardvirtualizationbasedsecuritystate.md)|仮想化ベースのセキュリティの状態です。 . 可能な値は、`running`、`rebootRequired`、`require64BitArchitecture`、`notLicensed`、`notConfigured`、`doesNotMeetHardwareRequirements`、`other` です。|
|deviceGuardLocalSystemAuthorityCredentialGuardState|[deviceGuardLocalSystemAuthorityCredentialGuardState](../resources/intune-devices-deviceguardlocalsystemauthoritycredentialguardstate.md)|ローカル システム機関 (LSA) の資格情報のガード状態です。 . 可能な値は、`running`、`rebootRequired`、`notLicensed`、`notConfigured`、`virtualizationBasedSecurityNotRunning` です。|

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




