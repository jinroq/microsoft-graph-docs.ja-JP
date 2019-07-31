---
title: attributeMappingSource リソースの種類
description: 'ソースオブジェクトから値を抽出 (変換) する方法を定義します。 たとえば、ソースオブジェクトの特定の属性から取得した単純な値を指定することも、複数のソース属性に基づいて文字列の連結/抽出/置換を行うより複雑な式にすることもできます。 '
localization_priority: Normal
doc_type: resourcePageType
author: davidmu1
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 4e2f0e3b3d5ce3ca0c1fef55f81aa454b149e5a2
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "36007971"
---
# <a name="attributemappingsource-resource-type"></a>attributeMappingSource リソースの種類

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

ソースオブジェクトから値を抽出 (変換) する方法を定義します。 たとえば、ソースオブジェクトの特定の属性から取得した単純な値を指定することも、複数のソース属性に基づいて文字列の連結/抽出/置換を行うより複雑な式にすることもできます。 

## <a name="properties"></a>プロパティ

| プロパティ              | 型                      | 説明               |
|:----------------------|:--------------------------|:--------------------------|
|式             |String                     |この**attributeMappingSource**オブジェクトの同等の式表現。|
|name                   |String                     |マッピングソースの Name パラメーター。 **Type**プロパティの値に応じて、関数の名前、source 属性の名前、または使用する定数値を指定できます。 |
|parameters             |[stringKeyAttributeMappingSourceValuePair](synchronization-stringkeyattributemappingsourcevaluepair.md)コレクション | このオブジェクトが関数を表す場合は、関数パラメータを一覧表示します。 パラメータは、 **attributeMappingSource**オブジェクト自体で構成され、複雑な式を使用できます。 **Type**がでは`Function`ない場合、このプロパティは null または空の配列になります。 |
|type                   | String                    |この属性マッピングソースの種類。 可能な値は、`Attribute`、`Constant`、`Function` です。 既定値は `Attribute` です。| 

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

シンプルな属性から属性へのマッピング

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

Source 属性から最初の8文字を抽出する式

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
  "suppressions": []
}
-->
