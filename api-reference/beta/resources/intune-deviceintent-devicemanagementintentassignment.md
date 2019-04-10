---
title: devicemanagementintentassignment リソースの種類
description: インテント割り当てエンティティ
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 3a955187e079e1f77accb21361bfe49689f52108
ms.sourcegitcommit: 77f485ec03a8c917f59d2fbed4df1ec755f3da58
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/08/2019
ms.locfileid: "31522427"
---
# <a name="devicemanagementintentassignment-resource-type"></a>devicemanagementintentassignment リソースの種類

> **重要:** ベータ版の Microsoft Graph api は変更される可能性があります。運用環境での使用はサポートされていません。

> **注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。

インテント割り当てエンティティ

## <a name="methods"></a>メソッド
|メソッド|戻り値の型|説明|
|:---|:---|:---|
|[devicemanagementintentassignments のリスト](../api/intune-deviceintent-devicemanagementintentassignment-list.md)|[devicemanagementintentassignment](../resources/intune-deviceintent-devicemanagementintentassignment.md)コレクション|[devicemanagementintentassignment](../resources/intune-deviceintent-devicemanagementintentassignment.md)オブジェクトのプロパティとリレーションシップをリストします。|
|[devicemanagementintentassignment の取得](../api/intune-deviceintent-devicemanagementintentassignment-get.md)|[devicemanagementintentassignment](../resources/intune-deviceintent-devicemanagementintentassignment.md)|[devicemanagementintentassignment](../resources/intune-deviceintent-devicemanagementintentassignment.md)オブジェクトのプロパティとリレーションシップを読み取ります。|
|[devicemanagementintentassignment の作成](../api/intune-deviceintent-devicemanagementintentassignment-create.md)|[devicemanagementintentassignment](../resources/intune-deviceintent-devicemanagementintentassignment.md)|新しい[devicemanagementintentassignment](../resources/intune-deviceintent-devicemanagementintentassignment.md)オブジェクトを作成します。|
|[devicemanagementintentassignment の削除](../api/intune-deviceintent-devicemanagementintentassignment-delete.md)|なし|[devicemanagementintentassignment](../resources/intune-deviceintent-devicemanagementintentassignment.md)を削除します。|
|[devicemanagementintentassignment の更新](../api/intune-deviceintent-devicemanagementintentassignment-update.md)|[devicemanagementintentassignment](../resources/intune-deviceintent-devicemanagementintentassignment.md)|[devicemanagementintentassignment](../resources/intune-deviceintent-devicemanagementintentassignment.md)オブジェクトのプロパティを更新します。|

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






