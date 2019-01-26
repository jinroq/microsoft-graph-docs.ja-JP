---
title: office365GroupsActivityCounts リソースの種類
description: リソースの JSON 表記を次に示します。
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
ms.openlocfilehash: c94e79f688e117960b3a8a0f2c9888a908634a82
ms.sourcegitcommit: 66066b71d353fd7c2481d43b1dba2c33390eee61
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/26/2019
ms.locfileid: "29572333"
---
# <a name="office365groupsactivitycounts-resource-type"></a>office365GroupsActivityCounts リソースの種類

## <a name="properties"></a>プロパティ

| プロパティ               | 型   | 説明                              |
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
