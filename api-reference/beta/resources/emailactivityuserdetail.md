---
title: emailactivityuserdetail リソースの種類
description: リソースの JSON 表記を次に示します。
localization_priority: Normal
author: angelgolfer-ms
ms.prod: outlook
ms.openlocfilehash: b871bf5dbaedd961fad09bf97be868f46e7430a1
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32542833"
---
# <a name="emailactivityuserdetail-resource-type"></a>emailactivityuserdetail リソースの種類

## <a name="properties"></a>プロパティ

| プロパティ          | 型              |
| :---------------- | :---------------- |
| reportrefreshdate | Date              |
| userPrincipalName | String            |
| displayName       | String            |
| isDeleted         | ブール値           |
| deletedDate       | Date              |
| lastactivitydate  | Date              |
| sendcount         | Int64             |
| receiveCount      | Int64             |
| readcount         | Int64             |
| assignedProducts  | String collection |
| reportperiod      | String            |

## <a name="json-representation"></a>JSON 表記

リソースの JSON 表記を次に示します。

<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.emailActivityUserDetail"
} -->

```json
{
  "reportRefreshDate": "Date", 
  "userPrincipalName": "String", 
  "displayName": "String", 
  "isDeleted": true, 
  "deletedDate": "Date", 
  "lastActivityDate": "Date", 
  "sendCount": 1024, 
  "receiveCount": 1024, 
  "readCount": 1024, 
  "assignedProducts": ["String"], 
  "reportPeriod": "String"
}
```
