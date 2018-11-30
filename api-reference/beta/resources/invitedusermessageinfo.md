---
title: 招待メッセージの構成
description: invitedUserMessageInfo オブジェクトでは、招待メッセージを構成できます。
ms.openlocfilehash: 326ca6654fd30da9c36022424b48c4a8f7b82ffe
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27068180"
---
# <a name="configuring-the-invitation-message"></a>招待メッセージの構成

> **重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。 実稼働アプリケーションでの、これらの API の使用はサポートされていません。

invitedUserMessageInfo オブジェクトでは、[招待](invitation.md)メッセージを構成できます。


## <a name="properties"></a>プロパティ
| プロパティ     | 型   |説明|
|:---------------|:--------|:----------|
|ccRecipients|[Recipients](recipient.md)|招待メッセージの送信先にする必要がある追加の受信者。現在、サポートされている追加の受信者は 1 人のみです。|
|customizedMessageBody|String|既定のメッセージを使用しない場合に送信するカスタマイズされたメッセージ本文。|
|messageLanguage|String|既定のメッセージを送信する言語。customizedMessageBody が指定されている場合、このプロパティは無視され、メッセージは ustomizedMessageBody を使用して送信されます。言語書式は ISO 639 である必要があります。既定では ja-JP です。|

## <a name="json-representation"></a>JSON 表記
以下は、リソースの JSON 表記です

<!-- {"blockType": "resource", "@odata.type": "microsoft.graph.invitedUserMessageInfo"} -->
```json
{
  "ccRecipients": [ {"@odata.type": "microsoft.graph.recipient"} ],
  "customizedMessageBody": "string",
  "messageLanguage": "string"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2016-22-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "invitedUserMessageInfo resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
