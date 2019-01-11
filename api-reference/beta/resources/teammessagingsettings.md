---
title: teamMessagingSettings リソースの種類
description: メッセージングを構成する設定は、チーム内の参照。
author: nkramer
localization_priority: Normal
ms.openlocfilehash: 06aca84355a07052dcea316145dfff437eee743b
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/11/2019
ms.locfileid: "27848259"
---
# <a name="teammessagingsettings-resource-type"></a>teamMessagingSettings リソースの種類

> **重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。 実稼働アプリケーションでの、これらの API の使用はサポートされていません。

メッセージングを構成する設定は、[チーム](team.md)内の参照。

## <a name="properties"></a>プロパティ
| プロパティ     | 種類   |説明|
|:---------------|:--------|:----------|
|allowUserEditMessages|ブール型|場合 true の場合、ユーザーに設定するには、自分のメッセージを編集できます。|
|allowUserDeleteMessages|ブール型|場合は true の場合、ユーザーに設定するには、そのメッセージを削除できます。|
|allowOwnerDeleteMessages|ブール型|場合は true の場合、所有者に設定するには、任意のメッセージを削除できます。|
|allowTeamMentions|ブール型|場合、参照投稿を許可する @team を true に設定します。|
|allowChannelMentions|ブール型|場合、参照投稿を許可する @channel を true に設定します。|

## <a name="json-representation"></a>JSON 表記

リソースの JSON 表記を次に示します。

<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.teamMessagingSettings"
}-->

```json
{
  "allowUserEditMessages": true,
  "allowUserDeleteMessages": true,
  "allowOwnerDeleteMessages": true,
  "allowTeamMentions": true,
  "allowChannelMentions": true    
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "team's messagingSettings resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
