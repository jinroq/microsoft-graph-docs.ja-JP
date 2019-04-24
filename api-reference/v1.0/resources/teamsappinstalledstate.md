---
title: メンバー
description: teamsapp の現在のインストール状態を示します。
author: nkramer
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: a58a0d046ef9c42f197e841ab542bf8dcb5f96f5
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32462250"
---
#<a name="teamsappinstalledstate-enum-type"></a>teamsAppInstalledState 列挙型

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

[teamsapp](teamsapp.md)の現在のインストール状態を示します。

## <a name="members"></a>メンバー

| メンバー | 値| 説明 |
|:---------------|:--------|:----------|
|notinstalled|.0|アプリが team にインストールされていません。|
|れる|1-d|アプリは正常にインストールされています。|
|windows、および非推奨|pbm-2|アプリはインストールされますが、ビューからは非表示になります。|
|windows viewer andパーマネント|1/3|アプリは完全にインストールされており、削除することはできません。|
<!--
{
  "type": "#page.annotation",
  "suppressions": [
    "Error: /api-reference/beta/resources/teamsappinstalledstate.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
