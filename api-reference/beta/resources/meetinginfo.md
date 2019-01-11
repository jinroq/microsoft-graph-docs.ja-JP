---
title: meetingInfo リソースの種類
description: 会議の情報を作成または、ミーティングに参加するために指定します。
author: VinodRavichandran
localization_priority: Normal
ms.openlocfilehash: 24ac0247fd39569276f2cb288646eca578447e07
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/11/2019
ms.locfileid: "27817753"
---
# <a name="meetinginfo-resource-type"></a>meetingInfo リソースの種類

> **重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。 実稼働アプリケーションでの、これらの API の使用はサポートされていません。

会議の情報を作成または、ミーティングに参加するために指定します。

## <a name="properties"></a>プロパティ

| プロパティ       | 種類    | 説明|
|:---------------|:--------|:----------|
| allowConversationWithoutHost | ブール型 |  |

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
<!-- {
  "type": "#page.annotation",
  "description": "meetingInfo resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
