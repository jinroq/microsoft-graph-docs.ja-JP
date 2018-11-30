---
title: Microsoft Graph API を使用して Microsoft Teams で作業する
description: マイクロソフト チームは、特定のチームの予定表、ファイル、ノート、プランナーの計画に組み込みのアクセスを提供する Office 365 でチャット ベース ワークスペースです。
ms.openlocfilehash: b42c33a34e0191eae236f675f29762834dfc29da
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27022106"
---
# <a name="use-the-microsoft-graph-api-to-work-with-microsoft-teams"></a>Microsoft Graph API を使用して Microsoft Teams で作業する



マイクロソフト チームは、特定のチームの予定表、ファイル、ノート、プランナーの計画に組み込みのアクセスを提供する Office 365 でチャット ベース ワークスペースです。

## <a name="key-resources-in-microsoft-teams"></a>マイクロソフトのチームで重要なリソース

| リソース | メソッド |
|:---------------|:--------|
|[チーム](../resources/team.md)| [チームの一覧を表示](../api/user-list-joinedteams.md)、[チームのすべてのリスト](/graph/teams-list-all-teams)、[作成](../api/team-put-teams.md)、[読み取り](../api/team-get.md)、[更新](../api/team-update.md)、[削除](/graph/api/group-delete?view=graph-rest-1.0)、[クローン](../api/team-clone.md)、[アーカイブ](../api/team-archive.md)、 [unarchive](../api/team-unarchive.md) |
|[group](../resources/group.md)| [メンバーを追加](../api/group-post-members.md) [メンバーを削除する](../api/group-delete-members.md)[所有者を追加](../api/group-post-owners.md) [所有者を削除](../api/group-delete-owners.md)[ファイルを取得](drive.md)[ノートブックを取得する](/graph/api/resources/notebook?view=graph-rest-1.0)[プランを取得](plannergroup.md)、[予定表の取得](event.md) |
|[チャネル](../resources/channel.md)|[リスト](../api/channel-list.md)、[作成](../api/channel-post.md)、[読み取り](../api/channel-get.md)、[更新](../api/channel-patch.md)、[削除](../api/channel-delete.md)|
|[teamsTab](../resources/teamstab.md) |[リスト](../api/teamstab-list.md)、[作成](../api/teamstab-add.md)、[読み取り](../api/teamstab-get.md)、[更新](../api/teamstab-update.md)、[削除](../api/teamstab-delete.md) |
|[teamsApp](../resources/teamsapp.md)|[リスト](../api/teamsapp-list.md)、[発行](../api/teamsapp-publish.md)、[更新](../api/teamsapp-update.md)、[削除](../api/teamsapp-delete.md)|
|[teamsAppInstallation](../resources/teamsappinstallation.md)| [ボックスの一覧](../api/teamsappinstallation-list.md)、[インストール](../api/teamsappinstallation-add.md)、[アップグレード](../api/teamsappinstallation-delete.md)、[削除](../api/teamsappinstallation-delete.md) |
| (プレビュー)[chatMessage](/graph/api/resources/chatmessage?view=graph-rest-beta)と[chatThread](/graph/api/resources/chatthread?view=graph-rest-beta) | [リスト](/graph/api/channel-list-messages?view=graph-rest-beta)、[作成](/graph/api/channel-post-chatthreads?view=graph-rest-beta)、[読み取り](/graph/api/channel-get-message?view=graph-rest-beta) |
| (プレビュー)[呼び出す](/graph/api/resources/call?view=graph-rest-beta) | [応答](/graph/api/call-answer?view=graph-rest-beta)、[拒否](/graph/api/call-reject?view=graph-rest-beta)、[リダイレクト](/graph/api/call-redirect?view=graph-rest-beta)、[ミュート](/graph/api/call-mute?view=graph-rest-beta)、[ミュートを解除](/graph/api/call-unmute?view=graph-rest-beta)[メタデータを更新](/graph/api/call-updatemetadata?view=graph-rest-beta)[画面を共有の役割を変更](/graph/api/call-changescreensharingrole?view=graph-rest-beta)[リストの参加者](/graph/api/call-list-participants?view=graph-rest-beta)[参加者を招待する](/graph/api/participant-invite?view=graph-rest-beta)、[参加者全員をミュート](/graph/api/participant-muteall?view=graph-rest-beta) |

## <a name="teams-and-groups"></a>チームとグループ

Microsoft Graph では、マイクロソフトのチームは、[グループ](../resources/group.md)・ リソースによって表されます。 マイクロソフトのチームと Office 365 の両方のグループは、グループの共同作業のさまざまなニーズに対応します。 グループ ベースのほぼすべての機能では、マイクロソフトのチームと Office 365 のグループ、グループの予定表、ファイル、メモ、写真、計画を適用しなど。 [チーム](team.md)とグループの間、Office 365 の主な違いは、メンバー間のコミュニケーションのモードです。 チーム メンバーは、特定のチームのコンテキストでの永続的なチャットで通信します。 Office 365 のグループのメンバーは、グループの会話は、Outlook 内のグループのコンテキストで発生する会話を電子メールで通信します。

チームを持つ任意のグループには、「チーム」が含まれている**resourceProvisioningOptions**プロパティがあります。 

>**注:****Group.resourceProvisioningOptions**プロパティを変更することができます。
追加またはそのコレクションから「チーム」を削除します。それ以外の場合、すべてのチームの一覧を表示すると誤った結果が得られます。

チームとグループの違いを API レベルでは、次のように。

- [ボックスの一覧には、チームが参加している](../api/user-list-joinedteams.md)メソッドは、マイクロソフトのチームにのみ適用されます。
- 参照の[既知の問題](/graph/known-issues)のこれらの Api です。

>**注:** タブまたはマイクロソフトのチームで実行されているボットの一部の例として API スタンドアロン アプリケーションではなく、[マイクロソフトのチームのアプリケーション](https://docs.microsoft.com/en-us/microsoftteams/platform/#apps-in-microsoft-teams)でのグループを使用する場合の[マイクロソフトのチームのページで Microsoft Graph を使用して](https://docs.microsoft.com/en-us/microsoftteams/platform/resources/microsoft-graph)この資料の指示に従います。

## <a name="membership-changes-in-microsoft-teams"></a>マイクロソフトのチームのメンバーシップを変更

チーム メンバーおよび所有者を追加するのには同じ ID を持つ[グループ](../resources/group.md)のメンバーシップを変更します。

| 使用例      | Verb      | URL |
| ------------------------------------- | ------------------------------------------------------------ | ------------------------------------------------------------ |
| [メンバーを追加する](../api/group-post-members.md)    | POST      | /groups/{id}/members/$ ref  |
| [メンバーを削除する](../api/group-delete-members.md)   | Delete    | /groups/{id}/members/{ユーザー Id}/$ref |
| [Add owner](../api/group-post-owners.md)     | POST       | /groups/{id}/owners/$ ref |
| [所有者を削除する](../api/group-delete-owners.md) | Delete    | /groups/{id}/owners/{ユーザー Id}/$ref |
| [チームを更新します。](../api/team-update.md)  | PATCH     | /teams/{id} |

所有者を追加するとするもそのユーザーのメンバーとして追加することをお勧めします。 チームの所有者は、メンバーではない場合は、所有権およびメンバーシップの変更がすぐに表示されないマイクロソフトのチームで。 さらに、別のアプリケーションと Api を処理するとは異なる。 たとえば、マイクロソフトのチームが表示されますチームのユーザーであるの所有者またはメンバーのいずれかマイクロソフト チームの PowerShell コマンドレットと私/joinedTeams API は、ユーザーのメンバーがチームを表示のみ。 混乱を避けるためには、メンバーの一覧にすべての所有者を追加します。 

既知の問題:/groups/id {0} を削除すると/所有者が呼び出されると、/groups/{id} からユーザーを削除するもとメンバーの一覧です。 この問題を回避するには、ことをお勧めこと所有者とメンバーの両方からユーザーを削除し、10 秒待ってからしてそれらをメンバーに追加します。

メンバーと所有者を追加および削除が配置されていない ID に {} を中かっこ

| Speed | 構文 | 
| ------ | ----- |
| 速く | https://graph.microsoft.com/v1.0/groups/02bd9fd6-8f93-4758-87c3-1fb73740a315/members/48d31887-5fad-4d73-a9f5-3c356e68a038/$ref | 
| 遅く | https://graph.microsoft.com/v1.0/groups/{02bd9fd6-8f93-4758-87c3-1fb73740a315}/members/{48d31887-5fad-4d73-a9f5-3c356e68a038}/$ref | 

同様に場合は、`userId`の URL またはペイロードとして表される UPN、パフォーマンスを低下する、GUID としてではなく。

| Speed | 構文 | 
| ------ | ----- |
| 速く | 48d31887-5fad-4d73-a9f5-3c356e68a038 | 
| 遅く | john@example.com | 

低速のパスを使用すると、現在のチーム メンバーまたは所有者が署名されている場合マイクロソフトのチームのアプリケーションと web サイトには、ときに、1 時間以内の変更が反映されます。
マイクロソフト チームのアプリケーションと web サイトにサインイン ユーザーの場合は 1 時間後、それらのいずれかがサインインするまで、変更は反映されません。

## <a name="see-also"></a>関連項目

- [マイクロソフト チームの API の概要](/graph/teams-concept-overview)
- サンプル コード: [contoso 社の航空会社](https://github.com/microsoftgraph/contoso-airlines-teams-sample)、 [C# サンプル ミニ](https://github.com/microsoftgraph/csharp-teams-sample-graph)
