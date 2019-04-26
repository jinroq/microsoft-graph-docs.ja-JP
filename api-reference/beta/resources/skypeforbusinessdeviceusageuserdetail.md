---
title: skypeforbusinessdevice使い方 userdetail リソースの種類
description: リソースの JSON 表記を次に示します。
localization_priority: Normal
ms.openlocfilehash: 95f2f6cf1f3f6c54c4b6b4b39a7118cd8a94b224
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32555935"
---
# <a name="skypeforbusinessdeviceusageuserdetail-resource-type"></a>skypeforbusinessdevice使い方 userdetail リソースの種類

## <a name="properties"></a>プロパティ

| プロパティ          | 型    |
| :---------------- | :------ |
| reportrefreshdate | Date    |
| userPrincipalName | String  |
| lastactivitydate  | Date    |
| 未使用のウィンドウ       | ブール値 |
| usedWindowsPhone  | ブール値 |
| used androidphone  | ブール値 |
| usediphone        | ブール値 |
| usedipad          | ブール値 |
| reportperiod      | String  |

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
