---
title: office365GroupsActivityStorage リソースの種類
description: リソースの JSON 表記を次に示します。
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
doc_type: resourcePageType
ms.openlocfilehash: a3168ad417f246017ba1018aca265ec0363c951e
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "36009462"
---
# <a name="office365groupsactivitystorage-resource-type"></a>office365GroupsActivityStorage リソースの種類

## <a name="properties"></a>プロパティ

| プロパティ                  | 型   | 説明                              |
| :------------------------ | :----- | ---------------------------------------- |
| reportRefreshDate         | 日付   | コンテンツの最新の日付。          |
| mailboxStorageUsedInBytes | Int64  | グループメールボックスで使用されている記憶域。       |
| Sitestorageused Inbytes    | Int64  | SharePoint ドキュメントライブラリで使用されているストレージ。 |
| reportDate                | 日付   | Exchange および SharePoint で使用されたストレージのスナップショット日付。 |
| reportPeriod              | String | レポートの対象となる日数を指定します。    |

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
