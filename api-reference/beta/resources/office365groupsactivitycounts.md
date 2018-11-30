---
title: office365GroupsActivityCounts リソースの種類
description: リソースの JSON 表記を次に示します。
ms.openlocfilehash: 4f3a5bf02f5f477ebab036fc9afa5d35a8061138
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27073264"
---
# <a name="office365groupsactivitycounts-resource-type"></a>office365GroupsActivityCounts リソースの種類

## <a name="properties"></a>プロパティ

| プロパティ               | 型   | 説明                              |
| :--------------------- | :----- | ---------------------------------------- |
| reportRefreshDate      | Date   | コンテンツの最新の日付。          |
| exchangeEmailsReceived | Int64  | グループのメールボックスで受信したメールの数です。 |
| yammerMessagesPosted   | Int64  | Yammer のグループに投稿されたメッセージの数です。 |
| yammerMessagesRead     | Int64  | Yammer グループでメッセージの数を読み取る。 |
| yammerMessagesLiked    | Int64  | Yammer グループに賛同のメッセージの数です。 |
| reportDate             | Date   | メールの数は、グループのメールボックスに送信されたまたはメッセージの数が転記された日付、または、Yammer グループで気に入られました |
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
