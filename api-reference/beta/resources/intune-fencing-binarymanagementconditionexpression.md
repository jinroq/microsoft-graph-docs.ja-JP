---
title: binaryManagementConditionExpression リソースの種類
description: 二項演算を使用して評価される管理条件式です。
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 509e03e7d492289fc9615f7f8ad47bf13d5bead4
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/11/2019
ms.locfileid: "27857051"
---
# <a name="binarymanagementconditionexpression-resource-type"></a>binaryManagementConditionExpression リソースの種類

> **重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。 実稼働アプリケーションでの、これらの API の使用はサポートされていません。

> **注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。

二項演算を使用して評価される管理条件式です。

[ManagementConditionExpressionModel](../resources/intune-fencing-managementconditionexpressionmodel.md)から継承します。

## <a name="properties"></a>プロパティ
|プロパティ|種類|説明|
|:---|:---|:---|
|operator|[binaryManagementConditionExpressionOperatorType](../resources/intune-fencing-binarymanagementconditionexpressionoperatortype.md)|二項演算の評価に使用する演算子です。 使用可能な値は、`or`、`and` です。|
|firstOperand|[managementConditionExpressionModel](../resources/intune-fencing-managementconditionexpressionmodel.md)|二項演算の 1 番目のオペランド。|
|secondOperand|[managementConditionExpressionModel](../resources/intune-fencing-managementconditionexpressionmodel.md)|二項演算の 2 番目のオペランド。|

## <a name="relationships"></a>リレーションシップ
なし
## <a name="json-representation"></a>JSON 表記
以下は、リソースの JSON 表記です。
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.binaryManagementConditionExpression"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.binaryManagementConditionExpression",
  "operator": "String",
  "firstOperand": {
    "@odata.type": "microsoft.graph.managementConditionExpressionModel"
  },
  "secondOperand": {
    "@odata.type": "microsoft.graph.managementConditionExpressionModel"
  }
}
```





