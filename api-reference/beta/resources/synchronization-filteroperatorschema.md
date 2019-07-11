---
title: Filter演算子スキーマリソースの種類
description: フィルターで使用できる演算子を記述します。
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
ms.openlocfilehash: c55838e6e7d12789d1bd84d63dff95b4d9b72efa
ms.sourcegitcommit: 121c0fad692fb3c5c01dc051481b5249e4491b48
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/11/2019
ms.locfileid: "35621369"
---
# <a name="filteroperatorschema-resource-type"></a>Filter演算子スキーマリソースの種類

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

[フィルター](synchronization-filter.md)で使用できる演算子を記述します。

## <a name="properties"></a>プロパティ

| プロパティ                   | 型                      | 説明    |
|:---------------------------|:--------------------------|:---------------|
|アリ                       |String          |演算子のアリティ。 可能な値は、`Binary`、`Unary` です。 既定値は `Binary` です。|
|multivaluedComparisonType   |scopeOperatorMultiValuedComparisonType          |可能な値は、`All`、`Any` です。 複数値属性にのみ適用されます。 `All`すべての値が条件を満たす必要があることを意味します。 `Any`少なくとも1つの値が条件を満たす必要があることを意味します。 既定値は `All` です。|
|name                        |String                     |オペレーター名。 |
|supportedAttributeTypes     |文字列コレクション         |演算子でサポートされている属性の種類。 可能な値は、`Boolean`、`Binary`、`Reference`、`Integer`、`String` です。|

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
<!--
{
  "type": "#page.annotation",
  "description": "filterOperatorSchema resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
