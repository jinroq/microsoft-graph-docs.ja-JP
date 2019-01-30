---
title: appHostedMediaConfig リソースの種類
description: メディア スタックは、アプリケーションによってホストされています。
author: VinodRavichandran
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: a2e52c1c4d48649c5763be643f8b2ededb71bce5
ms.sourcegitcommit: d95f6d39a0479da6e531f3734c4029dc596b9a3f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/30/2019
ms.locfileid: "29643693"
---
# <a name="apphostedmediaconfig-resource-type"></a>appHostedMediaConfig リソースの種類

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

メディア スタックは、アプリケーションによってホストされています。

## <a name="properties"></a>プロパティ

| プロパティ                          | 型    | 説明                                                     |
| :-------------------------------- | :------ | :---------------------------------------------------------------|
| blob                              | String  | スマート メディア エージェントによって生成されたメディア構成の blob です。    |
| removeFromDefaultAudioGroup       | Boolean | オーディオの既定のグループからのオーディオを削除します。                       |

## <a name="json-representation"></a>JSON 表記

リソースの JSON 表記を次に示します。

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.appHostedMediaConfig"
}-->
```json
{
  "blob": "String",
  "removeFromDefaultAudioGroup": true
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "appHostedMediaConfig resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/apphostedmediaconfig.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
