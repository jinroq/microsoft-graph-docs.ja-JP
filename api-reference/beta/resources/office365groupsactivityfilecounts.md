---
title: office365GroupsActivityFileCounts リソースの種類
description: リソースの JSON 表記を次に示します。
ms.openlocfilehash: eb2d967108d4f75064b91670ae43fb7a2dd7ce7a
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27067668"
---
# <a name="office365groupsactivityfilecounts-resource-type"></a>office365GroupsActivityFileCounts リソースの種類

## <a name="properties"></a>プロパティ

| プロパティ          | 型   | 説明                              |
| :---------------- | :----- | ---------------------------------------- |
| reportRefreshDate | Date   | コンテンツの最新の日付。          |
| total             | Int64  | グループの SharePoint ドキュメント ライブラリ内のファイルの合計数です。 |
| アクティブです            | Int64  | 、表示されたファイルの数は、編集、共有、またはグループの SharePoint ドキュメント ライブラリに同期します。 |
| reportDate        | Date   | グループの SharePoint サイトにアクティブだったファイルの数の日付です。 |
| reportPeriod      | String | レポートの対象日数です。    |

## <a name="json-representation"></a>JSON 表記

リソースの JSON 表記を次に示します。

<!-- {

  "blockType": "resource",
  "@odata.type": "microsoft.graph.office365GroupsActivityFileCounts"
} -->

```json
{
  "reportRefreshDate": "Date", 
  "total": 1024, 
  "active": 1024, 
  "reportDate": "Date", 
  "reportPeriod": "String"
}
```
