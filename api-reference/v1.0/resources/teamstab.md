---
title: teamsTab リソースの種類
description: 'タブでは、teamsTab をチーム内でのチャネル (接続) を固定しました。 '
localization_priority: Normal
author: nkramer
ms.prod: microsoft-teams
ms.openlocfilehash: 305b8d530eb0b10a658a1b5e5051f7854e3919ee
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/12/2019
ms.locfileid: "27917777"
---
# <a name="teamstab-resource-type"></a>teamsTab リソースの種類



[] タブ](../resources/teamstab.md)では、teamsTab を[チーム](team.md)内での[チャネル](channel.md)(接続) を固定しました。 

## <a name="methods"></a>メソッド

| メソッド       | 戻り値の型  |説明|
|:---------------|:--------|:----------|
|[一覧] タブ](../api/teamstab-list.md) | [teamsTab](teamstab.md) | リスト タブは、チャンネルに固定します。|
|[タブを取得します。](../api/teamstab-get.md) | [teamsTab](teamstab.md) | チャンネルに固定されているタブを読み取ります。|
|[タブを追加します。](../api/teamstab-add.md) | [teamsTab](teamstab.md) | (ピン) を追加するチャンネルをタブします。|
|[タブを削除します。](../api/teamstab-delete.md) | なし | 削除 (固定解除) チャネルからタブします。|
|[[更新] タブ](../api/teamstab-update.md) | [teamsTab](teamstab.md) | タブのプロパティを更新します。|


## <a name="properties"></a>プロパティ

|プロパティ|種類|説明|
|:---------------|:--------|:----------|
|  ID              |   文字列                  |  チャネル タブ読み取りのみの特定のインスタンスを一意に識別する識別子です。     |
|  displayName            |   string                  |  タブの名前です。     |
|  sortOrderIndex  |   int                     |  タブの並べ替え順序のインデックス     |
|  webUrl          |   文字列                  |  タブのインスタンスの高度なリンクの url です。 読み取り専用です。     |
|  configuration        |   [teamsTabConfiguration](teamstabconfiguration.md) |  タブに適用するカスタム設定のコンテナーです。タブでは、このプロパティが 1 回だけが構成されていると見なされます。     |

## <a name="relationships"></a>リレーションシップ

| リレーションシップ | 型   | 説明 |
|:---------------|:--------|:----------|
|teamsApp|[teamsApp](teamsapp.md) | タブにリンクされているアプリケーションです。タブを作成した後は、これを変更できません。 |

## <a name="json-representation"></a>JSON 表記

リソースの JSON 表記を次に示します。


<!-- {
  "blockType": "resource",
  "baseType": "microsoft.graph.entity",
  "@odata.type": "microsoft.graph.teamsTab"
}-->

```json
{  
  "id": "string",
  "displayName": "string",
  "sortOrderIndex": "string",
  "webUrl": "string",
  "configuration" : "teamsTabConfiguration"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "teamsTab resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

## <a name="see-also"></a>関連項目

[組み込みタブのタイプを設定します。](/graph/teams-configuring-builtin-tabs)
