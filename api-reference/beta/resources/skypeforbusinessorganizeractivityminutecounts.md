---
title: skypeForBusinessOrganizerActivityMinuteCounts リソースの種類
description: リソースの JSON 表記を次に示します。
localization_priority: Normal
ms.openlocfilehash: 6b3b38c61ebb7b294de9ea5fc2641a7527bf04f7
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32461186"
---
# <a name="skypeforbusinessorganizeractivityminutecounts-resource-type"></a>skypeForBusinessOrganizerActivityMinuteCounts リソースの種類

## <a name="properties"></a>プロパティ

| プロパティ           | 型   |
| :----------------- | :----- |
| audioVideo         | Int64  |
| dialInOut3rdParty  | Int64  |
| ダイヤルアウト microsoft | Int64  |
| reportrefreshdate  | Date   |
| reportDate         | Date   |
| reportperiod       | String |

## <a name="json-representation"></a>JSON 表記

リソースの JSON 表記を次に示します。

<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.skypeForBusinessOrganizerActivityMinuteCounts"
} -->

```json
{
  "audioVideo": 1024, 
  "dialInMicrosoft": 1024, 
  "dialOutMicrosoft": 1024, 
  "reportRefreshDate": "Date", 
  "reportDate": "Date", 
  "reportPeriod": "String"
}
```
