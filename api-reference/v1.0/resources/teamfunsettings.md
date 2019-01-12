---
title: teamFunSettings リソースの種類
description: Giphy、memes、およびチームのステッカーを構成する設定を使用します。
localization_priority: Normal
author: nkramer
ms.prod: microsoft-teams
ms.openlocfilehash: c701ffe76c82a6cb4b3586272926290f634a02d9
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/12/2019
ms.locfileid: "27987672"
---
# <a name="teamfunsettings-resource-type"></a>teamFunSettings リソースの種類



Giphy、memes、および[チーム](team.md)のステッカーを構成する設定を使用します。

## <a name="properties"></a>プロパティ
| プロパティ     | 種類   |説明|
|:---------------|:--------|:----------|
|allowGiphy|ブール型|場合 true の場合、有効にする Giphy の使用を設定します。|
|giphyContentRating|文字列 (列挙型)|コンテンツの規制を Giphy。 使用可能な値は、`moderate`、`strict` です。|
|allowStickersAndMemes|ブール型|場合は true、ステッカー、memes など、ユーザーに設定します。|
|allowCustomMemes|ブール型|場合に true を設定する、カスタムの memes を含むようにユーザーをできるようにする設定です。|

## <a name="json-representation"></a>JSON 表記

リソースの JSON 表記を次に示します。

<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.teamFunSettings"
}-->

```json
{
  "allowGiphy": true,
  "giphyContentRating": "strict",
  "allowStickersAndMemes": true,
  "allowCustomMemes": true
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "team's funSettings resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
