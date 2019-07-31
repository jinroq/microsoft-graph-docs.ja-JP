---
title: Emailapp使い方 Userdetail リソースの種類
description: リソースの JSON 表記を次に示します。
localization_priority: Normal
author: angelgolfer-ms
ms.prod: outlook
doc_type: resourcePageType
ms.openlocfilehash: ae0409124569f4318df94f97729402a91d4b8e45
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "35972146"
---
# <a name="emailappusageuserdetail-resource-type"></a>Emailapp使い方 Userdetail リソースの種類

## <a name="properties"></a>プロパティ

| プロパティ          | 型              |
| :---------------- | :---------------- |
| reportRefreshDate | 日付              |
| userPrincipalName | String            |
| displayName       | 文字列            |
| isDeleted         | Boolean           |
| deletedDate       | 日付              |
| lastActivityDate  | 日付              |
| mailForMac        | 文字列コレクション |
| outlookForMac     | 文字列コレクション |
| outlookForWindows | 文字列コレクション |
| outlookForMobile  | 文字列コレクション |
| otherForMobile    | 文字列コレクション |
| outlookForWeb     | 文字列コレクション |
| pop3App           | 文字列コレクション |
| imap4App          | 文字列コレクション |
| smtpApp           | 文字列コレクション |
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
