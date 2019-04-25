---
title: office365GroupsActivityCounts リソースの種類
description: リソースの JSON 表記を次に示します。
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
ms.openlocfilehash: c94e79f688e117960b3a8a0f2c9888a908634a82
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32581724"
---
# <a name="office365groupsactivitycounts-resource-type"></a>office365GroupsActivityCounts リソースの種類

## <a name="properties"></a>プロパティ

| プロパティ               | 型   | 説明                              |
| :--------------------- | :----- | ---------------------------------------- |
| reportrefreshdate      | Date   | コンテンツの最新の日付。          |
| exchangeEmailsReceived | Int64  | グループメールボックスで受信したメールの数。 |
| yammerMessagesPosted   | Int64  | Yammer グループに投稿されたメッセージの数。 |
| yammerMessagesRead     | Int64  | Yammer グループで読み取られたメッセージの数。 |
| yammerMessagesLiked    | Int64  | Yammer グループに賛同されたメッセージの数。 |
| reportDate             | Date   | グループメールボックスに送信されたメールの数またはメッセージ数が Yammer グループで投稿、読み取り、または賛同された日付 |
| reportperiod           | String | レポートの対象となる日数を指定します。    |

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
