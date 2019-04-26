---
title: chatinfo リソースの種類
description: Microsoft Teams のメッセージに関する情報。
author: VinodRavichandran
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: 552844795d3ba7e8ad4c8a3c3a6dff3c18990bc2
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/26/2019
ms.locfileid: "33339696"
---
# <a name="chatinfo-resource-type"></a>chatinfo リソースの種類

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Microsoft Teams のメッセージに関する情報。

## <a name="properties"></a>プロパティ

| プロパティ            | 型    | 説明|
|:--------------------|:--------|:-----------|
| messageId           | String  | Microsoft Teams チャネル内のメッセージの一意識別子。 |
| replyChainMessageId | String  | 返信メッセージの ID。 |
| id            | String  | Microsoft Teams のスレッドの一意識別子。 |

## <a name="json-representation"></a>JSON 表記

リソースの JSON 表記を次に示します。

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.chatInfo"
}-->
```json
{
  "messageId": "String",
  "replyChainMessageId": "String",
  "threadId": "String"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "chatInfo resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
