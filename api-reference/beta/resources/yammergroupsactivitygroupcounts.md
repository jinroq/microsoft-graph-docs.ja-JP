---
title: yammerGroupsActivityGroupCounts リソースの種類
description: リソースの JSON 表記を次に示します。
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
ms.openlocfilehash: 5ecf28f8389fa9ccd61be675f32f7ae7f4bf7907
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32551387"
---
# <a name="yammergroupsactivitygroupcounts-resource-type"></a>yammerGroupsActivityGroupCounts リソースの種類

## <a name="properties"></a>プロパティ

| プロパティ          | 型   |
| :---------------- | :----- |
| reportrefreshdate | Date   |
| total             | Int64  |
| active            | Int64  |
| reportDate        | Date   |
| reportperiod      | String |

## <a name="json-representation"></a>JSON 表記

リソースの JSON 表記を次に示します。

<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.yammerGroupsActivityGroupCounts"
} -->

```json
{
  "reportRefreshDate": "Date", 
  "total": 1024, 
  "active": 1024, 
  "reportDate": "Date", 
  "reportPeriod": "String"
}
```
