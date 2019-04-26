---
title: mediaConfig リソースの種類
description: 通話への接続に使用されるメディア構成。
author: VinodRavichandran
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: aa8ec08ce5f4092a8f3d8c89af4a405d3a5c347d
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/26/2019
ms.locfileid: "33342661"
---
# <a name="mediaconfig-resource-type"></a>mediaConfig リソースの種類

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

通話への接続に使用されるメディア構成。

## <a name="properties"></a>プロパティ

| プロパティ       | 型    | 説明|
|:---------------|:--------|:----------|
| removefromdefaultaudiogroup | Boolean |  |

## <a name="json-representation"></a>JSON 表記

リソースの JSON 表記を次に示します。

<!-- {
  "blockType": "resource",
  "optionalProperties": [
    "removeFromDefaultAudioGroup"
   ],
  "abstract": true,
  "@odata.type": "microsoft.graph.mediaConfig"
}-->
```json
{
  "removeFromDefaultAudioGroup": true
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "mediaConfig resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
