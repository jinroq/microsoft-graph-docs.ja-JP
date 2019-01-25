---
title: Members
description: TeamsApp の現在のインストール状態を説明します。
author: nkramer
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: 82e46faccd2a91a82ba4fb7352391f58a42c33a9
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/24/2019
ms.locfileid: "29517275"
---
#<a name="teamsappinstalledstate-enum-type"></a>teamsAppInstalledState 列挙型

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

の[teamsApp](teamsapp.md)の現在のインストール状態を説明します。

## <a name="members"></a>メンバー

| メンバー | 値| 説明 |
|:---------------|:--------|:----------|
|notInstalled|(0)|チームには、アプリケーションはインストールされていません。|
|Installed|-1|アプリケーションが正常にインストールします。|
|installedAndHidden|-2|アプリケーションがインストールされているがビューから非表示にします。|
|installedAndPermanent|-3|アプリケーションが完全にインストールされているしは削除できません。|
<!--
{
  "type": "#page.annotation",
  "suppressions": [
    "Error: /api-reference/beta/resources/teamsappinstalledstate.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
