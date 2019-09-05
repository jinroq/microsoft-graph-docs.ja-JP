---
title: Microsoft Graph API を使用して Microsoft Teams で作業する
description: Microsoft Teams は、Office 365 のチャットベースのワークスペースであり、チーム固有の予定表、ファイル、OneNote のノート、Planner のプランなどへの組み込みのアクセスを提供します。
localization_priority: Priority
author: nkramer
ms.prod: microsoft-teams
doc_type: conceptualPageType
ms.openlocfilehash: db0809790247e834a64672699b0a4183c04f5458
ms.sourcegitcommit: d1742ec820776f1e95cba76d98c6cfd17d3eadbb
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 09/04/2019
ms.locfileid: "36730324"
---
# <a name="use-the-microsoft-graph-api-to-work-with-microsoft-teams"></a>Microsoft Graph API を使用して Microsoft Teams で作業する



Microsoft Teams は、Office 365 のチャットベースのワークスペースであり、チーム固有の予定表、ファイル、OneNote のノート、Planner のプラン、シフトのスケジュールなどへの組み込みのアクセスを提供します。

## <a name="key-resources-in-microsoft-teams"></a>Microsoft Teams の主なリソース

| リソース | メソッド |
|:---------------|:--------|
|[team](../resources/team.md)| [各自のチームの一覧表示](../api/user-list-joinedteams.md)、[すべてのチームの一覧表示](/graph/teams-list-all-teams)、[作成](../api/team-put-teams.md)、[読み取り](../api/team-get.md)、[更新](../api/team-update.md)、[削除](/graph/api/group-delete?view=graph-rest-1.0)、[複製](../api/team-clone.md)、[アーカイブ](../api/team-archive.md)、[アーカイブ解除](../api/team-unarchive.md) |
|[group](../resources/group.md)| [メンバーの追加](../api/group-post-members.md)、 [メンバーの削除](../api/group-delete-members.md)、[所有者の追加](../api/group-post-owners.md)、 [所有者の削除](../api/group-delete-owners.md)、[ファイルの取得](drive.md)、[ノートブックの取得](/graph/api/resources/notebook?view=graph-rest-1.0)、[プランの取得](plannergroup.md)、[予定表の取得](event.md) |
|[channel](../resources/channel.md)|[一覧表示](../api/channel-list.md)、[作成](../api/channel-post.md)、[読み取り](../api/channel-get.md)、[更新](../api/channel-patch.md)、[削除](../api/channel-delete.md)|
|[teamsTab](../resources/teamstab.md) |[一覧表示](../api/teamstab-list.md)、[作成](../api/teamstab-add.md)、[読み取り](../api/teamstab-get.md)、[更新](../api/teamstab-update.md)、[削除](../api/teamstab-delete.md) |
|[teamsApp](../resources/teamsapp.md)|[一覧表示](../api/teamsapp-list.md)、[公開](../api/teamsapp-publish.md)、[更新](../api/teamsapp-update.md)、[削除](../api/teamsapp-delete.md)|
|[teamsAppInstallation](../resources/teamsappinstallation.md)| [一覧表示](../api/teamsappinstallation-list.md)、[インストール](../api/teamsappinstallation-add.md)、[アップグレード](../api/teamsappinstallation-delete.md)、[削除](../api/teamsappinstallation-delete.md) |
| [chatMessage](/graph/api/resources/chatmessage?view=graph-rest-beta) (プレビュー)| [一覧表示](/graph/api/channel-list-messages?view=graph-rest-beta)、[送信](/graph/api/channel-post-messages?view=graph-rest-beta)、[読み取り](/graph/api/channel-get-message?view=graph-rest-beta) |
| [call](/graph/api/resources/call?view=graph-rest-beta) (プレビュー)| [応答](/graph/api/call-answer?view=graph-rest-beta)、[拒否](/graph/api/call-reject?view=graph-rest-beta)、[リダイレクト](/graph/api/call-redirect?view=graph-rest-beta)、[ミュート](/graph/api/call-mute?view=graph-rest-beta)、[ミュート解除](/graph/api/call-unmute?view=graph-rest-beta)、[メタデータ更新](/graph/api/call-updatemetadata?view=graph-rest-beta)、[画面共有の役割の変更](/graph/api/call-changescreensharingrole?view=graph-rest-beta)、[参加者の一覧表示](/graph/api/call-list-participants?view=graph-rest-beta)、[参加者の招待](/graph/api/participant-invite?view=graph-rest-beta)、[すべての参加者のミュート](/graph/api/participant-muteall?view=graph-rest-beta) |
|[schedule](/graph/api/resources/schedule?view=graph-rest-beta) (プレビュー)| [作成または置換](/graph/api/team-put-schedule?view=graph-rest-beta)、[取得](/graph/api/schedule-get?view=graph-rest-beta)、[共有](/graph/api/schedule-share?view=graph-rest-beta) |
|[schedulingGroup](/graph/api/resources/schedulinggroup?view=graph-rest-beta) (プレビュー)| [作成](/graph/api/schedule-post-schedulinggroups?view=graph-rest-beta)、[一覧表示](/graph/api/schedule-list-schedulinggroups?view=graph-rest-beta)、[取得](/graph/api/schedulinggroup-get?view=graph-rest-beta)、[置換](/graph/api/schedulinggroup-put?view=graph-rest-beta)、[削除](/graph/api/schedulinggroup-delete?view=graph-rest-beta) |
|[シフト](/graph/api/resources/shift?view=graph-rest-beta)(プレビュー)| [作成](/graph/api/schedule-post-shifts?view=graph-rest-beta)、[一覧表示](/graph/api/schedule-list-shifts?view=graph-rest-beta)、[取得](/graph/api/shift-get?view=graph-rest-beta)、[置換](/graph/api/shift-put?view=graph-rest-beta)、[削除](/graph/api/shift-delete?view=graph-rest-beta) |
|[timeOff](/graph/api/resources/timeoff?view=graph-rest-beta)(プレビュー)| [作成](/graph/api/schedule-post-timesoff?view=graph-rest-beta)、[一覧表示](/graph/api/schedule-list-timesoff?view=graph-rest-beta)、[取得](/graph/api/timeoff-get?view=graph-rest-beta)、[置換](/graph/api/timeoff-put?view=graph-rest-beta)、[削除](/graph/api/timeoff-delete?view=graph-rest-beta) |
|[timeOffReason](/graph/api/resources/timeoffreason?view=graph-rest-beta) (プレビュー)| [作成](/graph/api/schedule-post-timeoffreasons?view=graph-rest-beta)、[一覧表示](/graph/api/schedule-list-timeoffreasons?view=graph-rest-beta)、[取得](/graph/api/timeoffreason-get?view=graph-rest-beta)、[置換](/graph/api/timeoffreason-put?view=graph-rest-beta)、[削除](/graph/api/timeoffreason-delete?view=graph-rest-beta) |

## <a name="teams-and-groups"></a>チームとグループ

Microsoft Graph では、Microsoft Teams は [group](../resources/group.md) リソースとして表されます。 Microsoft Teams と Office 365 の両方のグループは、グループの共同作業のためのさまざまなニーズに対応します。 ほとんどのグループベースの機能 (グループの予定表、ファイル、ノート、写真、プランなど) は Microsoft Teams グループと Office 365 グループに適用されます。 [チーム](team.md) と Office 365 のグループの主な違いは、メンバー間のコミュニケション モードです。 チーム メンバーのコミュニケーションには、特定のチームのコンテキストで常設チャットが使用されます。 Office 365 グループのメンバーのコミュニケーションには、グループ会話 (Outlook のグループのコンテキストで行われるメールによる会話) が使用されます。

チームを持つすべてのグループでは **resourceProvisioningOptions** プロパティが "Team" に設定されています。 

>**注:** **Group.resourceProvisioningOptions** プロパティは変更可能です。
このコレクションで "Team" を追加または削除しないでください。このようにすると、すべてのチームを一覧表示するときに誤った結果が表示されます。

チームとグループの API レベルでの違いを以下に示します。

- 「[参加チームの一覧表示](../api/user-list-joinedteams.md)」メソッドは Microsoft Teams のみに適用されます。
- これらの API に関する[既知の問題](/graph/known-issues)も参照してください。

>注:(たとえば、Microsoft Teams で実行されるタブまたはボットの一部として) スタンドアロン アプリではなく Microsoft Teams アプリのグループ API を使用する場合、記事「Microsoft Teams ページで Microsoft Graph を使用する」のガイダンスに従ってください。

## <a name="membership-changes-in-microsoft-teams"></a>Microsoft Teams のメンバーシップの変更

メンバーと所有者をチームに追加するには、同一 ID の [group](../resources/group.md) のメンバーシップを変更します。

| ユース ケース      | 動詞      | URL |
| ------------------------------------- | ------------------------------------------------------------ | ------------------------------------------------------------ |
| [メンバーを追加する](../api/group-post-members.md)    | POST      | /groups/{id}/members/$ref  |
| [メンバーを削除する](../api/group-delete-members.md)   | DELETE    | /groups/{id}/members/{userId}/$ref |
| [所有者を追加する](../api/group-post-owners.md)     | POST       | /groups/{id}/owners/$ref |
| [所有者を削除する](../api/group-delete-owners.md) | DELETE    | /groups/{id}/owners/{userId}/$ref |
| [チームを更新する](../api/team-update.md)  | PATCH     | /teams/{id} |

所有者を追加するときには、そのユーザーをメンバーとして追加することをお勧めします。 チームの所有者がメンバーではない場合、所有権とメンバーシップの変更は Microsoft Teams にすぐに反映されないことがあります。 また、アプリと API によってその処理方法は異なります。 たとえば Microsoft Teams ではユーザーがメンバーまたは所有者のいずれであるチームが表示されますが、Microsoft Teams PowerShell コマンドレッドと /me/joinedTeams API ではユーザーがメンバーであるチームだけが表示されます。 混乱を避けるため、すべての所有者をメンバー一覧にも追加してください。 

既知の問題: DELETE /groups/{id}/owners を呼び出すと、/groups/{id}/members 一覧からもユーザーが削除される。 この問題を回避するには、所有者とメンバーの両方からユーザーを削除してから 10 秒待ち、その後メンバーにユーザーを再度追加することをお勧めします。

メンバーと所有者を追加または削除するときには、波かっこ { } で ID を囲まないでください。

| 速度 | 構文 | 
| ------ | ----- |
| 高速 | https://graph.microsoft.com/v1.0/groups/02bd9fd6-8f93-4758-87c3-1fb73740a315/members/48d31887-5fad-4d73-a9f5-3c356e68a038/$ref | 
| 低速 | https://graph.microsoft.com/v1.0/groups/{02bd9fd6-8f93-4758-87c3-1fb73740a315}/members/{48d31887-5fad-4d73-a9f5-3c356e68a038}/$ref | 

同様に、URL またはペイロードの `userId` が GUID ではなく UPN として表される場合、パフォーマンスが遅くなります。

| 速度 | 構文 | 
| ------ | ----- |
| 高速 | 48d31887-5fad-4d73-a9f5-3c356e68a038 | 
| 低速 | john@example.com | 

低速のパスをとる場合、現在のチーム メンバーまたは所有者が Microsoft Teams アプリケーション/ Web サイトにサインインすると、変更は 1 時間以内に反映されます。
Microsoft Teams アプリケーション/Web サイトにこれらのユーザーがサインインしていない場合、変更が反映されるのは、いずれかのユーザーがサインインしてから 1 時間後になります。

## <a name="see-also"></a>関連項目

- [Microsoft Teams API の概要](/graph/teams-concept-overview)
- サンプル コード: [Contoso エアライン](https://github.com/microsoftgraph/contoso-airlines-teams-sample)、[C# ミニサンプル](https://github.com/microsoftgraph/csharp-teams-sample-graph)
