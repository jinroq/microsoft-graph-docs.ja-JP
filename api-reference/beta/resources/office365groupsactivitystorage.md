---
title: office365GroupsActivityStorage リソースの種類
description: リソースの JSON 表記を次に示します。
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
ms.openlocfilehash: 0485fd95046bc83350983bc1333dba83c79139d6
ms.sourcegitcommit: 66066b71d353fd7c2481d43b1dba2c33390eee61
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/26/2019
ms.locfileid: "29576382"
---
# <a name="office365groupsactivitystorage-resource-type"></a>office365GroupsActivityStorage リソースの種類

## <a name="properties"></a>プロパティ

| プロパティ                  | 型   | 説明                              |
| :------------------------ | :----- | ---------------------------------------- |
| reportRefreshDate         | 日付   | コンテンツの最新の日付。          |
| mailboxStorageUsedInBytes | Int64  | ストレージ グループのメールボックスで使用されています。       |
| siteStorageUsedInBytes    | Int64  | SharePoint ドキュメント ライブラリで使用されている記憶域。 |
| reportDate                | 日付   | Exchange と SharePoint のスナップショットの日付には、記憶域が使用されます。 |
| reportPeriod              | String | レポートの対象日数です。    |

## <a name="json-representation"></a>JSON 表記

リソースの JSON 表記を次に示します。

<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.office365GroupsActivityStorage"
} -->

```json
{
  "reportRefreshDate": "Date", 
  "mailboxStorageUsedInBytes": 1024, 
  "siteStorageUsedInBytes": 1024, 
  "reportDate": "Date", 
  "reportPeriod": "String"
}
```
