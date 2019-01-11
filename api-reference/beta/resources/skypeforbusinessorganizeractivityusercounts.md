---
title: skypeForBusinessOrganizerActivityUserCounts リソースの種類
description: リソースの JSON 表記を次に示します。
localization_priority: Normal
ms.openlocfilehash: 39ab5844adb9525b4e0f100892927d200609040c
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/11/2019
ms.locfileid: "27858711"
---
# <a name="skypeforbusinessorganizeractivityusercounts-resource-type"></a>skypeForBusinessOrganizerActivityUserCounts リソースの種類

## <a name="properties"></a>プロパティ

| プロパティ           | 種類   |
| :----------------- | :----- |
| im                 | Int64  |
| audioVideo         | Int64  |
| appSharing         | Int64  |
| web                | Int64  |
| dialInOut3rdParty  | Int64  |
| dialInOutMicrosoft | Int64  |
| reportRefreshDate  | 日付   |
| reportDate         | 日付   |
| reportPeriod       | String |

## <a name="json-representation"></a>JSON 表記

リソースの JSON 表記を次に示します。

<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.skypeForBusinessOrganizerActivityUserCounts"
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
