---
title: attributeMappingParameterSchema リソースの種類
description: AttributeMappingFunctionSchema で使用される1つのパラメーターを記述します。
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
ms.openlocfilehash: d8624851d37f475df66ec51f1951ebbbe1ea97a8
ms.sourcegitcommit: 121c0fad692fb3c5c01dc051481b5249e4491b48
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/11/2019
ms.locfileid: "35620270"
---
# <a name="attributemappingparameterschema-resource-type"></a>attributeMappingParameterSchema リソースの種類

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

[AttributeMappingFunctionSchema](../resources/synchronization-attributemappingfunctionschema.md)で使用される1つのパラメーターを記述します。

## <a name="properties"></a>プロパティ

| プロパティ                   | 型                      | 説明    |
|:---------------------------|:-------------------------|:---------------|
|Allow多重オカレンス    |Boolean                   |指定されたパラメーターは、複数回指定できます (たとえば、 `Concatenate(string,string,...)`関数内の複数の入力文字列)。 |
|name                        |String                    |パラメーター名。 |
|必須                    |Boolean                   |`true`パラメーターが必要な場合は、それ`false`以外の場合は。 |
|type                        |String                    |使用可能な値は、`Boolean`、`Binary`、`Reference`、`Integer`、`String` です。 既定値は `String` です。|

## <a name="json-representation"></a>JSON 表記

リソースの JSON 表記を次に示します。

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.attributeMappingParameterSchema"
}-->

```json
{
  "allowMultipleOccurrences": "Boolean",
  "name": "String",
  "required": "Boolean",
  "type": "String"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "attributeMappingParameterSchema resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
