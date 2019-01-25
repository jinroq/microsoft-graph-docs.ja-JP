---
title: teamsAsyncOperationType 列挙型
description: TeamsAsyncOperation のタイプです。 追加するメンバーがここでより多くの非同期操作はサポートされています。
author: nkramer
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: 4de95db194bf41939521b53f06614b46b6afae99
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/24/2019
ms.locfileid: "29516568"
---
# <a name="teamsasyncoperationtype-enum-type"></a>teamsAsyncOperationType 列挙型

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

[TeamsAsyncOperation](teamsasyncoperation.md)のタイプです。 追加するメンバーがここでより多くの非同期操作はサポートされています。

## <a name="members"></a>メンバー

| メンバー | 値| 説明 |
|:---------------|:--------|:----------|
|Invalid|(0)|無効な値|
|cloneTeam|-1|チームのクローンを作成する操作です。|
|archiveTeam|-2|チームをアーカイブする操作です。|
|unarchiveTeam|-3|アーカイブされたチームを復元する操作です。|
|createTeam|-3|最初からチームを作成する操作です。|

<!--
{
  "type": "#page.annotation",
  "suppressions": [
    "Error: /api-reference/beta/resources/teamsasyncoperationtype.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
