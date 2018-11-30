---
title: filterOperatorSchema リソースの種類
description: フィルターで使用できる演算子をについて説明します。
ms.openlocfilehash: 1a4e21aea2b65073a00c9797065f6788a66e2334
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27067703"
---
# <a name="filteroperatorschema-resource-type"></a>filterOperatorSchema リソースの種類

> **重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。 実稼働アプリケーションでの、これらの API の使用はサポートされていません。

[フィルター](synchronization-filter.md)で使用できる演算子をについて説明します。

## <a name="properties"></a>プロパティ

| プロパティ                   | 型                      | 説明    |
|:---------------------------|:--------------------------|:---------------|
|アリティ                       |String          |演算子のアリティ。 使用可能な値は、`Binary`、`Unary` です。 既定値は `Binary` です。|
|multivaluedComparisonType   |scopeOperatorMultiValuedComparisonType          |使用可能な値は、`All`、`Any` です。 複数値を持つ属性にのみ適用されます。 `All`すべての値が条件を満たす必要があることを意味します。 `Any`条件を満たすために、少なくとも 1 つの値が含まれていることを意味します。 既定値は `All` です。|
|名前                        |String                     |オペレーター名です。 |
|supportedAttributeTypes     |String コレクション         |属性の型が演算子でサポートします。 可能な値は、`Boolean`、`Binary`、`Reference`、`Integer`、`String` です。|

## <a name="json-representation"></a>JSON 表記

リソースの JSON 表記を次に示します。

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.filterOperatorSchema"
}-->

```json
{
  "arity": "String",
  "multivaluedComparisonType": "String",
  "name": "String",
  "supportedAttributeTypes": ["String"]
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "filterOperatorSchema resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->