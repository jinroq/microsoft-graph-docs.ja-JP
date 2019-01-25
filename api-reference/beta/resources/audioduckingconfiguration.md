---
title: audioDuckingConfiguration リソースの種類
description: ダック (その他のソースとの間でフェードアウト) の他のソースのためのパラメーター
author: VinodRavichandran
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: d61e4150250df25e020f45a65676d1c55c0e4c9d
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/24/2019
ms.locfileid: "29522463"
---
# <a name="audioduckingconfiguration-resource-type"></a>audioDuckingConfiguration リソースの種類

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

ダック (その他のソースとの間でフェードアウト) の他のソースのためのパラメーター

## <a name="properties"></a>プロパティ

| プロパティ      | 型     | 説明                                                                     |
| :------------ | :------- | :-------------------------------------------------------------------------------|
| lowerLevel    | Int64    | % のソースを ducked されているときに元のボリューム。             |
| rampActive    | Int64    | Ducked ソースの「フェードアウト」にかかる時間 (ミリ秒単位) の量。 |
| rampInactive  | Int64    | Ducked ソースの「フェードイン」にかかる時間 (ミリ秒単位) の量。  |
| upperLevel    | Int64    | % のソースは ducked されていないときに元のボリューム。         |

> **注:** ランプの期間は、5,000 人以上のミリ秒になることはできません。

## <a name="json-representation"></a>JSON 表記

リソースの JSON 表記を次に示します。

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.audioDuckingConfiguration"
}-->
```json
{
  "lowerLevel": 20,
  "rampActive": 1000,
  "rampInactive": 1000,
  "upperLevel": 100
}
```
<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "audioDuckingConfiguration resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/audioduckingconfiguration.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
