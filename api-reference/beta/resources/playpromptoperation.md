---
title: playPromptOperation リソースの種類
description: PlayPrompt アクションの結果を取得する playPrompt の操作です。
author: VinodRavichandran
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: d451418482d1adf1a4b7e16dc8a6eb8ca7febdb7
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/12/2019
ms.locfileid: "27937818"
---
# <a name="playpromptoperation-resource-type"></a>playPromptOperation リソースの種類

> **重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。 実稼働アプリケーションでの、これらの API の使用はサポートされていません。

PlayPrompt アクションの結果を取得する playPrompt の操作です。

## <a name="properties"></a>プロパティ

| プロパティ            | 種類                        | 説明|
|:--------------------|:----------------------------|:-----------------------------------------------------------------------------------|
| clientContext       | String                      | クライアントのコンテキスト。                                                                |
| completionReason    | String                      | 可能な値は、`unknown`、`completedSuccessfully`、`mediaOperationCanceled` です。 |
| createdDateTime     | DateTimeOffset              | 操作の開始時刻です。                                                   |
| id                  | String                      | 読み取り専用です。                                                                         |
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
<!-- {
  "type": "#page.annotation",
  "description": "playPromptOperation resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
