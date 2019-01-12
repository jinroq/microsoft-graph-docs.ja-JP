---
title: invitationParticipantInfo リソースの種類
description: '**InvitationParticipant**は、会話への招待に関連付けられている id のセットを表すために使用し、招待状の追加のパラメーターを提供します。'
author: VinodRavichandran
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: 8febd66915ee0b4fba26d9253cd56d67086e63bc
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/12/2019
ms.locfileid: "27982898"
---
# <a name="invitationparticipantinfo-resource-type"></a>invitationParticipantInfo リソースの種類

> **重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。 実稼働アプリケーションでの、これらの API の使用はサポートされていません。

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
<!-- {
  "type": "#page.annotation",
  "description": "invitationParticipantInfo resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
