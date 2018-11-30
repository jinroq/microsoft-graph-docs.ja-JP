---
title: yammerDeviceUsageUserDetail リソースの種類
description: リソースの JSON 表記を次に示します。
ms.openlocfilehash: 8812b61d974815fd1cdf1bbe1549a21193e5a2f4
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27073767"
---
# <a name="yammerdeviceusageuserdetail-resource-type"></a>yammerDeviceUsageUserDetail リソースの種類

## <a name="properties"></a>プロパティ

| プロパティ          | 型    |
| :---------------- | :------ |
| reportRefreshDate | Date    |
| userPrincipalName | String  |
| displayName       | String  |
| userState         | String  |
| stateChangeDate   | Date    |
| lastActivityDate  | Date    |
| usedWeb           | ブール値 |
| usedWindowsPhone  | ブール値 |
| usedAndroidPhone  | ブール値 |
| usediPhone        | ブール値 |
| usediPad          | ブール値 |
| usedOthers        | ブール値 |
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
