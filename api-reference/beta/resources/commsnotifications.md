---
title: commsNotifications リソースの種類
description: 複数の通知を1つのバッチで送信するために通信サーバーによって使用される通知の一覧。
author: VinodRavichandran
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: 770122387b89e96fdd8dbd9077488a9956fd90f4
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "35973252"
---
# <a name="commsnotifications-resource-type"></a>commsNotifications リソースの種類

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

複数の通知を1つのバッチで送信するために通信サーバーによって使用される通知の一覧。

## <a name="properties"></a>プロパティ

| プロパティ       | 型                                                 | 説明                                   |
|:---------------|:-----------------------------------------------------|:----------------------------------------------|
| value          | [Commsnotification](commsnotification.md)コレクション | リソースの変更の通知。 |

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
