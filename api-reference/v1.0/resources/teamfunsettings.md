---
title: teamFunSettings リソースの種類
description: チームでの Giphy、ミーム、およびステッカーの使用を構成する設定。
localization_priority: Normal
author: nkramer
ms.prod: microsoft-teams
ms.openlocfilehash: c701ffe76c82a6cb4b3586272926290f634a02d9
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32548517"
---
# <a name="teamfunsettings-resource-type"></a>teamFunSettings リソースの種類

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

[チーム](team.md)での giphy、memes、ステッカーの使用を構成するための設定。

## <a name="properties"></a>プロパティ
| プロパティ     | 型   |説明|
|:---------------|:--------|:----------|
|allowgiphy|ブール値|true に設定すると、giphy の使用が有効になります。|
|giphyContentRating|String (enum)|giphy コンテンツの評価。 可能な値は、`moderate`、`strict` です。|
|allowStickersAndMemes|ブール値|true に設定すると、ユーザーはステッカーと memes を含めることができます。|
|allowcustommemes|ブール値|true に設定すると、ユーザーはカスタム memes 含めることができます。|

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
  "suppressions": [
    "Error: /api-reference/beta/resources/teamfunsettings.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
