---
title: teamsUserActivityCounts リソースの種類
description: リソースの JSON 表記を次に示します。
ms.openlocfilehash: 39e90b4c9dc6b9929959139ba67ddb090d143e38
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27073133"
---
# <a name="teamsuseractivitycounts-resource-type"></a>teamsUserActivityCounts リソースの種類

## <a name="properties"></a>プロパティ

| プロパティ            | 型   |
| :------------------ | :----- |
| reportRefreshDate   | Date   |
| reportDate          | Date   |
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
