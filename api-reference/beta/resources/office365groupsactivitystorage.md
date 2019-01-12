---
title: office365GroupsActivityStorage リソースの種類
description: リソースの JSON 表記を次に示します。
localization_priority: Normal
ms.prod: reports
ms.openlocfilehash: 180e60a52b397f969aa10cee5bc27bba934ad1e4
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/12/2019
ms.locfileid: "27944454"
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
