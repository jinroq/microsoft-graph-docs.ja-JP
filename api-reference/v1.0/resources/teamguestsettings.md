---
title: teamGuestSettings リソースの種類
description: 来園者が作成、更新、またはチーム内のチャンネルを削除するかどうかを構成するのに設定します。
ms.openlocfilehash: 3c59c84e0baa9db580a81eeb72a405ec5097c478
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27022869"
---
# <a name="teamguestsettings-resource-type"></a>teamGuestSettings リソースの種類



来園者が作成、更新、または[チーム](team.md)内のチャンネルを削除するかどうかを構成するのに設定します。

## <a name="properties"></a>プロパティ
| プロパティ     | 型   |説明|
|:---------------|:--------|:----------|
|allowCreateUpdateChannels|ブール値|True の場合、来園者のセットを追加したりチャンネルを更新する場合。|
|allowDeleteChannels|ブール値|場合は true を指定すると、来園者に設定するには、チャンネルを削除できます。|

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
