---
title: teamsDeviceUsageUserCounts リソースの種類
description: リソースの JSON 表記を次に示します。
ms.openlocfilehash: 9640af67efc18f0a70c636673169e884ce82d971
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27073765"
---
# <a name="teamsdeviceusageusercounts-resource-type"></a>teamsDeviceUsageUserCounts リソースの種類

## <a name="properties"></a>プロパティ

| プロパティ          | 型   |
| :---------------- | :----- |
| reportRefreshDate | Date   |
| web               | Int64  |
| windowsPhone      | Int64  |
| androidPhone      | Int64  |
| ios               | Int64  |
| Mac               | Int64  |
| windows           | Int64  |
| reportDate        | Date   |
| reportPeriod      | String |

## <a name="json-representation"></a>JSON 表記

リソースの JSON 表記を次に示します。

<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.teamsDeviceUsageUserCounts"
} -->

```json
{
  "reportRefreshDate": "Date", 
  "web": 1024, 
  "windowsPhone": 1024, 
  "androidPhone": 1024, 
  "ios": 1024, 
  "mac": 1024, 
  "windows": 1024, 
  "reportDate": "Date", 
  "reportPeriod": "String"
}
```
