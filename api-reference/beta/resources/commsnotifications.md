---
title: 通知リソースの種類
description: リソースの JSON 表記を次に示します。
ms.openlocfilehash: 96246491c386971fe18184f26269d4abe3af6e6e
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27074166"
---
# <a name="notifications-resource-type"></a>通知リソースの種類

> **重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。 実稼働アプリケーションでの、これらの API の使用はサポートされていません。

## <a name="properties"></a>プロパティ

| プロパティ       | 型                                       | 説明 |
|:---------------|:-------------------------------------------|:------------|
| value          | [通知](commsnotification.md)のコレクション | リソースに変更を通知します。 |

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
  "description": "notifications resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->