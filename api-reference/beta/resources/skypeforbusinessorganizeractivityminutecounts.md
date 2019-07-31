---
title: skypeForBusinessOrganizerActivityMinuteCounts リソースの種類
description: リソースの JSON 表記を次に示します。
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
author: ''
ms.openlocfilehash: c06f2f266cf86d0eae9166b5520a4519d045f948
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "35964894"
---
# <a name="skypeforbusinessorganizeractivityminutecounts-resource-type"></a>skypeForBusinessOrganizerActivityMinuteCounts リソースの種類

## <a name="properties"></a>プロパティ

| プロパティ           | 型   |
| :----------------- | :----- |
| audioVideo         | Int64  |
| dialInMicrosoft    | Int64  |
| ダイヤルアウト Microsoft   | Int64  |
| reportRefreshDate  | 日付   |
| reportDate         | 日付   |
| reportPeriod       | String |

## <a name="json-representation"></a>JSON 表記

リソースの JSON 表記を次に示します。

<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.skypeForBusinessOrganizerActivityMinuteCounts"
} -->

```json
{
  "audioVideo": 1024,
  "dialInMicrosoft": 1024,
  "dialOutMicrosoft": 1024,
  "reportRefreshDate": "Date",
  "reportDate": "Date",
  "reportPeriod": "String"
}
```
