---
title: unaryManagementConditionExpression リソースの種類
description: 単項演算を使用して評価される管理条件式です。
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: f1224a869ec2ec9cae2f38273f7a68b64d3d7333
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/23/2019
ms.locfileid: "29406781"
---
# <a name="unarymanagementconditionexpression-resource-type"></a>unaryManagementConditionExpression リソースの種類

> **重要な:**[Microsoft Graph で/beta のバージョンの Api は予告なしに変更されることがあります。 実稼働アプリケーションでこれらの API を使用することは、サポートされていません。

> **注:** Intune の Microsoft グラフ API では、テナントの[Intune のアクティブなライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。

単項演算を使用して評価される管理条件式です。


[ManagementConditionExpressionModel](../resources/intune-fencing-managementconditionexpressionmodel.md)から継承します。

## <a name="properties"></a>プロパティ
|プロパティ|型|説明|
|:---|:---|:---|
|operator|[unaryManagementConditionExpressionOperatorType](../resources/intune-fencing-unarymanagementconditionexpressionoperatortype.md)|単項演算の評価に使用する演算子です。 使用可能な値: `not`。|
|オペランド|[managementConditionExpressionModel](../resources/intune-fencing-managementconditionexpressionmodel.md)|単項演算のオペランドです。|

## <a name="relationships"></a>リレーションシップ
なし

## <a name="json-representation"></a>JSON 表記
以下は、リソースの JSON 表記です。
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.unaryManagementConditionExpression"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.unaryManagementConditionExpression",
  "operator": "String",
  "operand": {
    "@odata.type": "microsoft.graph.managementConditionExpressionModel"
  }
}
```




