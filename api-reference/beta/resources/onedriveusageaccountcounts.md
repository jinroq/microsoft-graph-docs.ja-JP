---
title: oneDriveUsageAccountCounts リソースの種類
description: リソースの JSON 表記を次に示します。
localization_priority: Normal
ms.prod: sharepoint
ms.openlocfilehash: dd70875c272f63a1c9a7988c001225c2d200e0c6
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/12/2019
ms.locfileid: "27947184"
---
# <a name="onedriveusageaccountcounts-resource-type"></a>oneDriveUsageAccountCounts リソースの種類

## <a name="properties"></a>プロパティ

| プロパティ          | 種類   |
| :---------------- | :----- |
| reportRefreshDate | 日付   |
| ある          | String |
| total             | Int64  |
| アクティブです            | Int64  |
| reportDate        | 日付   |
| reportPeriod      | String |

## <a name="json-representation"></a>JSON 表記

リソースの JSON 表記を次に示します。

<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.oneDriveUsageAccountCounts"
} -->

```json
{
  "reportRefreshDate": "Date", 
  "siteType": "String", 
  "total": 1024, 
  "active": 1024, 
  "reportDate": "Date", 
  "reportPeriod": "String"
}
```
