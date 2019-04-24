---
title: chatinfo リソースの種類
description: Microsoft Teams のメッセージに関する情報。
author: VinodRavichandran
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: 3c1414d10a262280bcf0d3a307fc0c71aed2fbde
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32461074"
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
  "suppressions": [
    "Error: /api-reference/beta/resources/chatInfo.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
