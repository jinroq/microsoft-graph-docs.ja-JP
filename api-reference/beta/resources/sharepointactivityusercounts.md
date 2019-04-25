---
title: sharepointactivityusercounts リソースの種類
description: リソースの JSON 表記を次に示します。
localization_priority: Normal
ms.prod: sharepoint
ms.openlocfilehash: 9656b39572eac5b6474dd7884eb7d1d2edb17310
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32583950"
---
# <a name="sharepointactivityusercounts-resource-type"></a>sharepointactivityusercounts リソースの種類

## <a name="properties"></a>プロパティ

| プロパティ          | 型   |
| :---------------- | :----- |
| reportrefreshdate | Date   |
| visitedPage       | Int64  |
| viewedOrEdited    | Int64  |
| 同期            | Int64  |
| sharedinternally  | Int64  |
| sharedExternally  | Int64  |
| reportDate        | Date   |
| reportperiod      | String |

## <a name="json-representation"></a>JSON 表記

リソースの JSON 表記を次に示します。

<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.sharePointActivityUserCounts"
} -->

```json
{
  "reportRefreshDate": "Date", 
  "visitedPage": 1024, 
  "viewedOrEdited": 1024, 
  "synced": 1024, 
  "sharedInternally": 1024, 
  "sharedExternally": 1024, 
  "reportDate": "Date", 
  "reportPeriod": "String"
}
```
