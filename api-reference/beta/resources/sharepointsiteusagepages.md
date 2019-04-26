---
title: sharepointsiteの pages リソースの種類
description: リソースの JSON 表記を次に示します。
localization_priority: Normal
ms.prod: sharepoint
ms.openlocfilehash: 1a82c0a1174559db6d90e64f1fd1ed1403caa048
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32584055"
---
# <a name="sharepointsiteusagepages-resource-type"></a>sharepointsiteの pages リソースの種類

## <a name="properties"></a>プロパティ

| プロパティ          | 型   |
| :---------------- | :----- |
| reportrefreshdate | Date   |
| sitetype          | String |
| pageviewcount     | Int64  |
| reportDate        | Date   |
| reportperiod      | String |

## <a name="json-representation"></a>JSON 表記

リソースの JSON 表記を次に示します。

<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.sharePointSiteUsagePages"
} -->

```json
{
  "reportRefreshDate": "Date", 
  "siteType": "String", 
  "pageViewCount": 1024, 
  "reportDate": "Date", 
  "reportPeriod": "String"
}
```
