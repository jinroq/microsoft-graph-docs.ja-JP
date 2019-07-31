---
title: mailboxUsageDetail リソースの種類
description: リソースの JSON 表記を次に示します。
localization_priority: Normal
author: angelgolfer-ms
ms.prod: outlook
doc_type: resourcePageType
ms.openlocfilehash: e630a64e7ece98d956a5f3821ec92413512fc7e4
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "35966938"
---
# <a name="mailboxusagedetail-resource-type"></a>mailboxUsageDetail リソースの種類

## <a name="properties"></a>プロパティ

| プロパティ                        | 型    |
| :------------------------------ | :------ |
| reportRefreshDate               | 日付    |
| userPrincipalName               | String  |
| displayName                     | 文字列  |
| isDeleted                       | Boolean |
| deletedDate                     | 日付    |
| createdDate                     | 日付    |
| lastActivityDate                | 日付    |
| itemCount                       | Int64   |
| Storageused Inbytes              | Int64   |
| deletedItemCount                | Int64   |
| deletedItemSizeInBytes          | Int64   |
| Warnings Ewarnings Quot/バイト        | Int64   |
| prohibitSendQuotaInBytes        | Int64   |
| prohibitSendReceiveQuotaInBytes | Int64   |
| reportPeriod                    | String  |

## <a name="json-representation"></a>JSON 表記

リソースの JSON 表記を次に示します。

<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.mailboxUsageDetail"
} -->

```json
{
  "reportRefreshDate": "Date", 
  "userPrincipalName": "String", 
  "displayName": "String", 
  "isDeleted": true, 
  "deletedDate": "Date", 
  "createdDate": "Date", 
  "lastActivityDate": "Date", 
  "itemCount": 1024, 
  "storageUsedInBytes": 1024, 
  "deletedItemCount": 1024,
  "deletedItemSizeInBytes": 1024, 
  "issueWarningQuotaInBytes": 1024, 
  "prohibitSendQuotaInBytes": 1024, 
  "prohibitSendReceiveQuotaInBytes": 1024, 
  "reportPeriod": "String"
}
```
