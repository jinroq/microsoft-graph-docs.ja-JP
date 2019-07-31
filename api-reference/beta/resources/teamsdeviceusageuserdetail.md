---
title: Teamsdeviceの使い方 Userdetail リソースの種類
description: リソースの JSON 表記を次に示します。
author: nkramer
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: 5bd7443e775a8a9de0dbbc27cf8843331f8f8cb7
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "36007628"
---
# <a name="teamsdeviceusageuserdetail-resource-type"></a>Teamsdeviceの使い方 Userdetail リソースの種類

## <a name="properties"></a>プロパティ

| プロパティ          | 型    |
| :---------------- | :------ |
| reportRefreshDate | 日付    |
| userPrincipalName | String  |
| lastActivityDate  | 日付    |
| isDeleted         | Boolean |
| deletedDate       | 日付    |
| Used Web           | Boolean |
| usedWindowsPhone  | Boolean |
| usediOS           | Boolean |
| Used Mac           | Boolean |
| Used Androidphone  | Boolean |
| 未使用のウィンドウ       | Boolean |
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
