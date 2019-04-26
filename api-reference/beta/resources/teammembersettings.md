---
title: teammembersettings リソースの種類
description: メンバーが特定のアクション (チャネルの作成、ボットの追加など) をチーム内で実行できるかどうかを構成する設定。
localization_priority: Normal
author: nkramer
ms.prod: microsoft-teams
ms.openlocfilehash: 33f1930096ff63968db39e06ddec26c53ae8bcc9
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/26/2019
ms.locfileid: "33341723"
---
# <a name="teammembersettings-resource-type"></a>teammembersettings リソースの種類

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

[チーム](team.md)内で、メンバーが特定のアクション (チャネルの作成、ボットの追加など) を実行できるかどうかを構成するための設定。

## <a name="properties"></a>プロパティ
| プロパティ     | 型   |説明|
|:---------------|:--------|:----------|
|allowCreateUpdateChannels|Boolean|true に設定されている場合、メンバーはチャネルを追加および更新できます。|
|allowDeleteChannels|Boolean|true に設定されている場合、メンバーはチャネルを削除できます。|
|allowaddremoveapps|Boolean|true に設定すると、メンバーはアプリを追加および削除できるようになります。|
|allowCreateUpdateRemoveTabs|Boolean|true に設定されている場合、メンバーはタブの追加、更新、および削除を行うことができます。 |
|allowCreateUpdateRemoveConnectors|Boolean|true に設定されている場合、メンバーはコネクタの追加、更新、および削除を行うことができます。|

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
