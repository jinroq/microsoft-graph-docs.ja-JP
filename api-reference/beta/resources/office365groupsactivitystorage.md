---
title: office365GroupsActivityStorage リソースの種類
description: リソースの JSON 表記を次に示します。
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
ms.openlocfilehash: 0485fd95046bc83350983bc1333dba83c79139d6
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32505551"
---
# <a name="office365groupsactivitystorage-resource-type"></a>office365GroupsActivityStorage リソースの種類

## <a name="properties"></a>プロパティ

| プロパティ                  | 型   | 説明                              |
| :------------------------ | :----- | ---------------------------------------- |
| reportrefreshdate         | Date   | コンテンツの最新の日付。          |
| mailboxStorageUsedInBytes | Int64  | グループメールボックスで使用されている記憶域。       |
| sitestorageused inbytes    | Int64  | SharePoint ドキュメントライブラリで使用されているストレージ。 |
| reportDate                | Date   | Exchange および SharePoint で使用されたストレージのスナップショット日付。 |
| reportperiod              | String | レポートの対象となる日数を指定します。    |

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
