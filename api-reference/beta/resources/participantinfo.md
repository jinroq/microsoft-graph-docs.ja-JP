---
title: participantInfo リソースの種類
description: 参加者のアイデンティティについての追加のプロパティが含まれています
author: VinodRavichandran
localization_priority: Normal
ms.openlocfilehash: 94bbc587f26f8b5122571899eb235d9c1fc27e90
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/11/2019
ms.locfileid: "27870666"
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
