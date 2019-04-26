---
title: teamFunSettings リソースの種類
description: チームでの Giphy、ミーム、およびステッカーの使用を構成する設定。
localization_priority: Normal
author: nkramer
ms.prod: microsoft-teams
ms.openlocfilehash: 0f96157072ac7b6de403f82822226f316c8dcd46
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/26/2019
ms.locfileid: "33341709"
---
# <a name="teamfunsettings-resource-type"></a>teamFunSettings リソースの種類

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

[チーム](team.md)での giphy、memes、ステッカーの使用を構成するための設定。

## <a name="properties"></a>プロパティ
| プロパティ     | 型   |説明|
|:---------------|:--------|:----------|
|allowgiphy|Boolean|true に設定すると、giphy の使用が有効になります。|
|giphyContentRating|String (enum)|giphy コンテンツの評価。 可能な値は、`moderate`、`strict` です。|
|allowStickersAndMemes|Boolean|true に設定すると、ユーザーはステッカーと memes を含めることができます。|
|allowcustommemes|Boolean|true に設定すると、ユーザーはカスタム memes 含めることができます。|

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
<!--
{
  "type": "#page.annotation",
  "description": "team's funSettings resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
