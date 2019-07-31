---
title: noMediaConfig リソースの種類
description: メディアがないことを示すためのメディア構成。
author: VinodRavichandran
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: 97d2ac01b434e211eb8836f04343ef65b9f0ea1b
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "35966665"
---
# <a name="nomediaconfig-resource-type"></a>noMediaConfig リソースの種類

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

メディアがないことを示すためのメディア構成。

## <a name="properties"></a>プロパティ

| プロパティ       | 型    | 説明|
|:---------------|:--------|:----------|
| removeFromDefaultAudioGroup | Boolean |  |

## <a name="json-representation"></a>JSON 表記

リソースの JSON 表記を次に示します。

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "baseType": "microsoft.graph.mediaConfig",
  "@odata.type": "microsoft.graph.noMediaConfig"
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
  "description": "noMediaConfig resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
