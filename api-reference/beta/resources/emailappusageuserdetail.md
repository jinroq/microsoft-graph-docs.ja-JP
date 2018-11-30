---
title: emailAppUsageUserDetail リソースの種類
description: リソースの JSON 表記を次に示します。
ms.openlocfilehash: 951d53f7491ff7f2b7721b14ed354d770cfd1730
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27067090"
---
# <a name="emailappusageuserdetail-resource-type"></a>emailAppUsageUserDetail リソースの種類

## <a name="properties"></a>プロパティ

| プロパティ          | 型              |
| :---------------- | :---------------- |
| reportRefreshDate | Date              |
| userPrincipalName | String            |
| displayName       | String            |
| isDeleted         | ブール値           |
| deletedDate       | Date              |
| lastActivityDate  | Date              |
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
