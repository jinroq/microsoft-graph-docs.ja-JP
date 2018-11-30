---
title: yammerDeviceUsageUserCounts リソースの種類
description: リソースの JSON 表記を次に示します。
ms.openlocfilehash: 7faec83d113da3f412c913177a717fdc69504310
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27069971"
---
# <a name="yammerdeviceusageusercounts-resource-type"></a>yammerDeviceUsageUserCounts リソースの種類

## <a name="properties"></a>プロパティ

| プロパティ          | 型   |
| :---------------- | :----- |
| reportRefreshDate | Date   |
| web               | Int32  |
| windowsPhone      | Int32  |
| androidPhone      | Int32  |
| iPhone            | Int32  |
| iPad              | Int32  |
| その他の             | Int32  |
| reportDate        | Date   |
| reportPeriod      | String |

## <a name="json-representation"></a>JSON 表記

リソースの JSON 表記を次に示します。

<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.yammerDeviceUsageUserCounts"
} -->

```json
{
  "reportRefreshDate": "Date", 
  "web": 1024, 
  "windowsPhone": 1024, 
  "androidPhone": 1024, 
  "iPhone": 1024, 
  "iPad": 1024, 
  "other": 1024, 
  "reportDate": "Date", 
  "reportPeriod": "String"
}
```
