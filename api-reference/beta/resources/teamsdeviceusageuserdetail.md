---
title: teamsDeviceUsageUserDetail リソースの種類
description: リソースの JSON 表記を次に示します。
ms.openlocfilehash: 4eeec5f07a0a604249617ac87a62ea12b4052395
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27073764"
---
# <a name="teamsdeviceusageuserdetail-resource-type"></a>teamsDeviceUsageUserDetail リソースの種類

## <a name="properties"></a>プロパティ

| プロパティ          | 型    |
| :---------------- | :------ |
| reportRefreshDate | Date    |
| userPrincipalName | String  |
| lastActivityDate  | Date    |
| isDeleted         | ブール値 |
| deletedDate       | Date    |
| usedWeb           | ブール値 |
| usedWindowsPhone  | ブール値 |
| usediOS           | ブール値 |
| usedMac           | ブール値 |
| usedAndroidPhone  | ブール値 |
| usedWindows       | ブール値 |
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
