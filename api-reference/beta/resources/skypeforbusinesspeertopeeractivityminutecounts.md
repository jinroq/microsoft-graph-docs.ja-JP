---
title: skypeForBusinessPeerToPeerActivityMinuteCounts リソースの種類
description: リソースの JSON 表記を次に示します。
ms.openlocfilehash: 5377e8d8f2ec145f5aee590409206de75e915d9f
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27073322"
---
# <a name="skypeforbusinesspeertopeeractivityminutecounts-resource-type"></a>skypeForBusinessPeerToPeerActivityMinuteCounts リソースの種類

## <a name="properties"></a>プロパティ

| プロパティ          | 型   |
| :---------------- | :----- |
| audio             | Int64  |
| video             | Int64  |
| reportRefreshDate | Date   |
| reportDate        | Date   |
| reportPeriod      | String |

## <a name="json-representation"></a>JSON 表記

リソースの JSON 表記を次に示します。

<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.skypeForBusinessPeerToPeerActivityMinuteCounts"
} -->

```json
{
  "audio": 1024, 
  "video": 1024, 
  "reportRefreshDate": "Date", 
  "reportDate": "Date", 
  "reportPeriod": "String"
}
```
