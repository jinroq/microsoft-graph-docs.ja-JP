---
title: sharePointActivityPages リソースの種類
description: リソースの JSON 表記を次に示します。
localization_priority: Normal
ms.openlocfilehash: 758dcfd2e1c48b0bf8d0d85f06a68f26bfbbef99
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/11/2019
ms.locfileid: "27811845"
---
# <a name="sharepointactivitypages-resource-type"></a>sharePointActivityPages リソースの種類

## <a name="properties"></a>プロパティ

| プロパティ          | 種類   |
| :---------------- | :----- |
| reportRefreshDate | 日付   |
| visitedPageCount  | Int64  |
| reportDate        | 日付   |
| reportPeriod      | String |

## <a name="json-representation"></a>JSON 表記

リソースの JSON 表記を次に示します。

<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.sharePointActivityPages"
} -->

```json
{
  "reportRefreshDate": "Date", 
  "visitedPageCount": 1024, 
  "reportDate": "Date", 
  "reportPeriod": "String"
}
```
