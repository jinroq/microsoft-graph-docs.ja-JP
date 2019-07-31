---
title: skypeForBusinessActivityUserCounts リソースの種類
description: リソースの JSON 表記を次に示します。
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
author: ''
ms.openlocfilehash: 2d723655e55c2702dd2b68adf65e43b6af16c36a
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "35964936"
---
# <a name="skypeforbusinessactivityusercounts-resource-type"></a>skypeForBusinessActivityUserCounts リソースの種類

## <a name="properties"></a>プロパティ

| プロパティ          | 型   |
| :---------------- | :----- |
| peerToPeer        | Int64  |
| 別         | Int64  |
| 参加した      | Int64  |
| reportRefreshDate | 日付   |
| reportDate        | 日付   |
| reportPeriod      | String |

## <a name="json-representation"></a>JSON 表記

リソースの JSON 表記を次に示します。

<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.skypeForBusinessActivityUserCounts"
} -->

```json
{
  "peerToPeer": 1024, 
  "organized": 1024, 
  "participated": 1024, 
  "reportRefreshDate": "Date", 
  "reportDate": "Date", 
  "reportPeriod": "String"
}
```
