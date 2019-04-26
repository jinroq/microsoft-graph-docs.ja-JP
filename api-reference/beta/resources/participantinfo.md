---
title: participantInfo リソースの種類
description: 参加者の id に関する追加のプロパティが含まれています
author: VinodRavichandran
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: 9869cf1154735742630edf75ea3e4d5303d45bc9
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/26/2019
ms.locfileid: "33344919"
---
# <a name="participantinfo-resource-type"></a>participantInfo リソースの種類

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

参加者の id に関する追加のプロパティが含まれています

## <a name="properties"></a>プロパティ

| プロパティ       | 型                          | 説明  |
|:---------------|:------------------------------|:-------------|
| 独自性       | [identitySet](identityset.md) | この参加者に関連付けられている id[セット](identityset.md)。 |
| languageId     | String                        | 言語のカルチャ文字列。 |
| エリア         | String                        | 参加者の地域。 |

## <a name="json-representation"></a>JSON 表記

リソースの JSON 表記を次に示します。

<!-- {
  "blockType": "resource",
  "optionalProperties": [
    "languageId", "region"
  ],
  "@odata.type": "microsoft.graph.participantInfo"
}-->
```json
{
  "identity": { "@odata.type": "#microsoft.graph.identitySet" },
  "languageId": "String",
  "region": "String"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "participantInfo resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
