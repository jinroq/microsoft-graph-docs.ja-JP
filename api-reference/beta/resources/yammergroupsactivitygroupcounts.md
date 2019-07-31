---
title: yammerGroupsActivityGroupCounts リソースの種類
description: リソースの JSON 表記を次に示します。
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
doc_type: resourcePageType
ms.openlocfilehash: 4c342686ce2397a5d3b1dd697002fb44e16f3b11
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "36006921"
---
# <a name="yammergroupsactivitygroupcounts-resource-type"></a>yammerGroupsActivityGroupCounts リソースの種類

## <a name="properties"></a>プロパティ

| プロパティ          | 型   | 説明 |
| :---------------- | :----- | :---------- |
| reportRefreshDate | 日付   |             |
| total             | Int64  |             |
| active            | Int64  |             |
| reportDate        | 日付   |             |
| reportPeriod      | String |             |

## <a name="json-representation"></a>JSON 表記

リソースの JSON 表記を次に示します。

<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.yammerGroupsActivityGroupCounts"
} -->

```json
{
  "reportRefreshDate": "String", 
  "total": 1024, 
  "active": 1024, 
  "reportDate": "String", 
  "reportPeriod": "String"
}
```
