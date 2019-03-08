---
title: team リソースの種類
description: 'Microsoft Teams のチームは、チャネルのコレクションです。 '
author: nkramer
localization_priority: Priority
ms.prod: microsoft-teams
ms.openlocfilehash: 9a5f1968753d3d2412b3885e6a09e94f18731e40
ms.sourcegitcommit: d1a9e7c8e1376a99c5a5416257889ec113613a77
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 03/07/2019
ms.locfileid: "30458681"
---
# <a name="team-resource-type"></a>team リソースの種類

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Microsoft Teams のチームは、[チャネル](channel.md) のコレクションです。 チャネルは 1 つのトピック、つまりチーム内でのディスカッションの論理的分離を表します。

各チームには[グループ](../resources/group.md)が関連付けられています。
グループの ID はチームと同じです。たとえば、/groups/{id}/team は /teams/{id} と同じです。
チームのメンバーおよびグループの操作の詳細については、「[Microsoft Graph REST API を使用して Microsoft Teams を操作する](teams-api-overview.md)」を参照してください。

## <a name="methods"></a>メソッド

| メソッド       | 戻り値の型  |説明|
|:---------------|:--------|:----------|
|[チームを作成する](../api/team-post.md) | [teamsAsyncOperation](teamsasyncoperation.md) | チームを新規に作成します。 |
|[グループからチームを作成する](../api/team-put-teams.md) | [team](team.md) | 新しいチームを作成するか、既存のグループにチームを追加します。|
|[チームを取得する](../api/team-get.md) | [team](team.md) | 指定したチームのプロパティとリレーションシップを取得します。|
|[チームを更新する](../api/team-update.md) | [team](team.md) |指定されたチームのプロパティを更新します。 |
|[チームを削除する](/graph/api/group-delete?view=graph-rest-1.0) | なし |チームとその関連グループを削除します。 |
|[チームを複製する](../api/team-clone.md) | [teamsAsyncOperation](../resources/teamsasyncoperation.md) |チームとその関連グループをコピーします。 |
|[チームをアーカイブする](../api/team-archive.md) | [teamsAsyncOperation](../resources/teamsasyncoperation.md) |チームを読み取り専用状態にします。 |
|[チームを展開する](../api/team-unarchive.md) | [teamsAsyncOperation](../resources/teamsasyncoperation.md) |チームを読み取り/書き込み状態に復元します。 |
|[チームを一覧表示する](../api/user-list-joinedteams.md) | [team](team.md) コレクション | メンバーであるチームの一覧を表示します。 |
|[すべてのチームのリストを作成する](/graph/teams-list-all-teams) | [group](group.md) コレクション | チームを持つすべてのグループを一覧表示します。 |
|[組織に対してアプリを公開する](../resources/teamsapp.md)| [teamsApp](../resources/teamsapp.md) | 所属組織のみに表示する Teams アプリを作成します。 |
|[アプリをチームに追加する](../api/teamsappinstallation-add.md) | [teamsappinstallation](teamsappinstallation.md) | アプリをチームに追加 (インストール) します。|
|[チャネルにタブを追加する](../api/teamstab-add.md) | [teamsTab](../resources/teamstab.md) | タブをチームのチャネルに追加 (インストール) します。|
|[チャネル メッセージを一覧表示する](../api/channel-list-messages.md)  | [chatMessage](../resources/chatmessage.md) | [チャネルのメッセージを取得する](../api/channel-list-messages.md) |
|[チャネル メッセージを送信する](../api/channel-post-chatmessage.md)  | [chatMessage](../resources/chatmessage.md) | [メッセージをチャネルに送信する](../api/channel-post-chatmessage.md) |

## <a name="properties"></a>プロパティ

| プロパティ | 型   | 説明 |
|:---------------|:--------|:----------|
|displayName|string| チームの名前。 |
|説明|string| チームに関するオプションの説明。 |
|classification|string| 省略可能なラベル。 通常、チームのデータまたはビジネスの機密度を記述します。 テナントのディレクトリで事前に構成されているセットのいずれかに一致する必要があります。 |
|specialization|[teamSpecialization](teamspecialization.md)| 省略可能。 チームが特定のユース ケースを目的としているかどうかを示します。  チーム専門分野ごとに、ユース ケースをターゲットとする一意の動作とエクスペリエンスにアクセスできます。 |
|visibility|[teamVisibilityType](teamvisibilitytype.md)| グループとチームの可視性。 既定では Public です。 |
|funSettings|[teamFunSettings](teamfunsettings.md) |チームでの Giphy、ミーム、およびステッカーの使用を構成する設定。|
|guestSettings|[teamGuestSettings](teamguestsettings.md) |ゲストがチームでチャネルを作成、更新、削除できるかどうかを構成する設定。|
|InternalId | string | 監査ログまたは [Office 365 マネージメント アクティビティ API](https://docs.microsoft.com/ja-JP/office/office-365-management-api/office-365-management-activity-api-reference) など、いくつかの場所で使用されているチームの一意の ID。 |
|isArchived|Boolean|このチームが読み取り専用モードかどうか。 |
|memberSettings|[teamMemberSettings](teammembersettings.md) |メンバーが特定のアクション (チャネルの作成、ボットの追加など) をチーム内で実行できるかどうかを構成する設定。|
|messagingSettings|[teamMessagingSettings](teammessagingsettings.md) |チームでメッセージとメンションを構成する設定。|
|webUrl|string (読み取り専用) | Microsoft Teams クライアントのチームに移動するハイパーリンク。 これは、Microsoft Teams クライアントでチームを右クリックし、**[Get link to team]** を選択すると作成される URL です。 この URL は不透明 blob として扱われる必要があり、また解析されません。 |

## <a name="relationships"></a>リレーションシップ

| リレーションシップ | 型   | 説明 |
|:---------------|:--------|:----------|
|apps|[teamsApp](teamsapp.md) コレクション| (現在不使用) このチームにインストールされているアプリ。|
|channels|[channel](channel.md) コレクション|チームに関連付けられているチャネルとメッセージのコレクション。|
|installedApps|[teamsAppInstallation](teamsappinstallation.md) コレクション|このチームにインストールされているアプリ。|
|owners|[user](user.md)| このチームの所有者の一覧。 現時点では、アプリケーションのアクセス許可を使用してチームを作成するときに、必ず 1 つの所有者を指定してください。 ユーザー委任アクセス許可を使用するときには、所有者を指定できません (現在のユーザーが所有者になります)。 所有者は、UPN ではなくオブジェクト ID (GUID) として指定する必要があります。 |
|operations|[teamsAsyncOperation](teamsasyncoperation.md) コレクション| このチームで実行済みまたは実行中の非同期操作です。 | 
|template|[teamsTemplate](teamstemplate.md)| このチームの作成元テンプレート。 [使用可能なテンプレート](https://docs.microsoft.com/ja-JP/MicrosoftTeams/get-started-with-teams-templates)を参照してください。 |

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
  "internalId": "19:...big.number...@thread.skype",
  "isArchived": false,
  "webUrl": "https://...longUrl..."
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "team resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/team.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->

## <a name="see-also"></a>関連項目
- [チームを使用してグループを作成する](/graph/teams-create-group-and-team)
- [Teams API の概要](teams-api-overview.md)
