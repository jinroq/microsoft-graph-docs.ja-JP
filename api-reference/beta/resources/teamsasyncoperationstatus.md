---
title: teamsAsyncOperationStatus 列挙型
description: TeamsAsyncOperation の現在の状態について説明します。
author: nkramer
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: e9138adcc646677955a12091a3fb15badfd39f13
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/24/2019
ms.locfileid: "29511710"
---
# <a name="teamsasyncoperationstatus-enum-type"></a>teamsAsyncOperationStatus 列挙型

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

の[teamsAsyncOperation](teamsasyncoperation.md)の現在の状態について説明します。

## <a name="members"></a>メンバー

| メンバー | 値| 説明 |
|:---------------|:--------|:----------|
|Invalid|(0)|無効な値|
|NotStarted|-1|操作は開始されていません。|
|InProgress|-2|操作が行われています。|
|Succeeded|-3|操作が正常に完了しました。|
|Failed|-4|処理に失敗しました。|
<!--
{
  "type": "#page.annotation",
  "suppressions": [
    "Error: /api-reference/beta/resources/teamsasyncoperationstatus.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
