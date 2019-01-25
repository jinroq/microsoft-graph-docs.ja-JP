---
title: playPromptOperation リソースの種類
description: PlayPrompt アクションの結果を取得する playPrompt の操作です。
author: VinodRavichandran
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: a6ecdb06c910923d35f9d36590ad09fd7835fccb
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/24/2019
ms.locfileid: "29515203"
---
# <a name="playpromptoperation-resource-type"></a>playPromptOperation リソースの種類

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

PlayPrompt アクションの結果を取得する playPrompt の操作です。

## <a name="properties"></a>プロパティ

| プロパティ            | 型                        | 説明|
|:--------------------|:----------------------------|:-----------------------------------------------------------------------------------|
| ClientContext       | String                      | クライアントのコンテキスト。                                                                |
| completionReason    | String                      | 可能な値は、`unknown`、`completedSuccessfully`、`mediaOperationCanceled` です。 |
| createdDateTime     | DateTimeOffset              | 操作の開始時刻です。                                                   |
| id                  | 文字列                      | 読み取り専用です。                                                                         |
| lastActionDateTime  | DateTimeOffset              | 操作の最後の操作の時間です。                                      |
| resultInfo          | [resultInfo](resultInfo.md) | 結果の情報です。 読み取り専用です。 サーバーを生成します。                               |
| status              | String                      | 可能な値は、`notStarted`、`running`、`completed`、`failed` です。               |

## <a name="relationships"></a>関係
なし

## <a name="json-representation"></a>JSON 表記

リソースの JSON 表記を次に示します。

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.playPromptOperation"
}-->
```json
{
  "clientContext": "String",
  "completionReason": "unknown | completedSuccessfully | mediaOperationCanceled",
  "createdDateTime": "String (timestamp)",
  "id": "String (identifier)",
  "lastActionDateTime": "String (timestamp)",
  "resultInfo": {"@odata.type": "#microsoft.graph.resultInfo"},
  "status": "notStarted | running | completed | failed"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "playPromptOperation resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/playpromptoperation.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
