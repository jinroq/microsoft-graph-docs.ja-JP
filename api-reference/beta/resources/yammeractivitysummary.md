---
title: yammerActivitySummary リソースの種類
description: リソースの JSON 表記を次に示します。
ms.openlocfilehash: 6ff2b347de77f91c96cb5f5be797eb70db0bbbee
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27067433"
---
# <a name="yammeractivitysummary-resource-type"></a>yammerActivitySummary リソースの種類

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
  "@odata.type": "microsoft.graph.yammerActivitySummary"
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
