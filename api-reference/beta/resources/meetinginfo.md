---
title: 会議情報リソースの種類
description: 会議を作成または参加するために指定された会議情報。
author: VinodRavichandran
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: 3ad2ecbce32727cec26fbf0f9c72d3846e3792af
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/26/2019
ms.locfileid: "33342605"
---
# <a name="meetinginfo-resource-type"></a>会議情報リソースの種類

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

会議を作成または参加するために指定された会議情報。

## <a name="properties"></a>プロパティ

| プロパティ       | 型    | 説明|
|:---------------|:--------|:----------|
| allowConversationWithoutHost | Boolean |  |

## <a name="json-representation"></a>JSON 表記

リソースの JSON 表記を次に示します。

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.meetingInfo"
}-->
```json
{
  "allowConversationWithoutHost": true
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "meetingInfo resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
