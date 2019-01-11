---
title: emailAppUsageUserDetail リソースの種類
description: リソースの JSON 表記を次に示します。
localization_priority: Normal
ms.openlocfilehash: 9f1748d6ae3b313fd9f3a87cc211858b5b876b9a
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/11/2019
ms.locfileid: "27858948"
---
# <a name="emailappusageuserdetail-resource-type"></a>emailAppUsageUserDetail リソースの種類

## <a name="properties"></a>プロパティ

| プロパティ          | 種類              |
| :---------------- | :---------------- |
| reportRefreshDate | 日付              |
| userPrincipalName | String            |
| displayName       | String            |
| isDeleted         | ブール型           |
| deletedDate       | 日付              |
| lastActivityDate  | 日付              |
| mailForMac        | String コレクション |
| outlookForMac     | String コレクション |
| outlookForWindows | String コレクション |
| outlookForMobile  | String コレクション |
| otherForMobile    | String コレクション |
| outlookForWeb     | String コレクション |
| pop3App           | String コレクション |
| imap4App          | String コレクション |
| smtpApp           | String コレクション |
| reportPeriod      | String            |

## <a name="json-representation"></a>JSON 表記

リソースの JSON 表記を次に示します。

<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.emailAppUsageUserDetail"
} -->

```json
{
  "reportRefreshDate": "Date", 
  "userPrincipalName": "String", 
  "displayName": "String", 
  "isDeleted": true, 
  "deletedDate": "Date", 
  "lastActivityDate": "Date", 
  "mailForMac": ["String"], 
  "outlookForMac": ["String"], 
  "outlookForWindows": ["String"], 
  "outlookForMobile": ["String"], 
  "otherForMobile": ["String"], 
  "outlookForWeb": ["String"], 
  "pop3App": ["String"], 
  "imap4App": ["String"], 
  "smtpApp": ["String"], 
  "reportPeriod": "String"
}
```
