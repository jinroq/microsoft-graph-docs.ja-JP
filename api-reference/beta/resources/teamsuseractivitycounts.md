---
title: teamsUserActivityCounts リソースの種類
description: リソースの JSON 表記を次に示します。
author: nkramer
localization_priority: Normal
ms.openlocfilehash: c7351795f6b3dafbac996844fc1ac11cd24bbc03
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/11/2019
ms.locfileid: "27886591"
---
# <a name="teamsuseractivitycounts-resource-type"></a>teamsUserActivityCounts リソースの種類

## <a name="properties"></a>プロパティ

| プロパティ            | 種類   |
| :------------------ | :----- |
| reportRefreshDate   | 日付   |
| reportDate          | 日付   |
| teamChatMessages    | Int64  |
| privateChatMessages | Int64  |
| 呼び出し               | Int64  |
| 会議            | Int64  |
| reportPeriod        | String |


## <a name="json-representation"></a>JSON 表記

リソースの JSON 表記を次に示します。

<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.teamsUserActivityCounts"
} -->

```json
{
  "reportRefreshDate": "Date", 
  "reportDate": "Date", 
  "teamChatMessages": 1024, 
  "privateChatMessages": 1024, 
  "calls": 1024, 
  "meetings": 1024, 
  "reportPeriod": "String"
}
```
