---
title: invitationParticipantInfo リソースの種類
description: '**InvitationParticipant**は、会話への招待に関連付けられている id のセットを表すために使用し、招待状の追加のパラメーターを提供します。'
ms.openlocfilehash: 8b00625dad1c41121b0359586742301e16d163fc
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27068847"
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
