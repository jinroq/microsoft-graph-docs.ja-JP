---
title: yammerDeviceUsageUserDetail リソースの種類
description: リソースの JSON 表記を次に示します。
localization_priority: Normal
ms.openlocfilehash: 0f4d543ec8a96eaa4e237a1db1367efdc625c4e6
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/11/2019
ms.locfileid: "27892016"
---
# <a name="yammerdeviceusageuserdetail-resource-type"></a>yammerDeviceUsageUserDetail リソースの種類

## <a name="properties"></a>プロパティ

| プロパティ          | 種類    |
| :---------------- | :------ |
| reportRefreshDate | 日付    |
| userPrincipalName | String  |
| displayName       | String  |
| userState         | String  |
| stateChangeDate   | 日付    |
| lastActivityDate  | 日付    |
| usedWeb           | ブール型 |
| usedWindowsPhone  | ブール型 |
| usedAndroidPhone  | ブール型 |
| usediPhone        | ブール型 |
| usediPad          | ブール型 |
| usedOthers        | ブール型 |
| reportPeriod      | String  |

## <a name="json-representation"></a>JSON 表記

リソースの JSON 表記を次に示します。

<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.yammerDeviceUsageUserDetail"
} -->

```json
{
  "reportRefreshDate": "Date", 
  "userPrincipalName": "String", 
  "displayName": "String", 
  "userState": "String", 
  "stateChangeDate": "Date", 
  "lastActivityDate": "Date", 
  "usedWeb": true, 
  "usedWindowsPhone": true, 
  "usedAndroidPhone": true, 
  "usediPhone": true, 
  "usediPad": true, 
  "usedOthers": true, 
  "reportPeriod": "String"
}
```
