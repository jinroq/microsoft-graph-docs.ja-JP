---
title: チャットリソースの種類
description: チャットは、1人または複数の参加者間の chatMessages のコレクションです。
author: clearab
doc_type: resourcePageType
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: 83ab8428fb09a7a2dc0546dcebdf2f409d90d25a
ms.sourcegitcommit: 82b73552fff79a4ef7a2ee57fc2d1b3286b5bd4c
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/26/2019
ms.locfileid: "35908494"
---
# <a name="chat-resource-type"></a>チャットリソースの種類

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

チャットは、1人または複数の参加者間の[Chatmessages](chatmessage.md)のコレクションです。 参加者には、ユーザーまたはアプリがあります。

## <a name="methods"></a>メソッド

|  メソッド       |  戻り値の型  | 説明|
|:---------------|:--------|:----------|
|[チャットの一覧表示](../api/chat-list.md) | [chat](channel.md)コレクション | ユーザーが属するチャットのリストを取得します。|
|[チャットの取得](../api/chat-get.md) | [チャット](channel.md) | チャットのプロパティと関係を読み取ります。|
|[チャットメンバーを一覧表示する](../api/conversationmember-list.md) | [conversationmember](conversationmember.md)コレクション | チャット内のすべてのユーザーの一覧を取得します。|
|[チャットメンバーを取得する](../api/conversationmember-get.md) | [conversationmember](conversationmember.md) | チャットで1人のユーザーを取得します。|
|[チャット内のメッセージを一覧表示する](../api/chatmessage-list.md)  | [chatMessage](../resources/chatmessage.md) | 1 対 1 またはグループ チャットでのメッセージを取得します。 |
|[チャット内のメッセージを取得する](../api/chatmessage-get.md)  | [chatMessage](../resources/chatmessage.md) | チャット内の 1 つのメッセージを取得します。 |

## <a name="properties"></a>Properties

| プロパティ   | 型 |説明|
|:---------------|:--------|:----------|
| id| String| チャットの一意識別子。 読み取り専用です。|
| topic| String|  オプションチャットの件名またはトピック。 グループチャットでのみ使用できます。|
| createdDateTime| dateTimeOffset|  チャットが作成された日付と時刻。 読み取り専用です。|
| lastUpdatedDateTime| dateTimeOffset|  チャットが更新された日付と時刻。 読み取り専用です。|

## <a name="relationships"></a>関係

| リレーションシップ | 型 |説明|
|:---------------|:--------|:----------|
| installedApps | [teamsAppInstallation](teamsappinstallation.md) コレクション | チャット内のすべてのアプリのコレクション。 Null 許容型。 |
| members | [conversationMember](conversationmember.md)コレクション | チャット内のすべてのユーザーのコレクション。 Null 許容型。 |
| messages | [chatMessage](chatmessage.md) コレクション | チャット内のすべてのメッセージのコレクション。 Null 許容型。 |

## <a name="json-representation"></a>JSON 表記

以下は、リソースの JSON 表記です。

<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.chat"
}-->

```json
{
  "id": "string (identifier)",
  "topic": "string",
  "createdDateTime": "dateTimeOffset",
  "lastUpdatedDateTime": "dateTimeOffset"
}

```

## <a name="see-also"></a>関連項目

- [channel](channel.md)
- [chatMessage](chatmessage.md)

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "chat resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}
-->
