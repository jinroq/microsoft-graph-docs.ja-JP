---
title: windowsInformationProtectionDeviceRegistration リソースの種類
description: Bring-Your-Own-Device(BYOD) Windows デバイスのデバイス登録のレコードを表します。
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 5ae81d973db8c47d9fa613db0eb1b661bb8fa0f9
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/23/2019
ms.locfileid: "29430368"
---
# <a name="windowsinformationprotectiondeviceregistration-resource-type"></a>windowsInformationProtectionDeviceRegistration リソースの種類

> **重要な:**[Microsoft Graph で/beta のバージョンの Api は予告なしに変更されることがあります。 実稼働アプリケーションでこれらの API を使用することは、サポートされていません。

> **注:** Intune の Microsoft グラフ API では、テナントの[Intune のアクティブなライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。

Bring-Your-Own-Device(BYOD) Windows デバイスのデバイス登録のレコードを表します。

## <a name="methods"></a>メソッド
|メソッド|戻り値の型|説明|
|:---|:---|:---|
|[リスト windowsInformationProtectionDeviceRegistrations](../api/intune-mam-windowsinformationprotectiondeviceregistration-list.md)|[windowsInformationProtectionDeviceRegistration](../resources/intune-mam-windowsinformationprotectiondeviceregistration.md)コレクション|[WindowsInformationProtectionDeviceRegistration](../resources/intune-mam-windowsinformationprotectiondeviceregistration.md)オブジェクトのプロパティと関係を一覧表示します。|
|[WindowsInformationProtectionDeviceRegistration を取得します。](../api/intune-mam-windowsinformationprotectiondeviceregistration-get.md)|[windowsInformationProtectionDeviceRegistration](../resources/intune-mam-windowsinformationprotectiondeviceregistration.md)|[WindowsInformationProtectionDeviceRegistration](../resources/intune-mam-windowsinformationprotectiondeviceregistration.md)オブジェクトのプロパティと関係を参照してください。|
|[WindowsInformationProtectionDeviceRegistration を作成します。](../api/intune-mam-windowsinformationprotectiondeviceregistration-create.md)|[windowsInformationProtectionDeviceRegistration](../resources/intune-mam-windowsinformationprotectiondeviceregistration.md)|新しい[windowsInformationProtectionDeviceRegistration](../resources/intune-mam-windowsinformationprotectiondeviceregistration.md)オブジェクトを作成します。|
|[WindowsInformationProtectionDeviceRegistration を削除します。](../api/intune-mam-windowsinformationprotectiondeviceregistration-delete.md)|なし|の[windowsInformationProtectionDeviceRegistration](../resources/intune-mam-windowsinformationprotectiondeviceregistration.md)を削除します。|
|[WindowsInformationProtectionDeviceRegistration を更新します。](../api/intune-mam-windowsinformationprotectiondeviceregistration-update.md)|[windowsInformationProtectionDeviceRegistration](../resources/intune-mam-windowsinformationprotectiondeviceregistration.md)|[WindowsInformationProtectionDeviceRegistration](../resources/intune-mam-windowsinformationprotectiondeviceregistration.md)オブジェクトのプロパティを更新します。|
|[wipe action](../api/intune-mam-windowsinformationprotectiondeviceregistration-wipe.md)|なし|まだ文書化されていません|

## <a name="properties"></a>プロパティ
|プロパティ|型|説明|
|:---|:---|:---|
|id|String|エンティティのキー。|
|userId|String|このデバイスの登録レコードに関連付けられているユーザーの Id。|
|deviceRegistrationId|String|このデバイスの登録レコードのデバイスの識別子です。|
|deviceName|String|デバイス名。|
|deviceType|String|デバイスの種類、たとえば、Windows のラップトップ コンピューターと Windows phone です。|
|deviceMacAddress|String|デバイスの Mac アドレスです。|
|lastCheckInDateTime|DateTimeOffset|デバイスの最後のチェックインの時間です。|

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




