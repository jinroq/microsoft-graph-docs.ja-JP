---
title: office365GroupsActivityCounts リソースの種類
description: リソースの JSON 表記を次に示します。
localization_priority: Normal
ms.prod: reports
ms.openlocfilehash: 7e9f983d131d3b213689a48e10d8d23d3f99085b
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/12/2019
ms.locfileid: "27968289"
---
# <a name="office365groupsactivitycounts-resource-type"></a>office365GroupsActivityCounts リソースの種類

## <a name="properties"></a>プロパティ

| プロパティ               | 種類   | 説明                              |
| :--------------------- | :----- | ---------------------------------------- |
| reportRefreshDate      | 日付   | コンテンツの最新の日付。          |
| exchangeEmailsReceived | Int64  | グループのメールボックスで受信したメールの数です。 |
| yammerMessagesPosted   | Int64  | Yammer のグループに投稿されたメッセージの数です。 |
| yammerMessagesRead     | Int64  | Yammer グループでメッセージの数を読み取る。 |
| yammerMessagesLiked    | Int64  | Yammer グループに賛同のメッセージの数です。 |
| reportDate             | 日付   | メールの数は、グループのメールボックスに送信されたまたはメッセージの数が転記された日付、または、Yammer グループで気に入られました |
| reportPeriod           | String | レポートの対象日数です。    |

## <a name="json-representation"></a>JSON 表記

リソースの JSON 表記を次に示します。

<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.office365GroupsActivityCounts"
} -->

```json
{
  "reportRefreshDate": "Date", 
  "exchangeEmailsReceived": 1024, 
  "yammerMessagesPosted": 1024, 
  "yammerMessagesRead": 1024, 
  "yammerMessagesLiked": 1024, 
  "reportDate": "Date", 
  "reportPeriod": "String"
}
```
