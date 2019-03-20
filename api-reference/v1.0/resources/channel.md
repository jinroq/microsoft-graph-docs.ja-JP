---
title: チャネルのリソースの種類
description: 'チャネルは、チーム内のメッセージのコレクションです。 '
author: nkramer
localization_priority: Priority
ms.prod: microsoft-teams
ms.openlocfilehash: 2bebf78e4ad31047289bff77e681c34d92a94abf
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 02/21/2019
ms.locfileid: "30163715"
---
# <a name="channel-resource-type"></a>チャネルのリソースの種類



チャネルは、[チーム](../resources/team.md)内のメッセージのコレクションです。 チャネルは 1 つのトピック、つまりチーム内でのディスカッションの論理的分離を表します。 たとえば、「Friday Team Lunch (金曜日のチーム ランチ)」チャネルや「Architecture Discussion (アーキテクチャに関するディスカッション)」チャネルなどです。


## <a name="methods"></a>メソッド

| メソッド       | 戻り値の型  |説明|
|:---------------|:--------|:----------|
|[チャネルを一覧表示する](../api/channel-list.md) | [channel](channel.md) コレクション | このチーム内のチャネルの一覧を取得します。|
|[チャネルを作成する](../api/channel-post.md) | [channel](channel.md) | 表示名と説明を指定して新しいチャネルを作成します。|
|[チャネルを取得する](../api/channel-get.md) | [channel](channel.md) | チャネルのプロパティとリレーションシップを読み取ります。|
|[チャネルを更新する](../api/channel-patch.md) | [channel](channel.md) | チャネルのプロパティを更新します。|
|[チャネルを削除する](../api/channel-delete.md) | なし | チャネルを削除します。|

## <a name="properties"></a>プロパティ
| プロパティ     | 型   |説明|
|:---------------|:--------|:----------|
|description|String|チャネルの説明テキストです (省略可能)。|
|displayName|String|Microsoft Teams でユーザーに対して表示されるチャネルの名前。|
|id|String|チャネルの一意の識別子。 読み取り専用。|

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
  "id": "string (identifier)"
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
