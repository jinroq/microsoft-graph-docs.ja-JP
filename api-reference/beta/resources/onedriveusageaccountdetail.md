---
title: oneDriveUsageAccountDetail リソースの種類
description: リソースの JSON 表記を次に示します。
ms.openlocfilehash: 4b80ebc24aa45be0368dbb59d6d3e99e7adacc8c
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27071365"
---
# <a name="onedriveusageaccountdetail-resource-type"></a>oneDriveUsageAccountDetail リソースの種類

## <a name="properties"></a>プロパティ

| プロパティ                | 型    |
| :---------------------- | :------ |
| reportRefreshDate       | Date    |
| siteUrl                 | String  |
| ownerDisplayName        | String  |
| isDeleted               | ブール値 |
| lastActivityDate        | Date    |
| fileCount               | Int64   |
| activeFileCount         | Int64   |
| storageUsedInBytes      | Int64   |
| storageAllocatedInBytes | Int64   |
| reportPeriod            | String  |

## <a name="json-representation"></a>JSON 表記

リソースの JSON 表記を次に示します。

<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.oneDriveUsageAccountDetail"
} -->

```json
{
  "reportRefreshDate": "Date", 
  "siteUrl": "String", 
  "ownerDisplayName": "String", 
  "isDeleted": true, 
  "lastActivityDate": "Date", 
  "fileCount": 1024, 
  "activeFileCount": 1024, 
  "storageUsedInBytes": 1024, 
  "storageAllocatedInBytes": 1024, 
  "reportPeriod": "String"
}
```
