---
title: skypeForBusinessDeviceUsageDistributionUserCounts リソースの種類
description: リソースの JSON 表記を次に示します。
ms.openlocfilehash: 1534051455d805cf3bc9fabbb301ffde5be85ad9
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27074497"
---
# <a name="skypeforbusinessdeviceusagedistributionusercounts-resource-type"></a>skypeForBusinessDeviceUsageDistributionUserCounts リソースの種類

## <a name="properties"></a>プロパティ

| プロパティ          | 型   |
| :---------------- | :----- |
| reportRefreshDate | Date   |
| windows           | Int64  |
| windowsPhone      | Int64  |
| androidPhone      | Int64  |
| iPhone            | Int64  |
| iPad              | Int64  |
| reportPeriod      | String |

## <a name="json-representation"></a>JSON 表記

リソースの JSON 表記を次に示します。

<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.skypeForBusinessDeviceUsageDistributionUserCounts"
} -->

```json
{
  "reportRefreshDate": "Date", 
  "windows": 1024, 
  "windowsPhone": 1024, 
  "androidPhone": 1024, 
  "iPhone": 1024, 
  "iPad": 1024, 
  "reportPeriod": "String"
}
```
