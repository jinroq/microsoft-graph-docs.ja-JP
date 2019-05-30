---
title: playPromptOperation リソースの種類
description: Playprompt アクションの結果を取得する playPrompt 操作。
author: VinodRavichandran
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: 663675bb895d452c9ad50c89f22f1a51efca20a9
ms.sourcegitcommit: c0df90d66cb2072848d4bb0bf730c47a601b99ce
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/29/2019
ms.locfileid: "34536996"
---
# <a name="playpromptoperation-resource-type"></a>playPromptOperation リソースの種類

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Playprompt アクションの結果を取得する playPrompt 操作。

## <a name="properties"></a>プロパティ

| プロパティ            | 型                        | 説明|
|:--------------------|:----------------------------|:-----------------------------------------------------------------------------------|
| clientContext       | String                      | クライアントコンテキスト。                                                                |
| 「補完の理由」    | String                      | 可能な値は、`unknown`、`completedSuccessfully`、`mediaOperationCanceled` です。 |
| createdDateTime     | DateTimeOffset              | 操作の開始時刻。                                                   |
| id                  | 文字列                      | 読み取り専用です。                                                                         |
| lastActionDateTime  | DateTimeOffset              | 操作の最後の操作の時刻。                                      |
| resultInfo          | [resultInfo](resultinfo.md) | 結果の情報。 読み取り専用です。 サーバーによって生成されます。                               |
| status              | String                      | 使用可能な値: `notStarted`、`running`、`completed`、`failed`。               |

## <a name="relationships"></a>リレーションシップ
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
  "suppressions": []
}
-->
