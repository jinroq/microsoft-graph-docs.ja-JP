---
title: commsNotifications リソースの種類
description: 通信サーバーによって 1 つのバッチで複数の通知を送信するための通知の一覧です。
author: VinodRavichandran
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: 83a89e848d0992d253efb532ed078031b6f965d2
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/12/2019
ms.locfileid: "27946302"
---
# <a name="commsnotifications-resource-type"></a>commsNotifications リソースの種類

> **重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。 実稼働アプリケーションでの、これらの API の使用はサポートされていません。

通信サーバーによって 1 つのバッチで複数の通知を送信するための通知の一覧です。

## <a name="properties"></a>プロパティ

| プロパティ       | 種類                                                 | 説明                                   |
|:---------------|:-----------------------------------------------------|:----------------------------------------------|
| value          | [commsNotification](commsnotification.md)コレクション | リソースに変更を通知します。 |

## <a name="json-representation"></a>JSON 表記

リソースの JSON 表記を次に示します。

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.commsNotifications"
}-->
```json
{
  "value": [ { "@odata.type": "#microsoft.graph.commsNotification" } ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "commsNotifications resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
