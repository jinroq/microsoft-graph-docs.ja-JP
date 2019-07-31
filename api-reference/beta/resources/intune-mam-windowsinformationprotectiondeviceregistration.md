---
title: windowsInformationProtectionDeviceRegistration リソースの種類
description: 独自のデバイス (BYOD) Windows デバイスのデバイス登録レコードを表します。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: dfdcd206f9a26e68e36f83e8c87e191e59612ebe
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "35967876"
---
# <a name="windowsinformationprotectiondeviceregistration-resource-type"></a>windowsInformationProtectionDeviceRegistration リソースの種類

> **重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。

> **注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。

独自のデバイス (BYOD) Windows デバイスのデバイス登録レコードを表します。

## <a name="methods"></a>メソッド
|メソッド|戻り値の型|説明|
|:---|:---|:---|
|[リスト windowsInformationProtectionDeviceRegistrations](../api/intune-mam-windowsinformationprotectiondeviceregistration-list.md)|[windowsInformationProtectionDeviceRegistration](../resources/intune-mam-windowsinformationprotectiondeviceregistration.md)コレクション|[WindowsInformationProtectionDeviceRegistration](../resources/intune-mam-windowsinformationprotectiondeviceregistration.md)オブジェクトのプロパティとリレーションシップをリストします。|
|[WindowsInformationProtectionDeviceRegistration を取得する](../api/intune-mam-windowsinformationprotectiondeviceregistration-get.md)|[windowsInformationProtectionDeviceRegistration](../resources/intune-mam-windowsinformationprotectiondeviceregistration.md)|[WindowsInformationProtectionDeviceRegistration](../resources/intune-mam-windowsinformationprotectiondeviceregistration.md)オブジェクトのプロパティとリレーションシップを読み取ります。|
|[WindowsInformationProtectionDeviceRegistration を作成する](../api/intune-mam-windowsinformationprotectiondeviceregistration-create.md)|[windowsInformationProtectionDeviceRegistration](../resources/intune-mam-windowsinformationprotectiondeviceregistration.md)|新しい[windowsInformationProtectionDeviceRegistration](../resources/intune-mam-windowsinformationprotectiondeviceregistration.md)オブジェクトを作成します。|
|[WindowsInformationProtectionDeviceRegistration の削除](../api/intune-mam-windowsinformationprotectiondeviceregistration-delete.md)|None|[WindowsInformationProtectionDeviceRegistration](../resources/intune-mam-windowsinformationprotectiondeviceregistration.md)を削除します。|
|[WindowsInformationProtectionDeviceRegistration の更新](../api/intune-mam-windowsinformationprotectiondeviceregistration-update.md)|[windowsInformationProtectionDeviceRegistration](../resources/intune-mam-windowsinformationprotectiondeviceregistration.md)|[WindowsInformationProtectionDeviceRegistration](../resources/intune-mam-windowsinformationprotectiondeviceregistration.md)オブジェクトのプロパティを更新します。|
|[wipe action](../api/intune-mam-windowsinformationprotectiondeviceregistration-wipe.md)|なし|まだ文書化されていません|

## <a name="properties"></a>プロパティ
|プロパティ|型|説明|
|:---|:---|:---|
|id|文字列|エンティティのキー。|
|userId|String|このデバイス登録レコードに関連付けられている UserId。|
|deviceRegistrationId|String|このデバイス登録レコードのデバイス識別子。|
|deviceName|String|デバイス名。|
|deviceType|String|デバイスの種類。たとえば、Windows ラップトップ VS Windows phone。|
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





