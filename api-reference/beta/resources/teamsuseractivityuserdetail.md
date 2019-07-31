---
title: teamsUserActivityUserDetail リソースの種類
description: 以下に、リソースの JSON 表記を示します。
author: nkramer
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: cbe6297388907f28f8841e0a1dcb2ec3ae788844
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "35964355"
---
# <a name="teamsuseractivityuserdetail-resource-type"></a>teamsUserActivityUserDetail リソースの種類

## <a name="properties"></a>プロパティ

| プロパティ                | 型              |
| :---------------------- | :---------------- |
| reportRefreshDate       | 日付              |
| userPrincipalName       | String            |
| lastActivityDate        | 日付              |
| isDeleted               | Boolean           |
| deletedDate             | 日付              |
| assignedProducts        | 文字列コレクション |
| teamChatMessageCount    | Int64             |
| privateChatMessageCount | Int64             |
| callCount               | Int64             |
| 会議数            | Int64             |
| hasOtherAction          | Boolean           |
| reportPeriod            | String            |

## <a name="json-representation"></a>JSON 表記

以下に、リソースの JSON 表記を示します。

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
