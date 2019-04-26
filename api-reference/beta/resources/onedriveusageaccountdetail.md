---
title: onedrive のアカウント詳細リソースの種類
description: リソースの JSON 表記を次に示します。
localization_priority: Normal
ms.prod: sharepoint
ms.openlocfilehash: 9c13e03d1170b0ebbc53394541c4564c60c67e78
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32563547"
---
# <a name="onedriveusageaccountdetail-resource-type"></a>onedrive のアカウント詳細リソースの種類

## <a name="properties"></a>プロパティ

| プロパティ                | 型    |
| :---------------------- | :------ |
| reportrefreshdate       | Date    |
| siteUrl                 | String  |
| ownerdisplayname        | String  |
| isDeleted               | Boolean |
| lastactivitydate        | Date    |
| fileCount               | Int64   |
| activeFileCount         | Int64   |
| storageused inbytes      | Int64   |
| storageallocatedinbytes | Int64   |
| reportperiod            | String  |

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
