---
title: teamstab リソースの種類
description: 'teamstab は、チーム内のチャネルに固定 (接続) されたタブです。 '
localization_priority: Normal
author: nkramer
ms.prod: microsoft-teams
ms.openlocfilehash: 181d2fd23ff922709b3e098f6069adf300ad3928
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32456981"
---
# <a name="teamstab-resource-type"></a>teamstab リソースの種類



teamstab は、[チーム](team.md)内の[チャネル](channel.md)に固定 (接続) された[タブ](../resources/teamstab.md)です。 

## <a name="methods"></a>メソッド

| メソッド       | 戻り値の型  |説明|
|:---------------|:--------|:----------|
|[タブを一覧表示する](../api/teamstab-list.md) | [teamsTab](teamstab.md) | チャネルにピン留めされたタブを一覧表示します。|
|[タブを取得する](../api/teamstab-get.md) | [teamsTab](teamstab.md) | チャネルにピン留めされたタブを読み取ります。|
|[タブを追加する](../api/teamstab-add.md) | [teamsTab](teamstab.md) | チャネルにタブを追加 (ピン留め) します。|
|[タブの削除](../api/teamstab-delete.md) | なし | チャネルからタブを削除 (固定解除) します。|
|[タブを更新する](../api/teamstab-update.md) | [teamsTab](teamstab.md) | タブのプロパティを更新します。|


## <a name="properties"></a>プロパティ

|プロパティ|型|説明|
|:---------------|:--------|:----------|
|  ID              |   string                  |  チャネルタブの特定のインスタンスを一意に識別する識別子。読み取り専用。     |
|  displayName            |   string                  |  タブの名前を指定します。     |
|  webUrl          |   string                  |  tab インスタンスのディープリンク url。 読み取り専用です。     |
|  環境        |   [teamstabconfiguration](teamstabconfiguration.md) |  タブに適用されるカスタム設定のコンテナーです。このプロパティが設定されると、タブは構成されたことを示します。     |

## <a name="relationships"></a>リレーションシップ

| リレーションシップ | 型   | 説明 |
|:---------------|:--------|:----------|
|teamsApp|[teamsApp](teamsapp.md) | タブにリンクされているアプリケーション。これは、タブの作成後に変更することはできません。 |

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

[組み込みタブ タイプの構成](/graph/teams-configuring-builtin-tabs)
