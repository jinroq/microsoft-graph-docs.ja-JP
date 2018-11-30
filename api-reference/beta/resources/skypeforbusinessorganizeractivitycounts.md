---
title: skypeForBusinessOrganizerActivityCounts リソースの種類
description: リソースの JSON 表記を次に示します。
ms.openlocfilehash: 0729aef6367ebcb0a5edfaa461d80ffd8cb0775c
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27074496"
---
# <a name="skypeforbusinessorganizeractivitycounts-resource-type"></a>skypeForBusinessOrganizerActivityCounts リソースの種類

## <a name="properties"></a>プロパティ

| プロパティ           | 型   |
| :----------------- | :----- |
| im                 | Int64  |
| audioVideo         | Int64  |
| appSharing         | Int64  |
| web                | Int64  |
| dialInOut3rdParty  | Int64  |
| dialInOutMicrosoft | Int64  |
| reportRefreshDate  | Date   |
| reportDate         | Date   |
| reportPeriod       | String |

## <a name="json-representation"></a>JSON 表記

リソースの JSON 表記を次に示します。

<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.skypeForBusinessOrganizerActivityCounts"
} -->

```json
{
  "im": 1024, 
  "audioVideo": 1024, 
  "appSharing": 1024, 
  "web": 1024, 
  "dialInOut3rdParty": 1024, 
  "dialInOutMicrosoft": 1024, 
  "reportRefreshDate": "Date", 
  "reportDate": "Date", 
  "reportPeriod": "String"
}
```