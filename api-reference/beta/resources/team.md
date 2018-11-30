---
title: チーム リソースの種類
description: 'マイクロソフトのチームで、チームは、チャネルのコレクションです。 '
ms.openlocfilehash: 5ebb4dbc2c5913d69b69bdb244d8a7cfc83cec8d
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27070581"
---
# <a name="team-resource-type"></a>チーム リソースの種類

> **重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。 実稼働アプリケーションでの、これらの API の使用はサポートされていません。

マイクロソフトのチームで、チームは、[チャネル](channel.md)のコレクションです。 チャネルでは、トピックとチーム内での議論の論理的分離を表します。

すべてのチームは、[グループ](../resources/group.md)に関連付けられます。
グループは、チーム ・/groups/{id} などと同じ ID を持っているし、チームは、/teams/{id} と同じです。
グループとチームのメンバーの詳細については、[マイクロソフトのチームで作業するのには Microsoft グラフ REST API を使用](teams-api-overview.md)を参照してください。

## <a name="methods"></a>メソッド

| メソッド       | 戻り値の型  |説明|
|:---------------|:--------|:----------|
|[チームを作成します。](../api/team-put-teams.md) | [チーム](team.md) | 新しいチームを作成または既存のグループにチームを追加します。|
|[チームを取得します。](../api/team-get.md) | [チーム](team.md) | プロパティと指定されたチームの関係を取得します。|
|[チームを更新します。](../api/team-update.md) | [チーム](team.md) |指定されたチームのプロパティを更新します。 |
|[チームを削除します。](/graph/api/group-delete?view=graph-rest-1.0) | なし |チームおよびその関連付けられているグループを削除します。 |
|[チームのクローンを作成します。](../api/team-clone.md) | [teamsAsyncOperation](../resources/teamsasyncoperation.md) |チームおよびその関連付けられているグループをコピーします。 |
|[チームのアーカイブ](../api/team-archive.md) | [teamsAsyncOperation](../resources/teamsasyncoperation.md) |読み取り専用状態で、チームを配置します。 |
|[チームを unarchive します。](../api/team-unarchive.md) | [teamsAsyncOperation](../resources/teamsasyncoperation.md) |チームを読み取り/書き込み状態に復元します。 |
|[チームの一覧を表示します。](../api/user-list-joinedteams.md) | [チーム](team.md)コレクション | チームのメンバーを一覧表示します。 |
|[すべてのチームをリストします。](/graph/teams-list-all-teams) | [group](group.md) コレクション | チームのすべてのグループを一覧表示します。 |
|[組織にアプリケーションを発行します。](../resources/teamsapp.md)| [teamsApp](../resources/teamsapp.md) | 組織にのみ表示されているチームのアプリケーションを作成します。 |
|[アプリケーションをチームに追加します。](../api/teamsappinstallation-add.md) | [teamsappinstallation](teamsappinstallation.md) | (インストール) を追加するチームにアプリです。|
|[チャネルにタブを追加します。](../api/teamstab-add.md) | [teamsTab](../resources/teamstab.md) | (インストール) を追加するチャネル ・ チームのタブです。|
|[リストからチャネルのメッセージ](../api/channel-list-messages.md)  | [chatMessage](../resources/chatmessage.md) | [チャネルでメッセージを取得します。](../api/channel-list-messages.md) |

## <a name="properties"></a>プロパティ

| プロパティ | 型   | 説明 |
|:---------------|:--------|:----------|
|funSettings|[teamFunSettings](teamfunsettings.md) |Giphy、memes、およびチームのステッカーを構成する設定を使用します。|
|guestSettings|[teamGuestSettings](teamguestsettings.md) |来園者が作成、更新、またはチーム内のチャンネルを削除するかどうかを構成するのに設定します。|
|isArchived|ブール値|このチームが、読み取り専用モードでかどうかです。 |
|memberSettings|[teamMemberSettings](teammembersettings.md) |など、メンバーが特定のアクションを実行するかどうかを構成する設定は、チャネルを作成し、チームにボットを追加します。|
|messagingSettings|[teamMessagingSettings](teammessagingsettings.md) |メッセージングを構成する設定は、チーム内の参照。|
|webUrl|文字列 (読み取り専用) | クライアントの Microsoft のチームにチームに移動するハイパーリンク。 これは、クライアントの Microsoft のチームにチームを右クリックし、**チームへのリンクを取得する**を選択するときに表示される URL です。 この URL は、非透過 blob として扱われます、解析されない必要があります。 |

## <a name="relationships"></a>リレーションシップ

| リレーションシップ | 型   | 説明 |
|:---------------|:--------|:----------|
|apps|[teamsApp](teamsapp.md)コレクション| (古い形式)このチームにインストールされているアプリケーションです。|
|チャンネル|[チャネル](channel.md)コレクション|チャンネルとチームに関連付けられているメッセージのコレクションです。|
|installedApps|[teamsAppInstallation](teamsappinstallation.md)コレクション|このチームにインストールされているアプリケーションです。|

## <a name="json-representation"></a>JSON 表記

リソースの JSON 表記を次に示します。

<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.team",
  "baseType": "microsoft.graph.entity"
}-->

```json
{  
  "guestSettings": {"@odata.type": "microsoft.graph.teamGuestSettings"},
  "memberSettings": {"@odata.type": "microsoft.graph.teamMemberSettings"},
  "messagingSettings": {"@odata.type": "microsoft.graph.teamMessagingSettings"},
  "funSettings": {"@odata.type": "microsoft.graph.teamFunSettings"},
  "isArchived": false,
  "webUrl": "https://...longUrl..."
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "team resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

## <a name="see-also"></a>関連項目
- [チームのグループを作成](/graph/teams-create-group-and-team)
- [チーム API の概要](teams-api-overview.md)
