---
title: meetingParticipantInfo リソースの種類
description: 会議の参加者に関する情報。
author: VinodRavichandran
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: 62843378d53774d19ad3428e6b52c985761edda2
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "36009770"
---
# <a name="meetingparticipantinfo-resource-type"></a>meetingParticipantInfo リソースの種類

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

会議の参加者に関する情報。

## <a name="properties"></a>プロパティ

| プロパティ       | 型                          | 説明                              |
|:---------------|:------------------------------|:-----------------------------------------|
| 独自性       | [identitySet](identityset.md) | 参加者の id 情報。 |
| プリンシパル            | String                        | 参加者のユーザープリンシパル名。  |

## <a name="json-representation"></a>JSON 表記

リソースの JSON 表記を次に示します。

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.meetingParticipantInfo"
}-->
```json
{
  "identity": {"@odata.type": "#microsoft.graph.identitySet"},
  "upn": "String"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "meetingParticipantInfo resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
