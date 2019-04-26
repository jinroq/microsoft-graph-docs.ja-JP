---
title: participantInfo リソースの種類
description: 参加者の id に関する追加のプロパティが含まれています
author: VinodRavichandran
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: 3d040fd5be86068c30e7a63dae50888c4f3ec756
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32568595"
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
