---
title: windowsInformationProtectionDeviceRegistration リソースの種類
description: 独自のデバイス (byod) Windows デバイスのデバイス登録レコードを表します。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 4d4403ae2e4629a330fadd5136530d66c8a7d7f2
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 02/21/2019
ms.locfileid: "30161678"
---
# <a name="windowsinformationprotectiondeviceregistration-resource-type"></a>windowsInformationProtectionDeviceRegistration リソースの種類

> **重要:** ベータ版の Microsoft Graph api は変更される可能性があります。運用環境での使用はサポートされていません。

> **注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。

独自のデバイス (byod) Windows デバイスのデバイス登録レコードを表します。

## <a name="methods"></a>メソッド
|メソッド|戻り値の型|説明|
|:---|:---|:---|
|[リスト windowsInformationProtectionDeviceRegistrations](../api/intune-mam-windowsinformationprotectiondeviceregistration-list.md)|[windowsInformationProtectionDeviceRegistration](../resources/intune-mam-windowsinformationprotectiondeviceregistration.md)コレクション|[windowsInformationProtectionDeviceRegistration](../resources/intune-mam-windowsinformationprotectiondeviceregistration.md)オブジェクトのプロパティとリレーションシップをリストします。|
|[windowsInformationProtectionDeviceRegistration を取得する](../api/intune-mam-windowsinformationprotectiondeviceregistration-get.md)|[windowsInformationProtectionDeviceRegistration](../resources/intune-mam-windowsinformationprotectiondeviceregistration.md)|[windowsInformationProtectionDeviceRegistration](../resources/intune-mam-windowsinformationprotectiondeviceregistration.md)オブジェクトのプロパティとリレーションシップを読み取ります。|
|[windowsInformationProtectionDeviceRegistration を作成する](../api/intune-mam-windowsinformationprotectiondeviceregistration-create.md)|[windowsInformationProtectionDeviceRegistration](../resources/intune-mam-windowsinformationprotectiondeviceregistration.md)|新しい[windowsInformationProtectionDeviceRegistration](../resources/intune-mam-windowsinformationprotectiondeviceregistration.md)オブジェクトを作成します。|
|[windowsInformationProtectionDeviceRegistration の削除](../api/intune-mam-windowsinformationprotectiondeviceregistration-delete.md)|なし|[windowsInformationProtectionDeviceRegistration](../resources/intune-mam-windowsinformationprotectiondeviceregistration.md)を削除します。|
|[windowsInformationProtectionDeviceRegistration の更新](../api/intune-mam-windowsinformationprotectiondeviceregistration-update.md)|[windowsInformationProtectionDeviceRegistration](../resources/intune-mam-windowsinformationprotectiondeviceregistration.md)|[windowsInformationProtectionDeviceRegistration](../resources/intune-mam-windowsinformationprotectiondeviceregistration.md)オブジェクトのプロパティを更新します。|
|[wipe action](../api/intune-mam-windowsinformationprotectiondeviceregistration-wipe.md)|なし|まだ文書化されていません|

## <a name="properties"></a>プロパティ
|プロパティ|型|説明|
|:---|:---|:---|
|id|String|エンティティのキー。|
|userId|文字列型 (String)|このデバイス登録レコードに関連付けられている UserId。|
|deviceRegistrationId|String|このデバイス登録レコードのデバイス識別子。|
|deviceName|String|デバイス名。|
|deviceType|String|デバイスの種類。たとえば、windows ラップトップ VS windows phone。|
|deviceMacAddress|String|デバイスの Mac アドレス。|
|lastCheckInDateTime|DateTimeOffset|デバイスの最終チェックイン時刻。|

## <a name="relationships"></a>リレーションシップ
なし

## <a name="json-representation"></a>JSON 表記
以下は、リソースの JSON 表記です。
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.windowsInformationProtectionDeviceRegistration"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.windowsInformationProtectionDeviceRegistration",
  "id": "String (identifier)",
  "userId": "String",
  "deviceRegistrationId": "String",
  "deviceName": "String",
  "deviceType": "String",
  "deviceMacAddress": "String",
  "lastCheckInDateTime": "String (timestamp)"
}
```




