---
title: skypeForBusinessDeviceUsageUserDetail リソースの種類
description: リソースの JSON 表記を次に示します。
localization_priority: Normal
ms.openlocfilehash: 95f2f6cf1f3f6c54c4b6b4b39a7118cd8a94b224
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/11/2019
ms.locfileid: "27858381"
---
# <a name="skypeforbusinessdeviceusageuserdetail-resource-type"></a>skypeForBusinessDeviceUsageUserDetail リソースの種類

## <a name="properties"></a>プロパティ

| プロパティ          | 種類    |
| :---------------- | :------ |
| reportRefreshDate | 日付    |
| userPrincipalName | String  |
| lastActivityDate  | 日付    |
| usedWindows       | ブール型 |
| usedWindowsPhone  | ブール型 |
| usedAndroidPhone  | ブール型 |
| usediPhone        | ブール型 |
| usediPad          | ブール型 |
| reportPeriod      | String  |

## <a name="json-representation"></a>JSON 表記

リソースの JSON 表記を次に示します。

<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.skypeForBusinessDeviceUsageUserDetail"
} -->

```json
{
  "reportRefreshDate": "Date", 
  "userPrincipalName": "String", 
  "lastActivityDate": "Date", 
  "usedWindows": true, 
  "usedWindowsPhone": true, 
  "usedAndroidPhone": true, 
  "usediPhone": true, 
  "usediPad": true, 
  "reportPeriod": "String"
}
```
