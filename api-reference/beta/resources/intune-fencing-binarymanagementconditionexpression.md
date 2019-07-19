---
title: binaryManagementConditionExpression リソースの種類
description: バイナリ演算を使用して評価される管理条件式。
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 97c812c3a26af0401bbdea87997167bcada05a37
ms.sourcegitcommit: 0a62bc5849f27a55d83efce9b3eb01b9711bbe1d
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/14/2019
ms.locfileid: "34994819"
---
# <a name="binarymanagementconditionexpression-resource-type"></a>binaryManagementConditionExpression リソースの種類

> **重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。

> **注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。

バイナリ演算を使用して評価される管理条件式。


[Managementconditionexpression モデル](../resources/intune-fencing-managementconditionexpressionmodel.md)から継承します

## <a name="properties"></a>プロパティ
|プロパティ|型|説明|
|:---|:---|:---|
|operator|[Binarymanagementconditionexpression 演算子の種類](../resources/intune-fencing-binarymanagementconditionexpressionoperatortype.md)|二項演算の評価で使用される演算子です。 可能な値は、`or`、`and` です。|
|firstOperand|[Managementconditionexpression モデル](../resources/intune-fencing-managementconditionexpressionmodel.md)|二項演算の最初のオペランド。|
|この|[Managementconditionexpression モデル](../resources/intune-fencing-managementconditionexpressionmodel.md)|二項演算の2番目のオペランド。|

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





