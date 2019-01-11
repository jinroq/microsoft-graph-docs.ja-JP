---
title: siteUsageStorage リソースの種類
description: リソースの JSON 表記を次に示します。
localization_priority: Normal
ms.openlocfilehash: 1f656feacdbba3418049bd9f3072270aa04af798
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/11/2019
ms.locfileid: "27879927"
---
# <a name="siteusagestorage-resource-type"></a>siteUsageStorage リソースの種類

## <a name="properties"></a>プロパティ

| プロパティ           | 種類   |
| :----------------- | :----- |
| reportRefreshDate  | 日付   |
| ある           | String |
| storageUsedInBytes | Int64  |
| reportDate         | 日付   |
| reportPeriod       | String |

## <a name="json-representation"></a>JSON 表記

リソースの JSON 表記を次に示します。

<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.siteUsageStorage"
} -->

```json
{
  "reportRefreshDate": "Date", 
  "siteType": "String", 
  "storageUsedInBytes": 1024, 
  "reportDate": "Date", 
  "reportPeriod": "String"
}
```
