---
title: 招待メッセージの構成
description: InvitedUserMessageInfo オブジェクトを使用すると、招待メッセージを構成できます。
localization_priority: Normal
author: ''
ms.prod: ''
doc_type: resourcePageType
ms.openlocfilehash: fff33ce5ceda9ea3c60583338538a1bf502ae0f9
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "36036751"
---
# <a name="configuring-the-invitation-message"></a>招待メッセージの構成

InvitedUserMessageInfo オブジェクトを使用すると、[招待](invitation.md)メッセージを構成できます。


## <a name="properties"></a>プロパティ
| プロパティ     | 型   |説明|
|:---------------|:--------|:----------|
|ccRecipients|[Recipient](recipient.md) collection|その他の受信者に招待メッセージを送信する必要があります。 現時点では、1つの追加の受信者のみがサポートされています。|
|customizedMessageBody|String|既定のメッセージを必要としない場合に送信する、カスタマイズされたメッセージ本文。|
|messageLanguage|String|既定のメッセージを送信する言語を指定します。 CustomizedMessageBody が指定されている場合、このプロパティは無視され、customizedMessageBody を使用してメッセージが送信されます。 言語の形式は ISO 639 である必要があります。 既定値は en-us です。|

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
