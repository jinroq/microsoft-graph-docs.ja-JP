---
title: deviceManagementIntentAssignment リソースの種類
description: インテント割り当てエンティティ
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: e9a5d5ce8d55f70684ef4ce5e0a3c5ff6bf7e536
ms.sourcegitcommit: 0a62bc5849f27a55d83efce9b3eb01b9711bbe1d
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/14/2019
ms.locfileid: "34964011"
---
# <a name="devicemanagementintentassignment-resource-type"></a>deviceManagementIntentAssignment リソースの種類

> **重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。

> **注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。

インテント割り当てエンティティ

## <a name="methods"></a>メソッド
|メソッド|戻り値の型|説明|
|:---|:---|:---|
|[DeviceManagementIntentAssignments のリスト](../api/intune-deviceintent-devicemanagementintentassignment-list.md)|[Devicemanagementintentassignment](../resources/intune-deviceintent-devicemanagementintentassignment.md)コレクション|[Devicemanagementintentassignment](../resources/intune-deviceintent-devicemanagementintentassignment.md)オブジェクトのプロパティとリレーションシップをリストします。|
|[DeviceManagementIntentAssignment の取得](../api/intune-deviceintent-devicemanagementintentassignment-get.md)|[deviceManagementIntentAssignment](../resources/intune-deviceintent-devicemanagementintentassignment.md)|[Devicemanagementintentassignment](../resources/intune-deviceintent-devicemanagementintentassignment.md)オブジェクトのプロパティとリレーションシップを読み取ります。|
|[DeviceManagementIntentAssignment の作成](../api/intune-deviceintent-devicemanagementintentassignment-create.md)|[deviceManagementIntentAssignment](../resources/intune-deviceintent-devicemanagementintentassignment.md)|新しい[Devicemanagementintentassignment](../resources/intune-deviceintent-devicemanagementintentassignment.md)オブジェクトを作成します。|
|[DeviceManagementIntentAssignment の削除](../api/intune-deviceintent-devicemanagementintentassignment-delete.md)|None|[Devicemanagementintentassignment](../resources/intune-deviceintent-devicemanagementintentassignment.md)を削除します。|
|[DeviceManagementIntentAssignment の更新](../api/intune-deviceintent-devicemanagementintentassignment-update.md)|[deviceManagementIntentAssignment](../resources/intune-deviceintent-devicemanagementintentassignment.md)|[Devicemanagementintentassignment](../resources/intune-deviceintent-devicemanagementintentassignment.md)オブジェクトのプロパティを更新します。|

## <a name="properties"></a>プロパティ
|プロパティ|型|説明|
|:---|:---|:---|
|id|String|割り当て ID|
|target|[deviceAndAppManagementAssignmentTarget](../resources/intune-shared-deviceandappmanagementassignmenttarget.md)|割り当て先|

## <a name="relationships"></a>リレーションシップ
なし

## <a name="json-representation"></a>JSON 表記
以下は、リソースの JSON 表記です。
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.deviceManagementIntentAssignment"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceManagementIntentAssignment",
  "id": "String (identifier)",
  "target": {
    "@odata.type": "microsoft.graph.deviceAndAppManagementAssignmentTarget"
  }
}
```





