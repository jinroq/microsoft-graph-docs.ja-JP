---
title: teamsTab リソースの種類
description: 'タブでは、teamsTab をチーム内でのチャネル (接続) を固定しました。 '
ms.openlocfilehash: 102d4c0b766d8a0d9bdf22cb2ed76f5e06d87ad5
ms.sourcegitcommit: f3d479edf03935d0edbbc7668a65f7cde2a56c92
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 12/15/2018
ms.locfileid: "27283620"
---
# <a name="teamstab-resource-type"></a>teamsTab リソースの種類

> **重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。 実稼働アプリケーションでの、これらの API の使用はサポートされていません。

[] タブ](../resources/teamstab.md)では、teamsTab を[チーム](team.md)内での[チャネル](channel.md)(接続) を固定しました。 

## <a name="methods"></a>メソッド

| メソッド       | 戻り値の型  |説明|
|:---------------|:--------|:----------|
|[一覧] タブ](../api/teamstab-list.md) | [teamsTab](teamstab.md) | リスト タブは、チャンネルに固定します。|
|[タブを取得します。](../api/teamstab-get.md) | [teamsTab](teamstab.md) | チャンネルに固定されているタブを読み取ります。|
|[タブを追加します。](../api/teamstab-add.md) | [teamsTab](teamstab.md) | (ピン) を追加するチャンネルをタブします。|
|[タブを削除します。](../api/teamstab-delete.md) | なし | 削除 (固定解除) チャネルからタブします。|
|[[更新] タブ](../api/teamstab-update.md) | [teamsTab](teamstab.md) | タブのプロパティを更新します。|


## <a name="properties"></a>Properties

|プロパティ|種類|説明|
|:---------------|:--------|:----------|
|  ID              |   string                  |  チャネル タブ読み取りのみの特定のインスタンスを一意に識別する識別子です。     |
|  displayName            |   string                  |  タブの名前です。     |
|  name            |   文字列                  |  (非推奨)タブの名前です。     |
|  teamsAppId           |   string             |  タブのアプリケーション定義の識別子です。タブを作成した後は、この値を変更できません。     |
|  sortOrderIndex  |   int                     |  タブの並べ替え順序のインデックス。     |
|  webUrl          |   string                  |  タブのインスタンスの高度なリンクの url です。 読み取り専用です。     |
|  configuration        |   [teamsTabConfiguration](teamstabconfiguration.md) |  タブに適用するカスタム設定のコンテナーです。タブでは、このプロパティが 1 回だけが構成されていると見なされます。     |

## <a name="relationships"></a>リレーションシップ

| リレーションシップ | 型   | 説明 |
|:---------------|:--------|:----------|
|teamsApp|[teamsApp](teamsapp.md) | タブにリンクされているアプリケーションです。 |

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
  "teamsAppId": "string",
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
