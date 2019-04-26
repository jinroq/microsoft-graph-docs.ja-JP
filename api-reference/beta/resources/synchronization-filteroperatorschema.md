---
title: filter演算子スキーマリソースの種類
description: フィルターで使用できる演算子を記述します。
localization_priority: Normal
ms.openlocfilehash: 0f0ada4aaa02efa2484ffa75d88b2c8256f15fe8
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/26/2019
ms.locfileid: "33342865"
---
# <a name="filteroperatorschema-resource-type"></a>filter演算子スキーマリソースの種類

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

[フィルター](synchronization-filter.md)で使用できる演算子を記述します。

## <a name="properties"></a>プロパティ

| プロパティ                   | 型                      | 説明    |
|:---------------------------|:--------------------------|:---------------|
|アリ                       |String          |演算子のアリティ。 可能な値は、`Binary`、`Unary` です。 既定値は `Binary` です。|
|multivaluedComparisonType   |scopeOperatorMultiValuedComparisonType          |可能な値は、`All`、`Any` です。 複数値属性にのみ適用されます。 `All`すべての値が条件を満たす必要があることを意味します。 `Any`少なくとも1つの値が条件を満たす必要があることを意味します。 既定値は `All` です。|
|name                        |String                     |オペレーター名。 |
|supportedAttributeTypes     |String collection         |演算子でサポートされている属性の種類。 可能な値は、`Boolean`、`Binary`、`Reference`、`Integer`、`String` です。|

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
