---
title: clonableTeamParts 列挙型
description: 'チームのどの部分のクローンを作成する必要があるについて説明します。 '
localization_priority: Normal
ms.openlocfilehash: 3169d6e367484248e581c12c38887e07cf5c95af
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/24/2019
ms.locfileid: "29511465"
---
# <a name="clonableteamparts-enum-type"></a>clonableTeamParts 列挙型

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

[チーム](../resources/team.md)のどの部分のクローンを作成する必要があるについて説明します。 

## <a name="members"></a>メンバー

| メンバー | 値| 説明 |
|:---------------|:--------|:----------|
|apps|-1|インストールされたアプリの一覧をコピーします。|
|タブ|-2|チャネル内のタブにコピーします。|
|設定|-4|キーのグループの設定と、チーム内のすべての設定をコピーします。|
|チャンネル|-8|チャネルの構造 (ただし、チャネル内のメッセージではない) をコピーします。|
|members|1.6|メンバーとチームの所有者にコピーします。|
<!--
{
  "type": "#page.annotation",
  "suppressions": [
    "Error: /api-reference/beta/resources/clonableteamparts.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
