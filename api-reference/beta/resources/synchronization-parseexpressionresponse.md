---
title: parseExpressionResponse リソースの種類
description: '応答を表す、 [synchronizationSchema: parseExpression](../api/synchronization_synchronizationschema_parseexpression.md)アクション。'
localization_priority: Normal
ms.openlocfilehash: f8ea708468e1e580693b2bd0e6f0e7f3494996f0
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/24/2019
ms.locfileid: "29523891"
---
# <a name="parseexpressionresponse-resource-type"></a>parseExpressionResponse リソースの種類

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

応答を表す、 [synchronizationSchema: parseExpression](../api/synchronization_synchronizationschema_parseexpression.md)アクション。

## <a name="properties"></a>プロパティ
| プロパティ     | 型   |説明|
|:---------------|:--------|:----------|
|エラー|odata.error|エラーの詳細、式の評価でエラーが発生する場合。|
|evaluationResult|String コレクション|式の評価によって生成された値のコレクションです。|
|evaluationSucceeded|ブール値|`true`場合は、評価が正常に完了しました。|
|parsedExpression|[attributeMappingSource](synchronization-attributemappingsource.md)|解析された式を表す[attributeMappingSource](synchronization-attributemappingsource.md)オブジェクト。|
|parsingSucceeded|ブール値|`true`場合は、式が正しく解析されました。|

## <a name="json-representation"></a>JSON 表記

リソースの JSON 表記を次に示します。

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.parseExpressionResponse"
}-->

```json
{
  "error": {"@odata.type": "microsoft.graph.publicError"},
  "evaluationResult": ["String"],
  "evaluationSucceeded": true,
  "parsedExpression": {"@odata.type": "microsoft.graph.attributeMappingSource"},
  "parsingSucceeded": true
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "parseExpressionResponse resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/synchronization-parseexpressionresponse.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
