---
title: chatMessageReaction リソースの種類
description: 'ChatMessage エンティティへの対応を表します。 '
ms.openlocfilehash: 1ad1f7948405a8891ec9aa13065b71108e9c47c5
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27074185"
---
# <a name="chatmessagereaction-resource-type"></a>chatMessageReaction リソースの種類

[ChatMessage](chatmessage.md)エンティティへの対応を表します。 

エンティティの種類の`chatMessageReaction` [chatMessage](chatmessage.md)エンティティの一部として、[チャネルのメッセージを取得する](../api/channel-get-message.md)API の一部として返されます。

## <a name="properties"></a>プロパティ
| プロパティ     | 型   |説明|
|:---------------|:--------|:----------|
|reactionType|文字列| 反応の型。 計画値は次のとおりです。 <br><ul><li>-のようなメッセージのようなコンテンツは空白でもです。</li><li>Emoji の Emoji の反力です。 コンテンツは、絵文字の unicode 値に設定されています。</li><li>ラベルの内容は、ラベル内の文字列に設定されます。</li></ul>|
|createdDateTime|dateTimeOffset|ISO 8601 形式のメッセージ ルートの utc 形式のタイムスタンプです。|
|user|identitySet|メッセージに反応するユーザーです。|

## <a name="json-representation"></a>JSON 表記

リソースの JSON 表記を次に示します。

<!-- {
  "blockType": "resource",
  "optionalProperties": [
    "content"
  ],
  "baseType": "microsoft.graph.entity",
  "@odata.type": "microsoft.graph.chatMessageReaction"
}-->

```json
{
  "reactionType": "string ",
  "createdDateTime": "string (timestamp)",
  "user": {"@odata.type": "microsoft.graph.identitySet"}
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "chat message reaction resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
