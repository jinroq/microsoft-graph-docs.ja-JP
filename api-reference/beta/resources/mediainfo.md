---
title: mediaInfo リソースの種類
description: プロンプトのアクションで使用されるメディア情報。
author: VinodRavichandran
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: 4c6f8e4f4ceea184f9663c433672d0892ed92467
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/26/2019
ms.locfileid: "33342644"
---
# <a name="mediainfo-resource-type"></a>mediaInfo リソースの種類

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

プロンプトのアクションで使用されるメディア情報。

## <a name="properties"></a>プロパティ
| プロパティ       | 型    | 説明                      |
|:---------------|:--------|:---------------------------------|
| resourceId     | String  | リソースの一意の id です。 |
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
<!--
{
  "type": "#page.annotation",
  "description": "mediaInfo resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
