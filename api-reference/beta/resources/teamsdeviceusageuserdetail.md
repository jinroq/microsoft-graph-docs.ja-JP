---
title: teamsDeviceUsageUserDetail リソースの種類
description: リソースの JSON 表記を次に示します。
author: nkramer
ms.openlocfilehash: 1947b66a59190945e5a6b823b47ef8df7d02683a
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 12/18/2018
ms.locfileid: "27329002"
---
# <a name="teamsdeviceusageuserdetail-resource-type"></a>teamsDeviceUsageUserDetail リソースの種類

## <a name="properties"></a>Properties

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
