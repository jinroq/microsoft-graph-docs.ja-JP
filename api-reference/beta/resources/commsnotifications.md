---
title: commsnotifications リソースの種類
description: 複数の通知を1つのバッチで送信するために通信サーバーによって使用される通知の一覧。
author: VinodRavichandran
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: 4497e2e1ba28e7f2d0b203f8f982053c5eb8ae1f
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/26/2019
ms.locfileid: "33341469"
---
# <a name="commsnotifications-resource-type"></a>commsnotifications リソースの種類

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

複数の通知を1つのバッチで送信するために通信サーバーによって使用される通知の一覧。

## <a name="properties"></a>プロパティ

| プロパティ       | 型                                                 | 説明                                   |
|:---------------|:-----------------------------------------------------|:----------------------------------------------|
| value          | [commsnotification](commsnotification.md)コレクション | リソースの変更の通知。 |

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
<!--
{
  "type": "#page.annotation",
  "description": "commsNotifications resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
