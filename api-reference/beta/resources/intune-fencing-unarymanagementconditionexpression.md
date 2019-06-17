---
title: 非 Arymanagementconditionexpression リソースの種類
description: 単項演算を使用して評価される管理条件式。
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 5eb5e7ed67b0731cc795ab791c2463294764ead6
ms.sourcegitcommit: 0a62bc5849f27a55d83efce9b3eb01b9711bbe1d
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/14/2019
ms.locfileid: "34990107"
---
# <a name="unarymanagementconditionexpression-resource-type"></a>非 Arymanagementconditionexpression リソースの種類

> **重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。

> **注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。

単項演算を使用して評価される管理条件式。


[Managementconditionexpression モデル](../resources/intune-fencing-managementconditionexpressionmodel.md)から継承します

## <a name="properties"></a>プロパティ
|プロパティ|型|説明|
|:---|:---|:---|
|operator|[非 Arymanagementconditionexpression 演算子の種類](../resources/intune-fencing-unarymanagementconditionexpressionoperatortype.md)|単項演算の評価に使用する演算子。 可能な値は`not`次のとおりです。|
|左辺|[Managementconditionexpression モデル](../resources/intune-fencing-managementconditionexpressionmodel.md)|単項演算のオペランド。|

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





