---
title: yammerDeviceUsageUserDetail リソースの種類
description: リソースの JSON 表記を次に示します。
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
doc_type: resourcePageType
ms.openlocfilehash: 083ace4b10b24e8e5de5d287ddf418d93658c879
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "36006982"
---
# <a name="yammerdeviceusageuserdetail-resource-type"></a>yammerDeviceUsageUserDetail リソースの種類

## <a name="properties"></a>プロパティ

| プロパティ          | 型    |
| :---------------- | :------ |
| reportRefreshDate | 日付    |
| userPrincipalName | String  |
| displayName       | 文字列  |
| userState         | String  |
| stateChangeDate   | 日付    |
| lastActivityDate  | 日付    |
| Used Web           | Boolean |
| usedWindowsPhone  | Boolean |
| Used Androidphone  | Boolean |
| usediPhone        | Boolean |
| usediPad          | Boolean |
| usedOthers        | Boolean |
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
