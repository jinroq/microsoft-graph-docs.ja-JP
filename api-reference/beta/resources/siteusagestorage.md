---
title: siteUsageStorage リソースの種類
description: リソースの JSON 表記を次に示します。
localization_priority: Normal
ms.prod: sharepoint
ms.openlocfilehash: c136b776e0c96a8bc63a1c82ae2ad17f059026cc
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/12/2019
ms.locfileid: "27928102"
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
