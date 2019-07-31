---
title: Siteの種類ストレージリソースの種類
description: リソースの JSON 表記を次に示します。
localization_priority: Normal
ms.prod: sharepoint
doc_type: resourcePageType
author: ''
ms.openlocfilehash: 1ed15d4efb1c9a0fa81fdd79faeb9542d8093aab
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "36008230"
---
# <a name="siteusagestorage-resource-type"></a>Siteの種類ストレージリソースの種類

## <a name="properties"></a>プロパティ

| プロパティ           | 型   |
| :----------------- | :----- |
| reportRefreshDate  | 日付   |
| siteType           | String |
| Storageused Inbytes | Int64  |
| reportDate         | 日付   |
| reportPeriod       | String |

## <a name="json-representation"></a>JSON 表記

リソースの JSON 表記を次に示します。

<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.siteUsageStorage"
} -->

```json
{
  "reportRefreshDate": "Date", 
  "siteType": "String", 
  "storageUsedInBytes": 1024, 
  "reportDate": "Date", 
  "reportPeriod": "String"
}
```
