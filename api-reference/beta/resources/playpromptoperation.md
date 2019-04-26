---
title: playPromptOperation リソースの種類
description: playprompt アクションの結果を取得する playprompt 操作。
author: VinodRavichandran
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: 89a47fc8400d2f0d426ef6f683eb566f9c2376d4
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/26/2019
ms.locfileid: "33344370"
---
# <a name="playpromptoperation-resource-type"></a>playPromptOperation リソースの種類

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

playprompt アクションの結果を取得する playprompt 操作。

## <a name="properties"></a>プロパティ

| プロパティ            | 型                        | 説明|
|:--------------------|:----------------------------|:-----------------------------------------------------------------------------------|
| clientContext       | String                      | クライアントコンテキスト。                                                                |
| 「補完の理由」    | String                      | 可能な値は、`unknown`、`completedSuccessfully`、`mediaOperationCanceled` です。 |
| createdDateTime     | DateTimeOffset              | 操作の開始時刻。                                                   |
| id                  | String                      | 読み取り専用です。                                                                         |
| lastactiondatetime  | DateTimeOffset              | 操作の最後の操作の時刻。                                      |
| resultInfo          | [resultInfo](resultInfo.md) | 結果の情報。 読み取り専用です。 サーバーによって生成されます。                               |
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
