---
title: yammerActivityUserDetail リソースの種類
description: リソースの JSON 表記を次に示します。
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
ms.openlocfilehash: eea520e6024bb050001461fb5ada5c90ea2b2125
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32541186"
---
# <a name="yammeractivityuserdetail-resource-type"></a>yammerActivityUserDetail リソースの種類

## <a name="properties"></a>プロパティ

| プロパティ          | 型              |
| :---------------- | :---------------- |
| reportrefreshdate | Date              |
| userPrincipalName | String            |
| displayName       | String            |
| userState         | String            |
| stateChangeDate   | Date              |
| lastactivitydate  | Date              |
| postedCount       | Int64             |
| readcount         | Int64             |
| dcount        | Int64             |
| assignedProducts  | String collection |
| reportperiod      | String            |

## <a name="json-representation"></a>JSON 表記

リソースの JSON 表記を次に示します。

<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.yammerActivityUserDetail"
} -->

```json
{
  "reportRefreshDate": "Date", 
  "userPrincipalName": "String", 
  "displayName": "String", 
  "userState": "String", 
  "stateChangeDate": "Date", 
  "lastActivityDate": "Date", 
  "postedCount": 1024, 
  "readCount": 1024, 
  "likedCount": 1024, 
  "assignedProducts": ["String"], 
  "reportPeriod": "String"
}
```
