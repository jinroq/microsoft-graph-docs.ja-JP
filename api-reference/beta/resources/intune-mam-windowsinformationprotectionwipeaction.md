---
title: windowsInformationProtectionWipeAction リソースの種類
description: 表しますは、Bring-Your-Own-Device(BYOD) Windows デバイス用のテナント管理者によって発行された要求を拭きます。
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 67af8bdde412381bb6362ef1768dca12fdfce6c2
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/23/2019
ms.locfileid: "29431655"
---
# <a name="windowsinformationprotectionwipeaction-resource-type"></a>windowsInformationProtectionWipeAction リソースの種類

> **重要な:**[Microsoft Graph で/beta のバージョンの Api は予告なしに変更されることがあります。 実稼働アプリケーションでこれらの API を使用することは、サポートされていません。

> **注:** Intune の Microsoft グラフ API では、テナントの[Intune のアクティブなライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。

表しますは、Bring-Your-Own-Device(BYOD) Windows デバイス用のテナント管理者によって発行された要求を拭きます。

## <a name="methods"></a>メソッド
|メソッド|戻り値の型|説明|
|:---|:---|:---|
|[リスト windowsInformationProtectionWipeActions](../api/intune-mam-windowsinformationprotectionwipeaction-list.md)|[windowsInformationProtectionWipeAction](../resources/intune-mam-windowsinformationprotectionwipeaction.md)コレクション|[WindowsInformationProtectionWipeAction](../resources/intune-mam-windowsinformationprotectionwipeaction.md)オブジェクトのプロパティと関係を一覧表示します。|
|[WindowsInformationProtectionWipeAction を取得します。](../api/intune-mam-windowsinformationprotectionwipeaction-get.md)|[windowsInformationProtectionWipeAction](../resources/intune-mam-windowsinformationprotectionwipeaction.md)|[WindowsInformationProtectionWipeAction](../resources/intune-mam-windowsinformationprotectionwipeaction.md)オブジェクトのプロパティと関係を参照してください。|
|[WindowsInformationProtectionWipeAction を作成します。](../api/intune-mam-windowsinformationprotectionwipeaction-create.md)|[windowsInformationProtectionWipeAction](../resources/intune-mam-windowsinformationprotectionwipeaction.md)|新しい[windowsInformationProtectionWipeAction](../resources/intune-mam-windowsinformationprotectionwipeaction.md)オブジェクトを作成します。|
|[WindowsInformationProtectionWipeAction を削除します。](../api/intune-mam-windowsinformationprotectionwipeaction-delete.md)|なし|の[windowsInformationProtectionWipeAction](../resources/intune-mam-windowsinformationprotectionwipeaction.md)を削除します。|
|[WindowsInformationProtectionWipeAction を更新します。](../api/intune-mam-windowsinformationprotectionwipeaction-update.md)|[windowsInformationProtectionWipeAction](../resources/intune-mam-windowsinformationprotectionwipeaction.md)|[WindowsInformationProtectionWipeAction](../resources/intune-mam-windowsinformationprotectionwipeaction.md)オブジェクトのプロパティを更新します。|

## <a name="properties"></a>プロパティ
|プロパティ|型|説明|
|:---|:---|:---|
|id|String|エンティティのキー。|
|status|[actionState](../resources/intune-shared-actionstate.md)|アクションのステータスを消去します。 可能な値は、`none`、`pending`、`canceled`、`active`、`done`、`failed`、`notSupported` です。|
|targetedUserId|String|このワイプ操作のターゲットとなるユーザーの Id。|
|targetedDeviceRegistrationId|String|このワイプ操作のターゲットとなる DeviceRegistrationId。|
|targetedDeviceName|String|ターゲット ・ デバイスの名前です。|
|targetedDeviceMacAddress|String|ターゲット デバイスの Mac アドレスです。|

## <a name="relationships"></a>リレーションシップ
なし

## <a name="json-representation"></a>JSON 表記
以下は、リソースの JSON 表記です。
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.windowsInformationProtectionWipeAction"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.windowsInformationProtectionWipeAction",
  "id": "String (identifier)",
  "status": "String",
  "targetedUserId": "String",
  "targetedDeviceRegistrationId": "String",
  "targetedDeviceName": "String",
  "targetedDeviceMacAddress": "String"
}
```




