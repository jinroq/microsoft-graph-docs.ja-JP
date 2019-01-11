---
title: teamMemberSettings リソースの種類
description: など、メンバーが特定のアクションを実行するかどうかを構成する設定は、チャネルを作成し、チームにボットを追加します。
localization_priority: Normal
ms.openlocfilehash: 7b63bce5bc298f7d9599d8c6146d7962d319c79f
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/11/2019
ms.locfileid: "27826069"
---
# <a name="teammembersettings-resource-type"></a>teamMemberSettings リソースの種類



など、メンバーが特定のアクションを実行するかどうかを構成する設定は、チャネルを作成し、[チーム](team.md)にボットを追加します。

## <a name="properties"></a>プロパティ
| プロパティ     | 種類   |説明|
|:---------------|:--------|:----------|
|allowCreateUpdateChannels|ブール型|True の場合、メンバー セットを追加したりチャンネルを更新する場合。|
|allowDeleteChannels|ブール型|場合は true の場合、メンバーに設定するには、チャンネルを削除できます。|
|allowAddRemoveApps|ブール型|場合は true の場合、メンバー セットは、追加し、アプリケーションを削除できます。|
|allowCreateUpdateRemoveTabs|ブール型|場合は true の場合、メンバー セットを追加、更新、およびタブを削除します。 |
|allowCreateUpdateRemoveConnectors|ブール型|場合は true の場合、メンバー セットを追加、更新、およびコネクタを削除します。|

## <a name="json-representation"></a>JSON 表記

リソースの JSON 表記を次に示します。

<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.teamMemberSettings"
}-->

```json
{
  "allowCreateUpdateChannels": true,
  "allowDeleteChannels": true,
  "allowAddRemoveApps": true,
  "allowCreateUpdateRemoveTabs": true,
  "allowCreateUpdateRemoveConnectors": true
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "team's memberSettings resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
