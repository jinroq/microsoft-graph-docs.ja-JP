---
title: chatmessagereaction リソースの種類
description: 'chatmessage エンティティへの反応を表します。 '
localization_priority: Normal
ms.openlocfilehash: 5020653ef02c1604aece46f3ff2c7ea1c82a75ec
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32460640"
---
# <a name="chatmessagereaction-resource-type"></a>chatmessagereaction リソースの種類

[chatmessage](chatmessage.md)エンティティへの反応を表します。 

型`chatMessageReaction`のエンティティは、 [chatmessage](chatmessage.md)エンティティの一部として、 [Get channel messages](../api/channel-get-message.md) API の一部として返されます。

## <a name="properties"></a>プロパティ
| プロパティ     | 型   |説明|
|:---------------|:--------|:----------|
|reactiontype|string| 反応の種類。 計画される値は次のとおりです。 <br><ul><li>like-メッセージと同じですが、この場合、コンテンツは空白になります。</li><li>絵文字と絵文字の反応。 コンテンツは絵文字の unicode 値に設定されています。</li><li>label-コンテンツはラベル内の文字列に設定されます。</li></ul>|
|createdDateTime|dateTimeOffset|ISO-8601 形式のルートメッセージの UTC タイムスタンプ。|
|user|identitySet|メッセージに reacted したユーザー。|

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
