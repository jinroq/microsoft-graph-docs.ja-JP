---
title: attributeMappingParameterSchema リソースの種類
description: AttributeMappingFunctionSchema で使用される 1 つのパラメーターについて説明します。
ms.openlocfilehash: 164387a345f245f390d24b89a349e02ee2242041
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27073172"
---
# <a name="attributemappingparameterschema-resource-type"></a>attributeMappingParameterSchema リソースの種類

> **重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。 実稼働アプリケーションでの、これらの API の使用はサポートされていません。

[AttributeMappingFunctionSchema](../resources/synchronization-attributemappingfunctionschema.md)で使用される 1 つのパラメーターについて説明します。

## <a name="properties"></a>プロパティ

| プロパティ                   | 型                      | 説明    |
|:---------------------------|:-------------------------|:---------------|
|allowMultipleOccurrences    |ブール値                   |複数回指定したパラメーターを提供することができます (などの文字列を複数の入力、`Concatenate(string,string,...)`関数)。 |
|名前                        |String                    |パラメーターの名前です。 |
|必須                    |ブール値                   |`true`場合は、パラメーターが必要です。それ以外の場合`false`。 |
|type                        |String                    |可能な値は、`Boolean`、`Binary`、`Reference`、`Integer`、`String` です。 既定値は `String` です。|

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
<!-- {
  "type": "#page.annotation",
  "description": "attributeMappingParameterSchema resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->