---
title: mediaInfo リソースの種類
description: アクションで使用されるメディアの情報には次のメッセージが表示されます。
author: VinodRavichandran
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: 217b9a5aaa88a1bbf343447fad344b322cfeb611
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/12/2019
ms.locfileid: "27924532"
---
# <a name="mediainfo-resource-type"></a>mediaInfo リソースの種類

> **重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。 実稼働アプリケーションでの、これらの API の使用はサポートされていません。

アクションで使用されるメディアの情報には次のメッセージが表示されます。

## <a name="properties"></a>プロパティ
| プロパティ       | 種類    | 説明                      |
|:---------------|:--------|:---------------------------------|
| resourceId     | 文字列型 (String)  | リソースの一意の id。 |
| uri            | String  | リソースへのパス。            |

## <a name="json-representation"></a>JSON 表記

リソースの JSON 表記を次に示します。

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.mediaInfo"
}-->
```json
{
  "resourceId": "String",
  "uri": "String"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "mediaInfo resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
