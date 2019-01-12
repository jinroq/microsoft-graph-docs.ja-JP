---
title: office365GroupsActivityGroupCounts リソースの種類
description: リソースの JSON 表記を次に示します。
localization_priority: Normal
ms.prod: reports
ms.openlocfilehash: d3c1272f9bd99c3e7ee0f29a4c303e1c8ca95525
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/12/2019
ms.locfileid: "27975884"
---
# <a name="office365groupsactivitygroupcounts-resource-type"></a>office365GroupsActivityGroupCounts リソースの種類

## <a name="properties"></a>プロパティ

| プロパティ          | 種類   | 説明                              |
| :---------------- | :----- | ---------------------------------------- |
| reportRefreshDate | 日付   | コンテンツの最新の日付。          |
| total             | Int64  | グループの合計数です。              |
| アクティブです            | Int64  | アクティブなグループの数。 グループは、次のいずれかが発生した場合は、アクティブと見なされます: グループのメールボックスに受信した電子メールです。ユーザーを表示、編集、共有、または SharePoint ドキュメント ライブラリ内のファイルの同期ユーザーが SharePoint ページを表示ユーザーは、投稿、読み取り、または、Yammer グループ内のメッセージを気に入られました。 |
| reportDate        | 日付   | いくつかのグループにアクティブだった日付。 |
| reportPeriod      | String | レポートの対象日数です。    |

## <a name="json-representation"></a>JSON 表記

リソースの JSON 表記を次に示します。

<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.office365GroupsActivityGroupCounts"
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
