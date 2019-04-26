---
title: teamsdeviceの使い方 userdetail リソースの種類
description: リソースの JSON 表記を次に示します。
author: nkramer
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: 8cdd2fe1a212bb1d36846b80fc1b558c576deb47
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32553604"
---
# <a name="teamsdeviceusageuserdetail-resource-type"></a>teamsdeviceの使い方 userdetail リソースの種類

## <a name="properties"></a>プロパティ

| プロパティ          | 型    |
| :---------------- | :------ |
| reportrefreshdate | Date    |
| userPrincipalName | String  |
| lastactivitydate  | Date    |
| isDeleted         | ブール値 |
| deletedDate       | Date    |
| used web           | ブール値 |
| usedWindowsPhone  | ブール値 |
| usedios           | ブール値 |
| used mac           | ブール値 |
| used androidphone  | ブール値 |
| 未使用のウィンドウ       | ブール値 |
| reportperiod      | String  |

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
