---
title: filterOperatorSchema リソースの種類
description: フィルターで使用できる演算子をについて説明します。
localization_priority: Normal
ms.openlocfilehash: 04bee90f81c0098832cd4b6355be266668d0f69b
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/24/2019
ms.locfileid: "29515196"
---
# <a name="filteroperatorschema-resource-type"></a>filterOperatorSchema リソースの種類

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

[フィルター](synchronization-filter.md)で使用できる演算子をについて説明します。

## <a name="properties"></a>プロパティ

| プロパティ                   | 型                      | 説明    |
|:---------------------------|:--------------------------|:---------------|
|アリティ                       |String          |演算子のアリティ。 使用可能な値は、`Binary`、`Unary` です。 既定値は `Binary` です。|
|multivaluedComparisonType   |scopeOperatorMultiValuedComparisonType          |使用可能な値は、`All`、`Any` です。 複数値を持つ属性にのみ適用されます。 `All`すべての値が条件を満たす必要があることを意味します。 `Any`条件を満たすために、少なくとも 1 つの値が含まれていることを意味します。 既定値は `All` です。|
|name                        |String                     |オペレーター名です。 |
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
<!--
{
  "type": "#page.annotation",
  "description": "filterOperatorSchema resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/synchronization-filteroperatorschema.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
