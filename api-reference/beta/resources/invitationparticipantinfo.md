---
title: invitationParticipantInfo リソースの種類
description: '**InvitationParticipant**は、会話出席依頼に関連付けられている id のセットを表すために使用され、追加の招待パラメーターを提供します。'
author: VinodRavichandran
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: 56eb1ad90410edca795a8e29ecaa4b8b94e915ee
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/26/2019
ms.locfileid: "33345442"
---
# <a name="invitationparticipantinfo-resource-type"></a>invitationParticipantInfo リソースの種類

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

**InvitationParticipant**は、会話出席依頼に関連付けられている id のセットを表すために使用され、追加の招待パラメーターを提供します。

## <a name="properties"></a>プロパティ

| プロパティ                           | 型                          | 説明                                                                          |
| :--------------------------------- | :---------------------------- | :----------------------------------------------------------------------------------- |
| endpointtype                       | String                        | 使用可能な値は、`default`、`voicemail` です。 |
| 独自性                           | [identitySet](identityset.md) | この招待に関連付けられている id[セット](identityset.md)。                   |
| languageId                         | String                        | 言語のカルチャ文字列。                                                                                     |
| エリア                             | String                        | 参加者の地域。                                                           |
| replacesCallId                     | 文字列                        | 省略可能。 ターゲット id が現在一部である通話。 この呼び出しは、参加者が追加されると削除されます。 |

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
  "suppressions": []
}
-->
