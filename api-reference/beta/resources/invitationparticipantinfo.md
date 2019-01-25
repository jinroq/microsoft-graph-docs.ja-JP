---
title: invitationParticipantInfo リソースの種類
description: '**InvitationParticipant**は、会話への招待に関連付けられている id のセットを表すために使用し、招待状の追加のパラメーターを提供します。'
author: VinodRavichandran
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: cb20dde1a74472695755e65dc404a6709f79c8b0
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/24/2019
ms.locfileid: "29520677"
---
# <a name="invitationparticipantinfo-resource-type"></a>invitationParticipantInfo リソースの種類

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

**InvitationParticipant**は、会話への招待に関連付けられている id のセットを表すために使用し、招待状の追加のパラメーターを提供します。

## <a name="properties"></a>プロパティ

| プロパティ                           | 型                          | 説明                                                                          |
| :--------------------------------- | :---------------------------- | :----------------------------------------------------------------------------------- |
| endpointType                       | String                        | 使用可能な値は、`default`、`voicemail` です。 |
| identity                           | [identitySet](identityset.md) | この招待状に関連付けられている[identitySet](identityset.md) 。                   |
| languageId                         | String                        | 言語カルチャの文字列です。                                                                                     |
| 地域                             | String                        | 参加者の領域です。                                                           |
| replacesCallId                     | String                        | 省略可能。 ターゲットの idenity がの一部である現在の呼び出しです。 参加者を追加するには、この呼び出しが削除されます。 |

## <a name="json-representation"></a>JSON 表記

リソースの JSON 表記を次に示します。

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.invitationParticipantInfo"
}-->
```json
{
  "endpointType": "default | voicemail",
  "identity": {"@odata.type": "#microsoft.graph.identitySet"},
  "languageId": "String",
  "region": "String",
  "replacesCallId": "String"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "invitationParticipantInfo resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/invitationparticipantinfo.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
