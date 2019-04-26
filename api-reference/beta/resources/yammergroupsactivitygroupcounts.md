---
title: yammerGroupsActivityGroupCounts リソースの種類
description: リソースの JSON 表記を次に示します。
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
ms.openlocfilehash: 64947a1d151cab3dca14f4f232671242e1a985cc
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/26/2019
ms.locfileid: "33342731"
---
# <a name="yammergroupsactivitygroupcounts-resource-type"></a>yammerGroupsActivityGroupCounts リソースの種類

## <a name="properties"></a>プロパティ

| プロパティ          | 型   | 説明 |
| :---------------- | :----- | :---------- |
| reportrefreshdate | 日付   |             |
| total             | Int64  |             |
| active            | Int64  |             |
| reportDate        | 日付   |             |
| reportperiod      | String |             |

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
