---
title: filterClause リソースの種類
description: いずれかに候補オブジェクトが満たす必要があります、評価される 1 つのアサーションを表します`true`(オブジェクトでは、アサーションを満たしている) または`false`(オブジェクトでは、アサーションを満たしていません)。
localization_priority: Normal
ms.openlocfilehash: 89807a6086f661388c8d5b1d5f82bfe973c3af39
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/11/2019
ms.locfileid: "27833860"
---
# <a name="filterclause-resource-type"></a>filterClause リソースの種類

> **重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。 実稼働アプリケーションでの、これらの API の使用はサポートされていません。

いずれかに候補オブジェクトが満たす必要があります、評価される 1 つのアサーションを表します`true`(オブジェクトでは、アサーションを満たしている) または`false`(オブジェクトでは、アサーションを満たしていません)。

## <a name="properties"></a>プロパティ
| プロパティ     | 種類   |説明|
|:---------------|:--------|:----------|
|operatorName|String|ソースとターゲットのオペランドに適用する演算子の名前です。 サポートされている演算子のいずれかをする必要があります。 サポートされている演算子を検出することができます。|
|sourceOperandName|String|ソース オペランド (テスト中のオペランド) の名前です。 ソース オペランドの名前は、ソース オブジェクトの属性の名前のいずれかに一致しなければなりません。|
|targetOperand|[filterOperand](synchronization-filteroperand.md)|ソース オペランドを比較する値です。|

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
<!-- {
  "type": "#page.annotation",
  "description": "filterClause resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
