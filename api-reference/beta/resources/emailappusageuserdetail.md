---
title: emailapp使い方 userdetail リソースの種類
description: リソースの JSON 表記を次に示します。
localization_priority: Normal
author: angelgolfer-ms
ms.prod: outlook
ms.openlocfilehash: 1ebc99f25bf0b16343f48686496c1dbd7d329e65
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32542840"
---
# <a name="emailappusageuserdetail-resource-type"></a>emailapp使い方 userdetail リソースの種類

## <a name="properties"></a>プロパティ

| プロパティ          | 型              |
| :---------------- | :---------------- |
| reportrefreshdate | Date              |
| userPrincipalName | String            |
| displayName       | String            |
| isDeleted         | ブール値           |
| deletedDate       | Date              |
| lastactivitydate  | Date              |
| mailformac        | String collection |
| outlookformac     | String collection |
| outlookforwindows | String collection |
| outlookformobile  | String collection |
| otherformobile    | String collection |
| outlookforweb     | String collection |
| pop3App           | String collection |
| imap4App          | String collection |
| smtpApp           | String collection |
| reportperiod      | String            |

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
