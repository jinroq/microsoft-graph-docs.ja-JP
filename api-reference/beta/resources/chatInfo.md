---
title: chatInfo リソースの種類
description: マイクロソフトのチーム内のメッセージについて説明します。
ms.openlocfilehash: d7e90cf2cdf5180f6483675d919b4e635a1cd5fa
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27066478"
---
# <a name="chatinfo-resource-type"></a>chatInfo リソースの種類

> **重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。 実稼働アプリケーションでの、これらの API の使用はサポートされていません。

マイクロソフトのチーム内のメッセージについて説明します。

## <a name="properties"></a>プロパティ

| プロパティ            | 型    | 説明|
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
