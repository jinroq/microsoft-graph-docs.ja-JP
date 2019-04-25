---
title: stringKeyAttributeMappingSourceValuePair リソースの種類
description: キーが文字列で、値が attributeMappingSource であるキーと値のペアを表します。
localization_priority: Normal
ms.openlocfilehash: ff914c23a238356a821d2902bf18900cf9957548
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32523225"
---
# <a name="stringkeyattributemappingsourcevaluepair-resource-type"></a>stringKeyAttributeMappingSourceValuePair リソースの種類

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

キーが文字列で、値が[attributeMappingSource](synchronization-attributemappingsource.md)であるキーと値のペアを表します。

## <a name="properties"></a>プロパティ
| プロパティ     | 型   |説明|
|:---------------|:--------|:----------|
|Key|String
|The name of the parameter.|
|value|[attributeMappingSource](synchronization-attributemappingsource.md)|パラメーターの値を指定します。|

## <a name="json-representation"></a>JSON 表記

リソースの JSON 表記を次に示します。

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.stringKeyAttributeMappingSourceValuePair"
}-->

```json
{
  "key": "String",
  "value": {"@odata.type": "microsoft.graph.attributeMappingSource"}
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "stringKeyAttributeMappingSourceValuePair resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/synchronization-stringkeyattributemappingsourcevaluepair.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
