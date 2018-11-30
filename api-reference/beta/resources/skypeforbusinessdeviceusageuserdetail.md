---
title: skypeForBusinessDeviceUsageUserDetail リソースの種類
description: リソースの JSON 表記を次に示します。
ms.openlocfilehash: b62920d124fd52e0f653c128eeb0956cdfe0c680
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27068048"
---
# <a name="skypeforbusinessdeviceusageuserdetail-resource-type"></a>skypeForBusinessDeviceUsageUserDetail リソースの種類

## <a name="properties"></a>プロパティ

| プロパティ          | 型    |
| :---------------- | :------ |
| reportRefreshDate | Date    |
| userPrincipalName | String  |
| lastActivityDate  | Date    |
| usedWindows       | ブール値 |
| usedWindowsPhone  | ブール値 |
| usedAndroidPhone  | ブール値 |
| usediPhone        | ブール値 |
| usediPad          | ブール値 |
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
