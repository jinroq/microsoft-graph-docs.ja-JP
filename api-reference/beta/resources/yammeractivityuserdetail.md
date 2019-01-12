---
title: yammerActivityUserDetail リソースの種類
description: リソースの JSON 表記を次に示します。
localization_priority: Normal
ms.prod: reports
ms.openlocfilehash: d24e21c9525d49b7af5f8c4efaddd606c20c162b
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/12/2019
ms.locfileid: "27923034"
---
# <a name="yammeractivityuserdetail-resource-type"></a>yammerActivityUserDetail リソースの種類

## <a name="properties"></a>プロパティ

| プロパティ          | 種類              |
| :---------------- | :---------------- |
| reportRefreshDate | 日付              |
| userPrincipalName | String            |
| displayName       | String            |
| userState         | String            |
| stateChangeDate   | 日付              |
| lastActivityDate  | 日付              |
| postedCount       | Int64             |
| readCount         | Int64             |
| likedCount        | Int64             |
| assignedProducts  | String コレクション |
| reportPeriod      | String            |

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
