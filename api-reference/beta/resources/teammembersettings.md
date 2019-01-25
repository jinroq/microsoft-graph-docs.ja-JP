---
title: teamMemberSettings リソースの種類
description: など、メンバーが特定のアクションを実行するかどうかを構成する設定は、チャネルを作成し、チームにボットを追加します。
localization_priority: Normal
author: nkramer
ms.prod: microsoft-teams
ms.openlocfilehash: e6fae4d81ac005c1830d5bed9e05a4675e1a8ad0
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/24/2019
ms.locfileid: "29522645"
---
# <a name="teammembersettings-resource-type"></a>teamMemberSettings リソースの種類

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

など、メンバーが特定のアクションを実行するかどうかを構成する設定は、チャネルを作成し、[チーム](team.md)にボットを追加します。

## <a name="properties"></a>プロパティ
| プロパティ     | 型   |説明|
|:---------------|:--------|:----------|
|allowCreateUpdateChannels|ブール値|True の場合、メンバー セットを追加したりチャンネルを更新する場合。|
|allowDeleteChannels|ブール値|場合は true の場合、メンバーに設定するには、チャンネルを削除できます。|
|allowAddRemoveApps|ブール値|場合は true の場合、メンバー セットは、追加し、アプリケーションを削除できます。|
|allowCreateUpdateRemoveTabs|ブール値|場合は true の場合、メンバー セットを追加、更新、およびタブを削除します。 |
|allowCreateUpdateRemoveConnectors|ブール値|場合は true の場合、メンバー セットを追加、更新、およびコネクタを削除します。|

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
  "suppressions": [
    "Error: /api-reference/beta/resources/teammembersettings.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
