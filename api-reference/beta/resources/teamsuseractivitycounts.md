---
title: teamsUserActivityCounts リソースの種類
description: リソースの JSON 表記を次に示します。
author: nkramer
ms.openlocfilehash: f67540f4172993b1076d9590438262b0d4da1846
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 12/18/2018
ms.locfileid: "27334518"
---
# <a name="teamsuseractivitycounts-resource-type"></a>teamsUserActivityCounts リソースの種類

## <a name="properties"></a>Properties

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
