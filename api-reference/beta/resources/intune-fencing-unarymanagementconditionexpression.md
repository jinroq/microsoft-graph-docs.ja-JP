---
title: unaryManagementConditionExpression リソースの種類
description: 単項演算を使用して評価される管理条件式です。
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 06a379a53d6d85956a54bede444714e082196ba3
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/12/2019
ms.locfileid: "27949424"
---
# <a name="unarymanagementconditionexpression-resource-type"></a>unaryManagementConditionExpression リソースの種類

> **重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。 実稼働アプリケーションでの、これらの API の使用はサポートされていません。

> **注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。

単項演算を使用して評価される管理条件式です。

[ManagementConditionExpressionModel](../resources/intune-fencing-managementconditionexpressionmodel.md)から継承します。

## <a name="properties"></a>プロパティ
|プロパティ|種類|説明|
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





