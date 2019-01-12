---
title: teamGuestSettings リソースの種類
description: 来園者が作成、更新、またはチーム内のチャンネルを削除するかどうかを構成するのに設定します。
localization_priority: Normal
author: nkramer
ms.prod: microsoft-teams
ms.openlocfilehash: cb6e83093945a96784bfb91a76bc343a8c13d0ac
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/12/2019
ms.locfileid: "27924371"
---
# <a name="teamguestsettings-resource-type"></a>teamGuestSettings リソースの種類



来園者が作成、更新、または[チーム](team.md)内のチャンネルを削除するかどうかを構成するのに設定します。

## <a name="properties"></a>プロパティ
| プロパティ     | 種類   |説明|
|:---------------|:--------|:----------|
|allowCreateUpdateChannels|ブール型|True の場合、来園者のセットを追加したりチャンネルを更新する場合。|
|allowDeleteChannels|ブール型|場合は true を指定すると、来園者に設定するには、チャンネルを削除できます。|

## <a name="json-representation"></a>JSON 表記

リソースの JSON 表記を次に示します。

<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.teamGuestSettings"
}-->

```json
{
  "allowCreateUpdateChannels": true,
  "allowDeleteChannels": true
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "team's guestSettings resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
