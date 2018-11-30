---
title: teamsUserActivityUserDetail リソースの種類
description: リソースの JSON の representaion は、次のようにします。
ms.openlocfilehash: 4e40ea4adf07450e6b51555df47579955a2a0286
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27073145"
---
# <a name="teamsuseractivityuserdetail-resource-type"></a>teamsUserActivityUserDetail リソースの種類

## <a name="properties"></a>プロパティ

| プロパティ                | 型              |
| :---------------------- | :---------------- |
| reportRefreshDate       | Date              |
| userPrincipalName       | String            |
| lastActivityDate        | Date              |
| isDeleted               | ブール値           |
| deletedDate             | Date              |
| assignedProducts        | String コレクション |
| teamChatMessageCount    | Int64             |
| privateChatMessageCount | Int64             |
| callCount               | Int64             |
| meetingCount            | Int64             |
| hasOtherAction          | ブール値           |
| reportPeriod            | String            |

## <a name="json-representation"></a>JSON 表記

リソースの JSON の representaion は、次のようにします。

<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.teamsUserActivityUserDetail"
} -->

```json
{
  "reportRefreshDate": "Date", 
  "userPrincipalName": "String", 
  "lastActivityDate": "Date", 
  "isDeleted": true, 
  "deletedDate": "Date", 
  "assignedProducts": ["String"],
  "teamChatMessageCount": 1024, 
  "privateChatMessageCount": 1024, 
  "callCount": 1024, 
  "meetingCount": 1024, 
  "hasOtherAction": true, 
  "reportPeriod": "String"
}
```
