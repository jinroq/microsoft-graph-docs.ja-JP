---
title: チャネルのリソースの種類
description: 'チャネルは、チーム内の chatMessages のコレクションです。 '
author: clearab
localization_priority: Priority
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: cdcb7f10d068372c167f65a7868672a7cb669107
ms.sourcegitcommit: cca4f96414aededa03bb45e07e19bb20b7327563
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/30/2019
ms.locfileid: "36677128"
---
# <a name="channel-resource-type"></a>チャネルのリソースの種類

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

[チーム](../resources/team.md)はチャネルで構成されています。チャネルは、チームのメンバーと会話する場所です。 各チャネルは、特定のトピック、部門、プロジェクト専用です。 チャネルは、実際に作業を行う場所、チーム全体に対してテキスト、音声、ビデオによる会話を公開する場所、ファイルを共有する場所、タブを追加する場所です。

## <a name="methods"></a>メソッド

| メソッド       | 戻り値の型  |説明|
|:---------------|:--------|:----------|
|[チャネルを一覧表示する](../api/channel-list.md) | [channel](channel.md) コレクション | このチーム内のチャネルの一覧を取得します。|
|[チャネルを作成する](../api/channel-post.md) | [channel](channel.md) | 表示名と説明を指定して新しいチャネルを作成します。|
|[チャネルを取得する](../api/channel-get.md) | [channel](channel.md) | チャネルのプロパティとリレーションシップを読み取ります。|
|[チャネルを更新する](../api/channel-patch.md) | [channel](channel.md) | チャネルのプロパティを更新します。|
|[チャネルを削除する](../api/channel-delete.md) | なし | チャネルを削除します。|
|[メッセージの差分を取得する](../api/chatmessage-delta.md)  | [chatMessage](../resources/chatmessage.md) | チャネルの増分メッセージを取得します。 |
|[チャネル メッセージを一覧表示する](../api/channel-list-messages.md)  | [chatMessage](../resources/chatmessage.md) | チャネルのメッセージを取得します。 |
|[チャネル メンバーを一覧表示する](../api/conversationmember-list.md)| [conversationMember](conversationmember.md) コレクション| チャネルのメンバーを一覧表示します。 |
|[チャネル メンバーを取得する](../api/conversationmember-get.md)| [conversationMember](conversationmember.md)| チャネルのメンバーを取得します。 |
|[チャネル メンバーを追加する](../api/conversationmember-add.md) | [conversationMember](conversationmember.md)| チャネルにメンバーを追加します。 `private` の `channelType` のみサポートされます。|
|[チャネル メンバーを更新する](../api/conversationmember-update.md) | [conversationMember](conversationmember.md)| チャネルのメンバーを更新します。 `private` の `channelType` のみサポートされます。|
|[チャネル メンバーを削除する](../api/conversationmember-delete.md) | [conversationMember](conversationmember.md)| チャネルのメンバーを削除します。 `private` の `channelType` のみサポートされます。|
|[チャネルで chatMessage を作成する](../api/channel-post-messages.md) | [chatMessage](../resources/chatmessage.md) | メッセージをチャネルに送信します。 |
|[チャネルでの chatMessage 返信の作成](../api/channel-post-messagereply.md) | [chatMessage](../resources/chatmessage.md) | チャネル内のメッセージに返信します。|
|[タブを一覧表示する](../api/teamstab-list.md) | [teamsTab](teamstab.md) | チャネルにピン留めされているタブを一覧表示します。|
|[タブを取得する](../api/teamstab-get.md) | [teamsTab](teamstab.md) | チャネルにピン留めされているタブを読み取ります。|
|[タブを追加する](../api/teamstab-add.md) | [teamsTab](teamstab.md) | タブをチャネルに追加 (ピン留め) します。|
|[タブを削除する](../api/teamstab-delete.md) | なし | チャネルからタブを削除します (ピン留めを外します)。|
|[タブを更新する](../api/teamstab-update.md) | [teamsTab](teamstab.md) | タブのプロパティを更新します。|

## <a name="properties"></a>プロパティ

| プロパティ   | 型 |説明|
|:---------------|:--------|:----------|
|description|String|チャネルの説明テキストです (省略可能)。|
|displayName|String|Microsoft Teams でユーザーに対して表示されるチャネルの名前。|
|id|String|チャネルの一意の識別子。 読み取り専用。|
|isFavoriteByDefault|ブール値|チームのメンバー全員に対してチャネルを「お気に入り」として自動的にマークするかどうかを示します。 既定値: `false`。|
|メール|String| チャネルにメッセージを送信するときのメール アドレス。 読み取り専用です。|
|webUrl|String|Microsoft Teams のチャネルに移動するハイパーリンク。 これは、Microsoft Teams でチャネルを右クリックし、[チームへのリンクを取得] を選択すると作成される URL です。 この URL は不透明 blob として扱われる必要があり、また解析されません。 読み取り専用。|
|membershipType|[channelMembershipType](../resources/enums.md#channelmembershiptype-values)|チャネルの種類。 作成中に設定でき、変更できません。 既定値: 標準。|

## <a name="relationships"></a>リレーションシップ

| リレーションシップ | 型 |説明|
|:---------------|:--------|:----------|
|messages|[chatMessage](chatmessage.md) コレクション|チャネル内のすべてのメッセージのコレクションです。 ナビゲーションのプロパティです。 Null 許容型です。 現在この API では読み取りだけがサポートされていますが、最終的にはメッセージの作成もサポートされる予定です。|
|tabs|[teamsTab](../resources/teamstab.md) コレクション|チャネル内のすべてのタブのコレクションです。 ナビゲーションのプロパティです。|
|members|[conversationMember](conversationmember.md) コレクション|チャネルに関連付けられているメンバーシップ レコードのコレクション。|

## <a name="json-representation"></a>JSON 表記

リソースの JSON 表記を次に示します。

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
  "isFavoriteByDefault": true,
  "email": "string",
  "webUrl": "string",
  "membershipType": "channelMembershipType"
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
  "suppressions": []
}
-->
