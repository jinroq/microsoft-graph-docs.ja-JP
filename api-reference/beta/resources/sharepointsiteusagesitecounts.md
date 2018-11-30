---
title: sharePointSiteUsageSiteCounts リソースの種類
description: リソースの JSON 表記を次に示します。
ms.openlocfilehash: 631e01a417e177e356b701ca8dc93ffa51b4f50f
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27068116"
---
# <a name="sharepointsiteusagesitecounts-resource-type"></a>sharePointSiteUsageSiteCounts リソースの種類

## <a name="properties"></a>プロパティ

| プロパティ          | 型   |
| :---------------- | :----- |
| reportRefreshDate | Date   |
| ある          | String |
| total             | Int64  |
| アクティブです            | Int64  |
| reportDate        | Date   |
| reportPeriod      | String |

## <a name="json-representation"></a>JSON 表記

リソースの JSON 表記を次に示します。

<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.sharePointSiteUsageSiteCounts"
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
