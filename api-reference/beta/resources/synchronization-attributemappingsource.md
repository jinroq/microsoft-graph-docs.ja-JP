---
title: attributeMappingSource リソースの種類
description: '定義の値がどのようにする必要があります抽出 (変換)、ソース オブジェクトからです。 ソース オブジェクトの特定の属性から取得した単純な値であることなど、文字列の連結/抽出/交換のいくつかのソース属性に基づいたより複雑な式であることができます。 '
localization_priority: Normal
ms.openlocfilehash: 1d15cd82c0a58ac8bdd3ac5805abc166322f27fe
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/24/2019
ms.locfileid: "29510408"
---
# <a name="attributemappingsource-resource-type"></a>attributeMappingSource リソースの種類

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

定義の値がどのようにする必要があります抽出 (変換)、ソース オブジェクトからです。 ソース オブジェクトの特定の属性から取得した単純な値であることなど、文字列の連結/抽出/交換のいくつかのソース属性に基づいたより複雑な式であることができます。 

## <a name="properties"></a>プロパティ

| プロパティ              | 型                      | 説明               |
|:----------------------|:--------------------------|:--------------------------|
|式             |String                     |この**attributeMappingSource**オブジェクトの同等の式表現です。|
|name                   |String                     |マッピングのソースの名前のパラメーター。 **型**のプロパティの値によって、関数の場合、基になる属性、または使用する定数の値の名前の名前できます。 |
|parameters             |[stringKeyAttributeMappingSourceValuePair](synchronization-stringkeyattributemappingsourcevaluepair.md)コレクション | このオブジェクトは、関数を表している場合は、関数のパラメーターを一覧表示します。 パラメーターは、 **attributeMappingSource**オブジェクト自身であり、複雑な正規表現で構成されます。 **型**でない場合`Function`、このプロパティは null または空の配列になります。 |
|type                   | String                    |この属性のマッピングのソースの型。 可能な値は、`Attribute`、`Constant`、`Function` です。 既定値は `Attribute` です。| 

## <a name="json-representation"></a>JSON 表記

リソースの JSON 表記を次に示します。

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.attributeMappingSource"
}-->

```json
{
  "expression": "String",
  "name": "String",
  "parameters": [{"@odata.type": "microsoft.graph.stringKeyAttributeMappingSourceValuePair"}],
  "type": "String"
}
```

## <a name="json-examples"></a>JSON の例

単純な属性を属性のマッピング

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.attributeMappingSource"
}-->

```json
{
    "expression": "[mail]",
    "name": "mail",
    "type": "Attribute"
}
```

ソース属性の最初の 8 文字を抽出する式

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.attributeMappingSource"
}-->

```json
 {
    "expression": "Mid([userPrincipalName], 1, 8)",
    "name": "Mid",
    "parameters": [
        {
            "key": "source",
            "value": {
                "expression": "[userPrincipalName]",
                "name": "userPrincipalName",
                "parameters": [],
                "type": "Attribute"
            }
        },
        {
            "key": "start",
            "value": {
                "expression": "\"1\"",
                "name": "1",
                "parameters": [],
                "type": "Constant"
            }
        },
        {
            "key": "length",
            "value": {
                "expression": "\"8\"",
                "name": "8",
                "parameters": [],
                "type": "Constant"
            }
        }
    ],
    "type": "Function"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "attributeMappingSource resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/synchronization-attributemappingsource.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
