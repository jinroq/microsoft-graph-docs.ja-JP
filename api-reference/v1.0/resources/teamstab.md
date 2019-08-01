---
title: teamsTab リソースの種類
description: 'TeamsTab は、チーム内のチャネルに固定 (接続) されたタブです。 '
localization_priority: Normal
author: nkramer
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: bf07770d920ee05c7856f89e2e099bcc958ad50c
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "36033692"
---
# <a name="teamstab-resource-type"></a>teamsTab リソースの種類



TeamsTab は、[チーム](team.md)内の[チャネル](channel.md)に固定 (接続) された[タブ](../resources/teamstab.md)です。 

## <a name="methods"></a>メソッド

| メソッド       | 戻り値の型  |説明|
|:---------------|:--------|:----------|
|[タブを一覧表示する](../api/teamstab-list.md) | [teamsTab](teamstab.md) | チャネルにピン留めされているタブを一覧表示します。|
|[タブを取得する](../api/teamstab-get.md) | [teamsTab](teamstab.md) | チャネルにピン留めされているタブを読み取ります。|
|[タブを追加する](../api/teamstab-add.md) | [teamsTab](teamstab.md) | タブをチャネルに追加 (ピン留め) します。|
|[タブを削除する](../api/teamstab-delete.md) | なし | チャネルからタブを削除します (ピン留めを外します)。|
|[タブを更新する](../api/teamstab-update.md) | [teamsTab](teamstab.md) | タブのプロパティを更新します。|


## <a name="properties"></a>プロパティ

|プロパティ|型|説明|
|:---------------|:--------|:----------|
|  id              |   string                  |  チャネルタブの特定のインスタンスを一意に識別する識別子。読み取り専用。     |
|  displayName            |   string                  |  タブの名前を指定します。     |
|  webUrl          |   string                  |  Tab インスタンスのディープリンク url。 読み取り専用です。     |
|  環境        |   [teamsTabConfiguration](teamstabconfiguration.md) |  タブに適用されるカスタム設定のコンテナーです。このプロパティが設定されると、タブは構成されたことを示します。     |

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
