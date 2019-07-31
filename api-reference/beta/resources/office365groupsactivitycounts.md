---
title: office365GroupsActivityCounts リソースの種類
description: リソースの JSON 表記を次に示します。
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
doc_type: resourcePageType
ms.openlocfilehash: c1e441b142ef27abbdde4ac613ef8d75848f5001
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "35966553"
---
# <a name="office365groupsactivitycounts-resource-type"></a>office365GroupsActivityCounts リソースの種類

## <a name="properties"></a>プロパティ

| プロパティ               | 型   | 説明                              |
| :--------------------- | :----- | ---------------------------------------- |
| reportRefreshDate      | 日付   | コンテンツの最新の日付。          |
| exchangeEmailsReceived | Int64  | グループメールボックスで受信したメールの数。 |
| yammerMessagesPosted   | Int64  | Yammer グループに投稿されたメッセージの数。 |
| yammerMessagesRead     | Int64  | Yammer グループで読み取られたメッセージの数。 |
| yammerMessagesLiked    | Int64  | Yammer グループに賛同されたメッセージの数。 |
| reportDate             | 日付   | グループメールボックスに送信されたメールの数またはメッセージ数が Yammer グループで投稿、読み取り、または賛同された日付 |
| reportPeriod           | String | レポートの対象となる日数を指定します。    |

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
