---
title: binarymanagementconditionexpression リソースの種類
description: バイナリ演算を使用して評価される管理条件式。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 50092f7031719fb1050706ed81280a347638117d
ms.sourcegitcommit: 20fef447f7e658a454a3887ea49746142c22e45c
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/11/2019
ms.locfileid: "31799413"
---
# <a name="binarymanagementconditionexpression-resource-type"></a>binarymanagementconditionexpression リソースの種類

> **重要:** ベータ版の Microsoft Graph api は変更される可能性があります。運用環境での使用はサポートされていません。

> **注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。

バイナリ演算を使用して評価される管理条件式。


[managementconditionexpression モデル](../resources/intune-fencing-managementconditionexpressionmodel.md)から継承します

## <a name="properties"></a>プロパティ
|プロパティ|型|説明|
|:---|:---|:---|
|operator|[binarymanagementconditionexpression 演算子の種類](../resources/intune-fencing-binarymanagementconditionexpressionoperatortype.md)|二項演算の評価で使用される演算子です。 可能な値は、`or`、`and` です。|
|firstoperand|[managementconditionexpression モデル](../resources/intune-fencing-managementconditionexpressionmodel.md)|二項演算の最初のオペランド。|
|この|[managementconditionexpression モデル](../resources/intune-fencing-managementconditionexpressionmodel.md)|二項演算の2番目のオペランド。|

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





