---
title: office365GroupsActivityStorage リソースの種類
description: リソースの JSON 表記を次に示します。
ms.openlocfilehash: 23ff4d112373f52c4c19d6631ac89bac22399b29
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27073258"
---
# <a name="office365groupsactivitystorage-resource-type"></a>office365GroupsActivityStorage リソースの種類

## <a name="properties"></a>プロパティ

| プロパティ                  | 型   | 説明                              |
| :------------------------ | :----- | ---------------------------------------- |
| reportRefreshDate         | Date   | コンテンツの最新の日付。          |
| mailboxStorageUsedInBytes | Int64  | ストレージ グループのメールボックスで使用されています。       |
| siteStorageUsedInBytes    | Int64  | SharePoint ドキュメント ライブラリで使用されている記憶域。 |
| reportDate                | Date   | Exchange と SharePoint のスナップショットの日付には、記憶域が使用されます。 |
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
