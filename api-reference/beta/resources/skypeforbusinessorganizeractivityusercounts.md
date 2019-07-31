---
title: Skypeforbusinessオーガナイザー Eractivityuser計数リソースの種類
description: リソースの JSON 表記を次に示します。
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
author: ''
ms.openlocfilehash: b6fcb2114e78bd9aabb170795b49d80bb58e6844
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "35964873"
---
# <a name="skypeforbusinessorganizeractivityusercounts-resource-type"></a>Skypeforbusinessオーガナイザー Eractivityuser計数リソースの種類

## <a name="properties"></a>プロパティ

| プロパティ           | 型   |
| :----------------- | :----- |
| im                 | Int64  |
| audioVideo         | Int64  |
| appSharing         | Int64  |
| Web                | Int64  |
| dialInOut3rdParty  | Int64  |
| ダイヤルアウト Microsoft | Int64  |
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
