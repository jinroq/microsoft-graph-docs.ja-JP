---
title: teamMemberSettings リソースの種類
description: メンバーが特定のアクション (チャネルの作成、ボットの追加など) をチーム内で実行できるかどうかを構成する設定。
localization_priority: Normal
author: nkramer
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: c7c6690eb293581a60cba20d3f3ef63187339c35
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "36007698"
---
# <a name="teammembersettings-resource-type"></a>teamMemberSettings リソースの種類

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

[チーム](team.md)内で、メンバーが特定のアクション (チャネルの作成、ボットの追加など) を実行できるかどうかを構成するための設定。

## <a name="properties"></a>プロパティ
| プロパティ     | 型   |説明|
|:---------------|:--------|:----------|
|allowCreateUpdateChannels|Boolean|True に設定されている場合、メンバーはチャネルを追加および更新できます。|
|allowDeleteChannels|Boolean|True に設定されている場合、メンバーはチャネルを削除できます。|
|allowAddRemoveApps|Boolean|True に設定すると、メンバーはアプリを追加および削除できるようになります。|
|allowCreateUpdateRemoveTabs|Boolean|True に設定されている場合、メンバーはタブの追加、更新、および削除を行うことができます。 |
|allowCreateUpdateRemoveConnectors|Boolean|True に設定されている場合、メンバーはコネクタの追加、更新、および削除を行うことができます。|

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
<!--
{
  "type": "#page.annotation",
  "description": "team's memberSettings resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
