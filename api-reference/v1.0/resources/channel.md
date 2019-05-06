---
title: チャネルのリソースの種類
description: 'チャネルは、チーム内のメッセージのコレクションです。 '
author: nkramer
localization_priority: Priority
ms.prod: microsoft-teams
ms.openlocfilehash: 6c1f73746081e5b1e4f78acb91d43e33c1c9bf73
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32569460"
---
# <a name="channel-resource-type"></a>チャネルのリソースの種類

[チーム](../resources/team.md)はチャネルで構成されています。チャネルは、チームのメンバーと会話する場所です。 各チャネルは、特定のトピック、部門、プロジェクト専用です。
チャネルは、実際に作業を行う場所、チーム全体に対してテキスト、音声、ビデオによる会話を公開する場所、ファイルを共有する場所、タブを追加する場所です。

## <a name="methods"></a>メソッド

| メソッド       | 戻り値の型  |説明|
|:---------------|:--------|:----------|
|[チャネルを一覧表示する](../api/channel-list.md) | [channel](channel.md) コレクション | このチーム内のチャネルの一覧を取得します。|
|[チャネルを作成する](../api/channel-post.md) | [channel](channel.md) | 表示名と説明を指定して新しいチャネルを作成します。|
|[チャネルを取得する](../api/channel-get.md) | [channel](channel.md) | チャネルのプロパティとリレーションシップを読み取ります。|
|[チャネルを更新する](../api/channel-patch.md) | [channel](channel.md) | チャネルのプロパティを更新します。|
|[チャネルを削除する](../api/channel-delete.md) | なし | チャネルを削除します。|
|[タブを一覧表示する](../api/teamstab-list.md) | [teamsTab](teamstab.md) | チャネルにピン留めされているタブを一覧表示します。|
|[タブを取得する](../api/teamstab-get.md) | [teamsTab](teamstab.md) | チャネルにピン留めされているタブを読み取ります。|
|[タブを追加する](../api/teamstab-add.md) | [teamsTab](teamstab.md) | タブをチャネルに追加 (ピン留め) します。|
|[タブを削除する](../api/teamstab-delete.md) | なし | チャネルからタブを削除します (ピン留めを外します)。|
|[タブを更新する](../api/teamstab-update.md) | [teamsTab](teamstab.md) | タブのプロパティを更新します。|

## <a name="properties"></a>Properties
| プロパティ     | 型   |説明|
|:---------------|:--------|:----------|
|description|String|チャネルの説明テキストです (省略可能)。|
|displayName|String|Microsoft Teams でユーザーに対して表示されるチャネルの名前。|
|メール|String| チャネルにメッセージを送信するときのメール アドレス。 読み取り専用です。|
|id|String|チャネルの一意の識別子。 読み取り専用です。|
|webUrl|String|Microsoft Teams のチャネルに移動するハイパーリンク。 これは、Microsoft Teams でチャネルを右クリックし、[チームへのリンクを取得] を選択すると作成される URL です。 この URL は不透明 blob として扱われる必要があり、また解析されません。 読み取り専用です。|

## <a name="relationships"></a>関係
| リレーションシップ | 型   |説明|
|:---------------|:--------|:----------|
|tabs|[teamsTab](../resources/teamstab.md) コレクション|チャネル内のすべてのタブのコレクションです。 ナビゲーションのプロパティです。|


## <a name="json-representation"></a>JSON 表記

以下は、リソースの JSON 表記です

<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.channel"
}-->

```json
{
  "description": "string",
  "displayName": "string",
  "email": "string (identifier)",
  "id": "string",
  "webUrl": "string"
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
