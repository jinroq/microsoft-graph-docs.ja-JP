---
title: participantInfo リソースの種類
description: 参加者のアイデンティティについての追加のプロパティが含まれています
author: VinodRavichandran
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: 7860c80da8e0f56ca425cffe8876d6003fba1d0d
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/12/2019
ms.locfileid: "27991413"
---
# <a name="participantinfo-resource-type"></a>participantInfo リソースの種類

> **重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。 実稼働アプリケーションでの、これらの API の使用はサポートされていません。

参加者のアイデンティティについての追加のプロパティが含まれています

## <a name="properties"></a>プロパティ

| プロパティ       | 種類                          | 説明  |
|:---------------|:------------------------------|:-------------|
| identity       | [identitySet](identityset.md) | この構成要素に関連付けられている[identitySet](identityset.md) 。 |
| languageId     | String                        | 言語カルチャの文字列です。 |
| 地域         | String                        | 参加者の領域です。 |

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
<!-- {
  "type": "#page.annotation",
  "description": "participantInfo resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
