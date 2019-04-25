---
title: teamsuseractivityuserdetail リソースの種類
description: 以下に、リソースの JSON 表記を示します。
author: nkramer
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: 32b611ee9ec01b0339389256b8c8dff9eac99fa9
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32582907"
---
# <a name="teamsuseractivityuserdetail-resource-type"></a>teamsuseractivityuserdetail リソースの種類

## <a name="properties"></a>プロパティ

| プロパティ                | 型              |
| :---------------------- | :---------------- |
| reportrefreshdate       | Date              |
| userPrincipalName       | String            |
| lastactivitydate        | Date              |
| isDeleted               | Boolean           |
| deletedDate             | Date              |
| assignedProducts        | String collection |
| teamchatmessagecount    | Int64             |
| privateChatMessageCount | Int64             |
| callcount               | Int64             |
| 会議数            | Int64             |
| hasotheraction          | Boolean           |
| reportperiod            | String            |

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
