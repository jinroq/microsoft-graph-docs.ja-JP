---
title: Emailappの User計数リソースの種類
description: リソースの JSON 表記を次に示します。
localization_priority: Normal
author: angelgolfer-ms
ms.prod: outlook
doc_type: resourcePageType
ms.openlocfilehash: d8af9e9337c68fcd4434514b85fa9217c79add26
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "35972174"
---
# <a name="emailappusageusercounts-resource-type"></a>Emailappの User計数リソースの種類

## <a name="properties"></a>プロパティ

| プロパティ          | 型   |
| :---------------- | :----- |
| reportRefreshDate | 日付   |
| mailForMac        | Int64  |
| outlookForMac     | Int64  |
| outlookForWindows | Int64  |
| outlookForMobile  | Int64  |
| otherForMobile    | Int64  |
| outlookForWeb     | Int64  |
| pop3App           | Int64  |
| imap4App          | Int64  |
| smtpApp           | Int64  |
| reportDate        | 日付   |
| reportPeriod      | String |

## <a name="json-representation"></a>JSON 表記

リソースの JSON 表記を次に示します。

<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.emailAppUsageUserCounts"
} -->

```json
{
  "reportRefreshDate": "Date", 
  "mailForMac": 1024, 
  "outlookForMac": 1024, 
  "outlookForWindows": 1024, 
  "outlookForMobile": 1024, 
  "otherForMobile": 1024, 
  "outlookForWeb": 1024, 
  "pop3App": 1024, 
  "imap4App": 1024, 
  "smtpApp": 1024, 
  "reportDate": "Date", 
  "reportPeriod": "String"
}
```
