---
title: chatInfo リソースの種類
description: マイクロソフトのチーム内のメッセージについて説明します。
author: VinodRavichandran
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: 840073d6882d6665be60e7386eaafe3168b70dbe
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/12/2019
ms.locfileid: "27940751"
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
