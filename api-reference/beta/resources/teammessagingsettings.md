---
title: teammessagingsettings リソースの種類
description: チームでメッセージとメンションを構成する設定。
author: nkramer
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: d98dfa3c2306cabb99b6de96aed2010cefa10717
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32553949"
---
# <a name="teammessagingsettings-resource-type"></a>teammessagingsettings リソースの種類



[チーム](team.md)内のメッセージとメンションを構成するための設定。

## <a name="properties"></a>プロパティ
| プロパティ     | 型   |説明|
|:---------------|:--------|:----------|
|allowusereditmessages|ブール値|true に設定されている場合、ユーザーは自分のメッセージを編集できます。|
|allowUserDeleteMessages|ブール値|true に設定されている場合、ユーザーは自分のメッセージを削除できます。|
|allowOwnerDeleteMessages|ブール値|true に設定されている場合、所有者は任意のメッセージを削除できます。|
|allowteammentions ション|ブール値|true に設定すると @team メンションが許可されます。|
|allowchannelmentions ション|ブール値|true に設定すると @channel メンションが許可されます。|

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
