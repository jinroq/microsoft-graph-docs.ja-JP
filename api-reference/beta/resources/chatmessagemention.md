---
title: chatMessageMention リソースの種類
description: 'ChatMessage エンティティ内のメンションを表します。 メンションは、ユーザー、チーム、ボット、またはチャネルにすることができます。 '
localization_priority: Normal
author: nkramer
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: 130b1d536c881991a54e5b6fd06aee2f3f59483a
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "36012962"
---
# <a name="chatmessagemention-resource-type"></a>chatMessageMention リソースの種類

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

[Chatmessage](chatmessage.md)エンティティ内のメンションを表します。 メンションは、[ユーザー](user.md)、[チーム](team.md)、ボット、または[チャネル](channel.md)にすることができます。 

1つまたは複数のメンションを含む**Chatmessage**オブジェクトでは、メッセージ本文の**コンテンツ**プロパティは、HTML でチャットメッセージを表します。 各メンションの**mentionText**を HTML `at`要素で囲みます。属性は`id` 、メンションの**id**プロパティに対応しています。

一例として、チャットメッセージには2つのメンションが含まれており、それぞれに "Megan" と "Alex" という説明文があります。 Body**コンテンツ**プロパティは、 `at` 2 つのメンションの要素を次のように指定します。

``` json
"body": {
    "contentType": "html",
    "content": "<div><div>Ah, <at id=\"0\">Megan</at>, <at id=\"1\">Alex</at>, I saw them in a separate folder. Thanks!</div>\n</div>"
}
```

**コンテンツ**プロパティの最初のメンションには、0 `id`の HTML 属性があります。 これは、 **chatMessageMention**の最初のインスタンスの**id**プロパティに対応します。これは0でもあります。

2番目のメン`id`ションの属性は1で、2番目のインスタンスの**id**プロパティと一致します。1は1です。

この例の詳細については、「 [List channel message リプライ](../api/channel-list-messagereplies.md#example)」を参照してください。

## <a name="properties"></a>プロパティ
| プロパティ     | 型   |説明|
|:---------------|:--------|:----------|
|id|Int32|指定した**Chatmessage**で言及されているエンティティのインデックスです。 メッセージ本文の対応する`<at id="{index}">`タグの {index} 値と一致します。|
|mentionText|string|メンションを表すために使用される文字列。 たとえば、ユーザーの表示名、チーム名。|
|明記|[identitySet](identityset.md)|前述したエンティティ (ユーザー、アプリケーション、チーム、またはチャネル)。  @Mentioned されたチャネルまたはチームの場合は、チーム/チャネルの ID を提供する**会話**プロパティと、チームまたはチャネルのいずれかを表す**conversationIdentityType**プロパティが含まれます。|


## <a name="json-representation"></a>JSON 表記

リソースの JSON 表記を次に示します。

<!-- {
  "blockType": "resource",
  "baseType": "microsoft.graph.entity",
  "@odata.type": "microsoft.graph.chatMessageMention"
}-->

```json
{
  "id": 1024,
  "mentionText": "string",
  "mentioned": {"@odata.type": "microsoft.graph.identitySet"}
 }

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "chat mention resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
