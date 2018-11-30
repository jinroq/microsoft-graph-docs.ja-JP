---
title: filterClause リソースの種類
description: いずれかに候補オブジェクトが満たす必要があります、評価される 1 つのアサーションを表します`true`(オブジェクトでは、アサーションを満たしている) または`false`(オブジェクトでは、アサーションを満たしていません)。
ms.openlocfilehash: 0861324849f224c4e750f0c7b926464280b9a377
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27067699"
---
# <a name="filterclause-resource-type"></a>filterClause リソースの種類

> **重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。 実稼働アプリケーションでの、これらの API の使用はサポートされていません。

いずれかに候補オブジェクトが満たす必要があります、評価される 1 つのアサーションを表します`true`(オブジェクトでは、アサーションを満たしている) または`false`(オブジェクトでは、アサーションを満たしていません)。

## <a name="properties"></a>プロパティ
| プロパティ     | 型   |説明|
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