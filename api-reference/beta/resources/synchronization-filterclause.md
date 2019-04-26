---
title: filterclause リソースの種類
description: 候補オブジェクトが満たす必要がある1つのアサーションを表し、(オブジェクト`true`がアサートを満たす) または`false` (オブジェクトはアサーションを満たしていない) のどちらかに評価されます。
localization_priority: Normal
ms.openlocfilehash: 657651af512fff0b1daf08985e0f14983ca253f3
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/26/2019
ms.locfileid: "33342976"
---
# <a name="filterclause-resource-type"></a>filterclause リソースの種類

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

候補オブジェクトが満たす必要がある1つのアサーションを表し、(オブジェクト`true`がアサートを満たす) または`false` (オブジェクトはアサーションを満たしていない) のどちらかに評価されます。

## <a name="properties"></a>プロパティ
| プロパティ     | 型   |説明|
|:---------------|:--------|:----------|
|オペレーター名|String|ソースとターゲットのオペランドに適用される演算子の名前です。 サポートされている演算子のいずれかである必要があります。 サポートされている演算子を検出できます。|
|sourceoperandname|String|source オペランドの名前 (テストされているオペランド)。 ソースのオペランド名は、ソースオブジェクトの属性名のいずれかと一致している必要があります。|
|targetoperand|[filteroperand](synchronization-filteroperand.md)|source オペランドのテスト対象となる値を指定します。|

## <a name="json-representation"></a>JSON 表記

リソースの JSON 表記を次に示します。

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.filterClause"
}-->

```json
{
  "operatorName": "String",
  "sourceOperandName": "String",
  "targetOperand": {"@odata.type": "microsoft.graph.filterOperand"}
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "filterClause resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
