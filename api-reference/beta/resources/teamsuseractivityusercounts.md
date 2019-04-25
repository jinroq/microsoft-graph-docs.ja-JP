---
title: teamsuseractivityusercounts リソースの種類
description: リソースの JSON 表記を次に示します。
author: nkramer
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: bcb69c09d621ce3cce006fd9130afa0a70e4cdb8
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32582914"
---
# <a name="teamsuseractivityusercounts-resource-type"></a>teamsuseractivityusercounts リソースの種類

## <a name="properties"></a>プロパティ

| プロパティ            | 型   |
| :------------------ | :----- |
| reportrefreshdate   | Date   |
| reportDate          | Date   |
| teamchatmessages    | Int64  |
| privateChatMessages | Int64  |
| calls               | Int64  |
| meetings            | Int64  |
| otheractions        | Int64  |
| reportperiod        | String |

## <a name="json-representation"></a>JSON 表記

リソースの JSON 表記を次に示します。

<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.teamsUserActivityUserCounts"
} -->

```json
{
  "reportRefreshDate": "Date", 
  "reportDate": "Date", 
  "teamChatMessages": 1024, 
  "privateChatMessages": 1024, 
  "calls": 1024, 
  "meetings": 1024, 
  "otherActions": 1024, 
  "reportPeriod": "String"
}
```
