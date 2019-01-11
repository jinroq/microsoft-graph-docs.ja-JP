---
title: chatInfo リソースの種類
description: マイクロソフトのチーム内のメッセージについて説明します。
author: VinodRavichandran
localization_priority: Normal
ms.openlocfilehash: c2cc0dd288abdab7852017600c4c55b9a40b0aa7
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/11/2019
ms.locfileid: "27852942"
---
# <a name="chatinfo-resource-type"></a>chatInfo リソースの種類

> **重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。 実稼働アプリケーションでの、これらの API の使用はサポートされていません。

マイクロソフトのチーム内のメッセージについて説明します。

## <a name="properties"></a>プロパティ

| プロパティ            | 種類    | 説明|
|:--------------------|:--------|:-----------|
| メッセージ Id           | String  | マイクロソフト チームのチャネルでのメッセージの一意の識別子です。 |
| replyChainMessageId | String  | 返信メッセージの ID です。 |
| スレッド Id            | String  | マイクロソフトのチームでのスレッドの一意の識別子です。 |

## <a name="json-representation"></a>JSON 表記

リソースの JSON 表記を次に示します。

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.chatInfo"
}-->
```json
{
  "messageId": "String",
  "replyChainMessageId": "String",
  "threadId": "String"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "chatInfo resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
