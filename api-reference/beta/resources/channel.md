---
title: チャネル リソースの種類
description: 'チャネルは、チーム内での chatMessages のコレクションです。 '
author: nkramer
localization_priority: Priority
ms.openlocfilehash: 058632c9f56462195db0cd268fd0af262d4292f3
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/11/2019
ms.locfileid: "27842687"
---
# <a name="channel-resource-type"></a>チャネル リソースの種類

> **重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。 実稼働アプリケーションでの、これらの API の使用はサポートされていません。

チャネルは、[チーム](../resources/team.md)内での[chatMessages](chatmessage.md)のコレクションです。 チャネルでは、トピックとチーム内での議論の論理的分離を表します。 例としては、「金曜日チーム ランチ」のチャネルとチャネルの「アーキテクチャの説明」にあります。


## <a name="methods"></a>メソッド

| メソッド       | 戻り値の型  |説明|
|:---------------|:--------|:----------|
|[チャネルのリスト](../api/channel-list.md) | [チャネル](channel.md)コレクション | このチームでは、チャネルの一覧を取得します。|
|[チャネルを作成します。](../api/channel-post.md) | [チャネル](channel.md) | 表示名と説明を含めることで、新しいチャネルを作成します。|
|[チャネルを取得します。](../api/channel-get.md) | [チャネル](channel.md) | チャネルのプロパティと関係を参照してください。|
|[チャネルを更新します。](../api/channel-patch.md) | [チャネル](channel.md) | チャネルのプロパティを更新します。|
|[チャネルを削除します。](../api/channel-delete.md) | なし | チャネルを削除します。|
|[リストからチャネルのメッセージ](../api/channel-list-messages.md)  | [chatMessage](../resources/chatmessage.md) | チャネルでメッセージを取得します。 |
|[チャットのスレッドを作成します。](../api/channel-post-chatthreads.md) | [chatThread](chatthread.md)コレクション| 指定したチャンネルでのチャットのスレッドを作成します。|

## <a name="properties"></a>プロパティ
| プロパティ     | 種類   |説明|
|:---------------|:--------|:----------|
|説明|String|チャネルの省略可能な説明です。|
|displayName|String|チャネルの名前は、マイクロソフトのチーム内のユーザーに表示されます。|
|id|String|チャネルの一意の識別子です。 読み取り専用です。|
|isFavoriteByDefault|ブール型|かどうかチャネルが自動的にマークされます 'お気に入り' チームのすべてのメンバーの。 既定値: `false`。|
|email|ブール型| チャネルにメッセージを送信する電子メール アドレスです。 読み取り専用です。|
|webUrl|String|ハイパーリンクは、マイクロソフトのチーム内のチャネルに移動します。 これは、マイクロソフトのチームでチャネルを右クリックし、チャネルを取得] リンクを選択するときに表示される URL です。 この URL は、非透過 blob として扱われます、解析されない必要があります。 読み取り専用です。|


## <a name="relationships"></a>リレーションシップ
| リレーションシップ | 型   |説明|
|:---------------|:--------|:----------|
|messages|[chatMessage](chatmessage.md)コレクション|チャネル内のすべてのメッセージのコレクションです。 ナビゲーション プロパティです。 Null 許容型。 現在この API のみの読み取りをサポートしていますは、ついに手書きのメッセージも。|
|chatThreads|[chatThread](chatthread.md)コレクション|(これは、段階的に廃止のメッセージ プロパティを優先して) chatThreads は、新規メッセージの作成ができないメッセージの読み取りをサポートしています。 ChatThreads は、ナビゲーション プロパティで、null 値です。|
|タブ|[teamsTab](../resources/teamstab.md)コレクション|チャネル内のすべてのタブのコレクションです。 ナビゲーション プロパティです。|


## <a name="json-representation"></a>JSON 表記

以下は、リソースの JSON 表記です

<!-- {
  "blockType": "resource",
  "optionalProperties": [
    "chatthreads"
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
<!-- {
  "type": "#page.annotation",
  "description": "channel resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
