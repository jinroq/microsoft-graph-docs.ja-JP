---
title: emailAppUsageUserDetail リソースの種類
description: リソースの JSON 表記を次に示します。
localization_priority: Normal
author: angelgolfer-ms
ms.prod: outlook
ms.openlocfilehash: 1ebc99f25bf0b16343f48686496c1dbd7d329e65
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/12/2019
ms.locfileid: "27977655"
---
# <a name="emailappusageuserdetail-resource-type"></a>emailAppUsageUserDetail リソースの種類

## <a name="properties"></a>プロパティ

| プロパティ          | 型              |
| :---------------- | :---------------- |
| reportRefreshDate | 日付              |
| userPrincipalName | String            |
| displayName       | String            |
| isDeleted         | Boolean           |
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
