---
title: office365GroupsActivityStorage リソースの種類
description: リソースの JSON 表記を次に示します。
localization_priority: Normal
ms.openlocfilehash: 9824d3d172a8578f8a25a049c2d0d3b407bbc47e
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/11/2019
ms.locfileid: "27862252"
---
# <a name="office365groupsactivitystorage-resource-type"></a>office365GroupsActivityStorage リソースの種類

## <a name="properties"></a>プロパティ

| プロパティ                  | 種類   | 説明                              |
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
