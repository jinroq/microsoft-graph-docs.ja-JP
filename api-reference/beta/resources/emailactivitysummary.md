---
title: emailActivitySummary リソースの種類
description: リソースの JSON 表記を次に示します。
localization_priority: Normal
ms.openlocfilehash: 82fbdc2621b9c8746ed3028fe44414edeb7e56db
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/11/2019
ms.locfileid: "27871345"
---
# <a name="emailactivitysummary-resource-type"></a>emailActivitySummary リソースの種類

## <a name="properties"></a>プロパティ

| プロパティ          | 種類   |
| :---------------- | :----- |
| reportRefreshDate | 日付   |
| 送信              | Int64  |
| 表示されます。           | Int64  |
| 読み取り              | Int64  |
| reportDate        | 日付   |
| reportPeriod      | String |

## <a name="json-representation"></a>JSON 表記

リソースの JSON 表記を次に示します。

<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.emailActivitySummary"
} -->

```json
{
  "reportRefreshDate": "Date", 
  "send": 1024, 
  "receive": 1024, 
  "read": 1024, 
  "reportDate": "Date", 
  "reportPeriod": "String"
}
```
