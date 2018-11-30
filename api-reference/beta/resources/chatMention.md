---
title: chatMessageMention リソースの種類
description: 'ChatMessage エンティティの参照を表します。 ユーザー、チーム、ボットまたはチャネルをことができます。 '
ms.openlocfilehash: 5f1e427b0ed2b8ffcfbc86417beb4719dc6fb2a3
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27066765"
---
# <a name="chatmessagemention-resource-type"></a>chatMessageMention リソースの種類

> **重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。 実稼働アプリケーションでの、これらの API の使用はサポートされていません。

[ChatMessage](chatmessage.md)エンティティの参照を表します。 ユーザー、チーム、ボットまたはチャネルをことができます。 

## <a name="properties"></a>プロパティ
| プロパティ     | 型   |説明|
|:---------------|:--------|:----------|
|ID|文字列|記載されているエンティティの id|
|mentionText|文字列|Ex の説明を表すために使用する文字列: ユーザーの表示名、チーム名等|
|記載されています。|[identitySet](identityset.md)|記載されているユーザー|

## <a name="json-representation"></a>JSON 表記

リソースの JSON 表記を次に示します。

<!-- {
  "blockType": "resource",
  "baseType": "microsoft.graph.entity",
  "@odata.type": "microsoft.graph.chatMessageMention"
}-->

```json
{
  "id": "string (identifier)",
  "mentionText": "string",
  "mentioned": "microsoft.graph.identitySet"
 }

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "chat mention resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
