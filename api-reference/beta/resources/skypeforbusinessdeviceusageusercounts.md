---
title: skypeforbusinessdevice使い方 user計数リソースの種類
description: リソースの JSON 表記を次に示します。
localization_priority: Normal
ms.openlocfilehash: d98590e83637e45d35f135c56f2c0b8ff7d282bb
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32583502"
---
# <a name="skypeforbusinessdeviceusageusercounts-resource-type"></a>skypeforbusinessdevice使い方 user計数リソースの種類

## <a name="properties"></a>プロパティ

| プロパティ          | 型   |
| :---------------- | :----- |
| reportrefreshdate | Date   |
| ws           | Int64  |
| windowsPhone      | Int64  |
| androidphone      | Int64  |
| iPhone            | Int64  |
| iPad              | Int64  |
| reportDate        | Date   |
| reportperiod      | String |

## <a name="json-representation"></a>JSON 表記

リソースの JSON 表記を次に示します。

<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.skypeForBusinessDeviceUsageUserCounts"
} -->

```json
{
  "reportRefreshDate": "Date", 
  "windows": 1024, 
  "windowsPhone": 1024, 
  "androidPhone": 1024, 
  "iPhone": 1024, 
  "iPad": 1024, 
  "reportDate": "Date", 
  "reportPeriod": "String"
}
```
