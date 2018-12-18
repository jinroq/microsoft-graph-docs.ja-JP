---
title: teamsUserActivityUserDetail リソースの種類
description: リソースの JSON の representaion は、次のようにします。
author: nkramer
ms.openlocfilehash: a1f47bc52c2a0a613598ce663f16023dce208c51
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 12/18/2018
ms.locfileid: "27331942"
---
# <a name="teamsuseractivityuserdetail-resource-type"></a>teamsUserActivityUserDetail リソースの種類

## <a name="properties"></a>Properties

| プロパティ                | 種類              |
| :---------------------- | :---------------- |
| reportRefreshDate       | 日付              |
| userPrincipalName       | String            |
| lastActivityDate        | 日付              |
| isDeleted               | ブール型           |
| deletedDate             | 日付              |
| assignedProducts        | String コレクション |
| teamChatMessageCount    | Int64             |
| privateChatMessageCount | Int64             |
| callCount               | Int64             |
| meetingCount            | Int64             |
| hasOtherAction          | ブール型           |
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
