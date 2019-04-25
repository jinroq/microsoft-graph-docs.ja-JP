---
title: skypeforbusinessオーガナイザー eractivityuser計数リソースの種類
description: リソースの JSON 表記を次に示します。
localization_priority: Normal
ms.openlocfilehash: 39ab5844adb9525b4e0f100892927d200609040c
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32534865"
---
# <a name="skypeforbusinessorganizeractivityusercounts-resource-type"></a>skypeforbusinessオーガナイザー eractivityuser計数リソースの種類

## <a name="properties"></a>プロパティ

| プロパティ           | 型   |
| :----------------- | :----- |
| im                 | Int64  |
| audioVideo         | Int64  |
| appSharing         | Int64  |
| web                | Int64  |
| dialInOut3rdParty  | Int64  |
| ダイヤルアウト microsoft | Int64  |
| reportrefreshdate  | Date   |
| reportDate         | Date   |
| reportperiod       | String |

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
