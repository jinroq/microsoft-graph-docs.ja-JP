---
title: sharepointsiteの詳細リソースの種類
description: リソースの JSON 表記を次に示します。
localization_priority: Normal
ms.prod: sharepoint
ms.openlocfilehash: e0827f6b6b991136198fc174e01e7d0e1f91c259
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32583999"
---
# <a name="sharepointsiteusagedetail-resource-type"></a>sharepointsiteの詳細リソースの種類

## <a name="properties"></a>プロパティ

| プロパティ                | 型    |
| :---------------------- | :------ |
| reportrefreshdate       | Date    |
| siteId                  | Guid  |
| siteUrl                 | String  |
| ownerdisplayname        | String  |
| isDeleted               | Boolean |
| lastactivitydate        | Date    |
| fileCount               | Int64   |
| activeFileCount         | Int64   |
| pageviewcount           | Int64   |
| visitedPageCount        | Int64   |
| storageused inbytes      | Int64   |
| storageallocatedinbytes | Int64   |
| rootwebtemplate         | String  |
| reportperiod            | String  |

## <a name="json-representation"></a>JSON 表記

リソースの JSON 表記を次に示します。

<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.sharePointSiteUsageDetail"
} -->

```json
{
  "reportRefreshDate": "Date", 
  "siteId": "Guid", 
  "siteUrl": "String", 
  "ownerDisplayName": "String", 
  "isDeleted": true, 
  "lastActivityDate": "Date", 
  "fileCount": 1024, 
  "activeFileCount": 1024, 
  "pageViewCount": 1024, 
  "visitedPageCount": 1024, 
  "storageUsedInBytes": 1024, 
  "storageAllocatedInBytes": 1024, 
  "rootWebTemplate": "String", 
  "reportPeriod": "String"
}
```
