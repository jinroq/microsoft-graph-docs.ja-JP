---
title: teamsUserActivityUserDetail リソースの種類
description: リソースの JSON の representaion は、次のようにします。
author: nkramer
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: 32b611ee9ec01b0339389256b8c8dff9eac99fa9
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/12/2019
ms.locfileid: "27913430"
---
# <a name="teamsuseractivityuserdetail-resource-type"></a>teamsUserActivityUserDetail リソースの種類

## <a name="properties"></a>プロパティ

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
