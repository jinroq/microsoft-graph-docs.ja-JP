---
title: チャネルのリソースの種類
description: 'チャネルは、チーム内の chatMessages のコレクションです。 '
author: nkramer
localization_priority: Priority
ms.prod: microsoft-teams
ms.openlocfilehash: d58a3e0b867a675e378fa126108331fd5b27856c
ms.sourcegitcommit: a4773239d8559899c3f9433b3073e250a56d2e04
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 02/13/2019
ms.locfileid: "29994469"
---
# <a name="channel-resource-type"></a>チャネルのリソースの種類

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

チャネルは、[チーム](../resources/team.md)内の [chatMessages](chatmessage.md) のコレクションです。 チャネルは 1 つのトピック、つまりチーム内でのディスカッションの論理的分離を表します。 たとえば、「Friday Team Lunch (金曜日のチーム ランチ)」チャネルや「Architecture Discussion (アーキテクチャに関するディスカッション)」チャネルなどです。


## <a name="methods"></a>メソッド

| メソッド       | 戻り値の型  |説明|
|:---------------|:--------|:----------|
|[チャネルを一覧表示する](../api/channel-list.md) | [channel](channel.md) コレクション | このチーム内のチャネルの一覧を取得します。|
|[チャネルを作成する](../api/channel-post.md) | [channel](channel.md) | 表示名と説明を指定して新しいチャネルを作成します。|
|[チャネルを取得する](../api/channel-get.md) | [channel](channel.md) | チャネルのプロパティとリレーションシップを読み取ります。|
|[チャネルを更新する](../api/channel-patch.md) | [channel](channel.md) | チャネルのプロパティを更新します。|
|[チャネルを削除する](../api/channel-delete.md) | なし | チャネルを削除します。|
|[チャネル メッセージを一覧表示する](../api/channel-list-messages.md)  | [chatMessage](../resources/chatmessage.md) | チャネルのメッセージを取得します。 |
|[チャネル メッセージを送信する](../api/channel-post-chatmessage.md)  | [chatMessage](../resources/chatmessage.md) | [メッセージをチャネルに送信する](../api/channel-post-chatmessage.md) |


## <a name="properties"></a>プロパティ
| プロパティ     | 型   |説明|
|:---------------|:--------|:----------|
|description|String|チャネルの説明テキストです (省略可能)。|
|displayName|String|Microsoft Teams でユーザーに対して表示されるチャネルの名前。|
|id|String|チャネルの一意の識別子。 読み取り専用です。|
|isFavoriteByDefault|Boolean|チームのメンバー全員に対してチャネルを「お気に入り」として自動的にマークするかどうか。 既定値: `false`。|
|email|Boolean| チャネルにメッセージを送信するときのメール アドレス。 読み取り専用です。|
|webUrl|String|Microsoft Teams のチャネルに移動するハイパーリンク。 これは、Microsoft Teams でチャネルを右クリックし、[チームへのリンクを取得] を選択すると作成される URL です。 この URL は不透明 blob として扱われる必要があり、また解析されません。 読み取り専用です。|


## <a name="relationships"></a>関係
| リレーションシップ | 型   |説明|
|:---------------|:--------|:----------|
|messages|[chatMessage](chatmessage.md) コレクション|チャネル内のすべてのメッセージのコレクションです。 ナビゲーションのプロパティです。 Null 許容型です。 現在この API では読み取りだけがサポートされていますが、最終的にはメッセージの作成もサポートされる予定です。|
|tabs|[teamsTab](../resources/teamstab.md) コレクション|チャネル内のすべてのタブのコレクションです。 ナビゲーションのプロパティです。|


## <a name="json-representation"></a>JSON 表記

以下は、リソースの JSON 表記です

<!-- {
  "blockType": "resource",
  "optionalProperties": [
    "messages"
  ],
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.channel"
}-->

```json
{
  "description": "string",
  "displayName": "string",
  "id": "string (identifier)",
}

```


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "channel resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/channel.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
