---
title: チャネル リソースの種類
description: 'チャネルは、チーム内でのメッセージのコレクションです。 '
ms.openlocfilehash: 17a2e2edb86bfe7e107e69414a70dbe92fe4d3bc
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27021614"
---
# <a name="channel-resource-type"></a>チャネル リソースの種類



チャネルは、[チーム](../resources/team.md)内でのメッセージのコレクションです。 チャネルでは、トピックとチーム内での議論の論理的分離を表します。 例としては、「金曜日チーム ランチ」のチャネルとチャネルの「アーキテクチャの説明」にあります。


## <a name="methods"></a>メソッド

| メソッド       | 戻り値の型  |説明|
|:---------------|:--------|:----------|
|[チャネルのリスト](../api/channel-list.md) | [チャネル](channel.md)コレクション | このチームでは、チャネルの一覧を取得します。|
|[チャネルを作成します。](../api/channel-post.md) | [チャネル](channel.md) | 表示名と説明を含めることで、新しいチャネルを作成します。|
|[チャネルを取得します。](../api/channel-get.md) | [チャネル](channel.md) | チャネルのプロパティと関係を参照してください。|
|[チャネルを更新します。](../api/channel-patch.md) | [チャネル](channel.md) | チャネルのプロパティを更新します。|
|[チャネルを削除します。](../api/channel-delete.md) | なし | チャネルを削除します。|

## <a name="properties"></a>プロパティ
| プロパティ     | 型   |説明|
|:---------------|:--------|:----------|
|説明|String|チャネルの省略可能な説明です。|
|displayName|String|チャネルの名前は、マイクロソフトのチーム内のユーザーに表示されます。|
|id|String|チャネルの一意の識別子です。 読み取り専用。|

## <a name="relationships"></a>リレーションシップ
| リレーションシップ | 型   |説明|
|:---------------|:--------|:----------|
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