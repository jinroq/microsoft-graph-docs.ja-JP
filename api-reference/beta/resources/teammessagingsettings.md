---
title: teamMessagingSettings リソースの種類
description: チームでメッセージとメンションを構成する設定。
author: nkramer
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: 3a89ed35c820338cde7b3f22a7345c860b1a4427
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "35964530"
---
# <a name="teammessagingsettings-resource-type"></a>teamMessagingSettings リソースの種類

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

[チーム](team.md)内のメッセージとメンションを構成するための設定。

## <a name="properties"></a>プロパティ
| プロパティ     | 型   |説明|
|:---------------|:--------|:----------|
|allowUserEditMessages|Boolean|True に設定されている場合、ユーザーは自分のメッセージを編集できます。|
|allowUserDeleteMessages|Boolean|True に設定されている場合、ユーザーは自分のメッセージを削除できます。|
|allowOwnerDeleteMessages|Boolean|True に設定されている場合、所有者は任意のメッセージを削除できます。|
|allowTeamMentions ション|Boolean|True に設定すると @team メンションが許可されます。|
|allowChannelMentions ション|Boolean|True に設定すると @channel メンションが許可されます。|

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
<!--
{
  "type": "#page.annotation",
  "description": "team's messagingSettings resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
