---
title: teamsDeviceUsageUserDetail リソースの種類
description: リソースの JSON 表記を次に示します。
author: nkramer
localization_priority: Normal
ms.openlocfilehash: 06e2cea1154c608b61642b07adbd96aae1710903
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/11/2019
ms.locfileid: "27807106"
---
# <a name="teamsdeviceusageuserdetail-resource-type"></a>teamsDeviceUsageUserDetail リソースの種類

## <a name="properties"></a>プロパティ

| プロパティ          | 種類    |
| :---------------- | :------ |
| reportRefreshDate | 日付    |
| userPrincipalName | String  |
| lastActivityDate  | 日付    |
| isDeleted         | ブール型 |
| deletedDate       | 日付    |
| usedWeb           | ブール型 |
| usedWindowsPhone  | ブール型 |
| usediOS           | ブール型 |
| usedMac           | ブール型 |
| usedAndroidPhone  | ブール型 |
| usedWindows       | ブール型 |
| reportPeriod      | String  |

## <a name="json-representation"></a>JSON 表記

リソースの JSON 表記を次に示します。

<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.teamsDeviceUsageUserDetail"
} -->

```json
{
  "reportRefreshDate": "Date", 
  "userPrincipalName": "String", 
  "lastActivityDate": "Date", 
  "isDeleted": true, 
  "deletedDate": "Date", 
  "usedWeb": true, 
  "usedWindowsPhone": true, 
  "usediOS": true, 
  "usedMac": true, 
  "usedAndroidPhone": true, 
  "usedWindows": true, 
  "reportPeriod": "String"
}
```
