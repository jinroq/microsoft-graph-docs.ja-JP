---
title: teamsDeviceUsageDistributionUserCounts リソースの種類
description: リソースの JSON 表記を次に示します。
ms.openlocfilehash: b039320e389e1a61832089991b2368b27e51c475
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27066736"
---
# <a name="teamsdeviceusagedistributionusercounts-resource-type"></a>teamsDeviceUsageDistributionUserCounts リソースの種類

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
| reportPeriod      | String |

## <a name="json-representation"></a>JSON 表記

リソースの JSON 表記を次に示します。

<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.teamsDeviceUsageDistributionUserCounts"
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
  "reportPeriod": "String"
}
```