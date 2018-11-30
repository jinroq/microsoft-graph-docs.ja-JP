---
title: yammerGroupsActivityCounts リソースの種類
description: リソースの JSON 表記を次に示します。
ms.openlocfilehash: a308b6180eaf91614247b0b5f47064ae7e7de2b2
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27073143"
---
# <a name="yammergroupsactivitycounts-resource-type"></a>yammerGroupsActivityCounts リソースの種類

## <a name="properties"></a>プロパティ

| プロパティ          | 型   |
| :---------------- | :----- |
| reportRefreshDate | Date   |
| 気に入られました             | Int64  |
| 転記            | Int64  |
| 読み取り              | Int64  |
| reportDate        | Date   |
| reportPeriod      | String |

## <a name="json-representation"></a>JSON 表記

リソースの JSON 表記を次に示します。

<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.yammerGroupsActivityCounts"
} -->

```json
{
  "reportRefreshDate": "Date", 
  "liked": 1024, 
  "posted": 1024, 
  "read": 1024, 
  "reportDate": "Date", 
  "reportPeriod": "String"
}
```
