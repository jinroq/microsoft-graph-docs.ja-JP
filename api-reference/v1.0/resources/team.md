---
title: team リソースの種類
description: 'Microsoft Teams のチームは、チャネルのコレクションです。 '
author: nkramer
localization_priority: Priority
ms.prod: microsoft-teams
ms.openlocfilehash: 7c3dd42c25ce8c48722ab857f61e0c6a9a275581
ms.sourcegitcommit: 7b98b61db7cdbaff037e1b222ac58eef4c5bee89
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 03/29/2019
ms.locfileid: "30964137"
---
# <a name="team-resource-type"></a><span data-ttu-id="4151a-103">team リソースの種類</span><span class="sxs-lookup"><span data-stu-id="4151a-103">team resource type</span></span>



<span data-ttu-id="4151a-104">Microsoft Teams のチームは、[channel](channel.md) オブジェクトのコレクションです。</span><span class="sxs-lookup"><span data-stu-id="4151a-104">A team in Microsoft Teams is a collection of [channels](channel.md).</span></span> <span data-ttu-id="4151a-105">チャネルは 1 つのトピック、つまりチーム内でのディスカッションの論理的分離を表します。</span><span class="sxs-lookup"><span data-stu-id="4151a-105">A channel represents a topic, and therefore a logical isolation of discussion, within a team.</span></span>

<span data-ttu-id="4151a-106">各チームには[グループ](../resources/group.md)が関連付けられています。</span><span class="sxs-lookup"><span data-stu-id="4151a-106">Every team is associated with a [group](../resources/group.md).</span></span>
<span data-ttu-id="4151a-107">グループの ID はチームと同じです。たとえば、/groups/{id}/team は /teams/{id} と同じです。</span><span class="sxs-lookup"><span data-stu-id="4151a-107">The group has the same ID as the team - for example, /groups/{id}/team is the same as /teams/{id}.</span></span>
<span data-ttu-id="4151a-108">チームのメンバーおよびグループの操作の詳細については、「[Microsoft Graph REST API を使用して Microsoft Teams を操作する](teams-api-overview.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="4151a-108">For more information about working with groups and members in teams, see [Use the Microsoft Graph REST API to work with Microsoft Teams](teams-api-overview.md).</span></span>

## <a name="methods"></a><span data-ttu-id="4151a-109">メソッド</span><span class="sxs-lookup"><span data-stu-id="4151a-109">Methods</span></span>

| <span data-ttu-id="4151a-110">メソッド</span><span class="sxs-lookup"><span data-stu-id="4151a-110">Method</span></span>       | <span data-ttu-id="4151a-111">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="4151a-111">Return Type</span></span>  |<span data-ttu-id="4151a-112">説明</span><span class="sxs-lookup"><span data-stu-id="4151a-112">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="4151a-113">チームを作成する</span><span class="sxs-lookup"><span data-stu-id="4151a-113">Create team</span></span>](../api/team-put-teams.md) | [<span data-ttu-id="4151a-114">team</span><span class="sxs-lookup"><span data-stu-id="4151a-114">team</span></span>](team.md) | <span data-ttu-id="4151a-115">新しいチームを作成するか、既存のグループにチームを追加します。</span><span class="sxs-lookup"><span data-stu-id="4151a-115">Create a new team, or add a team to an existing group.</span></span>|
|[<span data-ttu-id="4151a-116">チームを取得する</span><span class="sxs-lookup"><span data-stu-id="4151a-116">Get team</span></span>](../api/team-get.md) | [<span data-ttu-id="4151a-117">team</span><span class="sxs-lookup"><span data-stu-id="4151a-117">team</span></span>](team.md) | <span data-ttu-id="4151a-118">指定したチームのプロパティとリレーションシップを取得します。</span><span class="sxs-lookup"><span data-stu-id="4151a-118">Retrieve the properties and relationships of the specified team.</span></span>|
|[<span data-ttu-id="4151a-119">チームを更新する</span><span class="sxs-lookup"><span data-stu-id="4151a-119">Update team</span></span>](../api/team-update.md) | [<span data-ttu-id="4151a-120">team</span><span class="sxs-lookup"><span data-stu-id="4151a-120">team</span></span>](team.md) |<span data-ttu-id="4151a-121">指定されたチームのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="4151a-121">Update the properties of the specified team.</span></span> |
|[<span data-ttu-id="4151a-122">チームを削除する</span><span class="sxs-lookup"><span data-stu-id="4151a-122">Delete team</span></span>](/graph/api/group-delete?view=graph-rest-1.0) | <span data-ttu-id="4151a-123">なし</span><span class="sxs-lookup"><span data-stu-id="4151a-123">None</span></span> |<span data-ttu-id="4151a-124">チームとその関連グループを削除します。</span><span class="sxs-lookup"><span data-stu-id="4151a-124">Delete the team and its associated group.</span></span> |
|[<span data-ttu-id="4151a-125">チームを複製する</span><span class="sxs-lookup"><span data-stu-id="4151a-125">Clone team</span></span>](../api/team-clone.md) | [<span data-ttu-id="4151a-126">teamsAsyncOperation</span><span class="sxs-lookup"><span data-stu-id="4151a-126">teamsAsyncOperation</span></span>](../resources/teamsasyncoperation.md) |<span data-ttu-id="4151a-127">チームとその関連グループをコピーします。</span><span class="sxs-lookup"><span data-stu-id="4151a-127">Copy the team and its associated group.</span></span> |
|[<span data-ttu-id="4151a-128">チームをアーカイブする</span><span class="sxs-lookup"><span data-stu-id="4151a-128">Archive team</span></span>](../api/team-archive.md) | [<span data-ttu-id="4151a-129">teamsAsyncOperation</span><span class="sxs-lookup"><span data-stu-id="4151a-129">teamsAsyncOperation</span></span>](../resources/teamsasyncoperation.md) |<span data-ttu-id="4151a-130">チームを読み取り専用状態にします。</span><span class="sxs-lookup"><span data-stu-id="4151a-130">Put the team in a read-only state.</span></span> |
|[<span data-ttu-id="4151a-131">チームを展開する</span><span class="sxs-lookup"><span data-stu-id="4151a-131">Unarchive team</span></span>](../api/team-unarchive.md) | [<span data-ttu-id="4151a-132">teamsAsyncOperation</span><span class="sxs-lookup"><span data-stu-id="4151a-132">teamsAsyncOperation</span></span>](../resources/teamsasyncoperation.md) |<span data-ttu-id="4151a-133">チームを読み取り/書き込み状態に復元します。</span><span class="sxs-lookup"><span data-stu-id="4151a-133">Restore the team to a read-write state.</span></span> |
|[<span data-ttu-id="4151a-134">チームを一覧表示する</span><span class="sxs-lookup"><span data-stu-id="4151a-134">List your teams</span></span>](../api/user-list-joinedteams.md) | <span data-ttu-id="4151a-135">[team](team.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="4151a-135">[team](team.md) collection</span></span> | <span data-ttu-id="4151a-136">メンバーであるチームの一覧を表示します。</span><span class="sxs-lookup"><span data-stu-id="4151a-136">List the teams you are a member of.</span></span> |
|[<span data-ttu-id="4151a-137">すべてのチームのリストを作成する</span><span class="sxs-lookup"><span data-stu-id="4151a-137">List all teams</span></span>](/graph/teams-list-all-teams) | <span data-ttu-id="4151a-138">[group](group.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="4151a-138">[group](group.md) collection</span></span> | <span data-ttu-id="4151a-139">チームを持つすべてのグループを一覧表示します。</span><span class="sxs-lookup"><span data-stu-id="4151a-139">List all groups that have teams.</span></span> |
|[<span data-ttu-id="4151a-140">組織に対してアプリを公開する</span><span class="sxs-lookup"><span data-stu-id="4151a-140">Publish apps to your organization</span></span>](../resources/teamsapp.md)| [<span data-ttu-id="4151a-141">teamsApp</span><span class="sxs-lookup"><span data-stu-id="4151a-141">teamsApp</span></span>](../resources/teamsapp.md) | <span data-ttu-id="4151a-142">所属組織のみに表示する Teams アプリを作成します。</span><span class="sxs-lookup"><span data-stu-id="4151a-142">Create Teams apps visible only to your organization.</span></span> |
|[<span data-ttu-id="4151a-143">アプリをチームに追加する</span><span class="sxs-lookup"><span data-stu-id="4151a-143">Add app to team</span></span>](../api/teamsappinstallation-add.md) | [<span data-ttu-id="4151a-144">teamsAppInstallation</span><span class="sxs-lookup"><span data-stu-id="4151a-144">teamsAppInstallation</span></span>](teamsappinstallation.md) | <span data-ttu-id="4151a-145">アプリをチームに追加 (インストール) します。</span><span class="sxs-lookup"><span data-stu-id="4151a-145">Adds (installs) an app to a team.</span></span>|
|[<span data-ttu-id="4151a-146">チャネルにタブを追加する</span><span class="sxs-lookup"><span data-stu-id="4151a-146">Add tab to channel</span></span>](../api/teamstab-add.md) | [<span data-ttu-id="4151a-147">teamsTab</span><span class="sxs-lookup"><span data-stu-id="4151a-147">teamsTab</span></span>](../resources/teamstab.md) | <span data-ttu-id="4151a-148">タブをチームのチャネルに追加 (インストール) します。</span><span class="sxs-lookup"><span data-stu-id="4151a-148">Adds (installs) a tab to a team's channel.</span></span>|

## <a name="properties"></a><span data-ttu-id="4151a-149">プロパティ</span><span class="sxs-lookup"><span data-stu-id="4151a-149">Properties</span></span>

| <span data-ttu-id="4151a-150">プロパティ</span><span class="sxs-lookup"><span data-stu-id="4151a-150">Property</span></span> | <span data-ttu-id="4151a-151">型</span><span class="sxs-lookup"><span data-stu-id="4151a-151">Type</span></span>   | <span data-ttu-id="4151a-152">説明</span><span class="sxs-lookup"><span data-stu-id="4151a-152">Description</span></span> |
|:---------------|:--------|:----------|
|<span data-ttu-id="4151a-153">funSettings</span><span class="sxs-lookup"><span data-stu-id="4151a-153">funSettings</span></span>|[<span data-ttu-id="4151a-154">teamFunSettings</span><span class="sxs-lookup"><span data-stu-id="4151a-154">teamFunSettings</span></span>](teamfunsettings.md) |<span data-ttu-id="4151a-155">チームでの Giphy、ミーム、およびステッカーの使用を構成する設定。</span><span class="sxs-lookup"><span data-stu-id="4151a-155">Settings to configure use of Giphy, memes, and stickers in the team.</span></span>|
|<span data-ttu-id="4151a-156">guestSettings</span><span class="sxs-lookup"><span data-stu-id="4151a-156">guestSettings</span></span>|[<span data-ttu-id="4151a-157">teamGuestSettings</span><span class="sxs-lookup"><span data-stu-id="4151a-157">teamGuestSettings</span></span>](teamguestsettings.md) |<span data-ttu-id="4151a-158">ゲストがチームでチャネルを作成、更新、削除できるかどうかを構成する設定。</span><span class="sxs-lookup"><span data-stu-id="4151a-158">Settings to configure whether guests can create, update, or delete channels in the team.</span></span>|
|<span data-ttu-id="4151a-159">InternalId</span><span class="sxs-lookup"><span data-stu-id="4151a-159">internalId</span></span> | <span data-ttu-id="4151a-160">string</span><span class="sxs-lookup"><span data-stu-id="4151a-160">string</span></span> | <span data-ttu-id="4151a-161">監査ログまたは [Office 365 マネージメント アクティビティ API](https://docs.microsoft.com/ja-JP/office/office-365-management-api/office-365-management-activity-api-reference) など、いくつかの場所で使用されているチームの一意の ID。</span><span class="sxs-lookup"><span data-stu-id="4151a-161">A unique ID for the team that has been used in a few places such as the audit log/[Office 365 Management Activity API](https://docs.microsoft.com/ja-JP/office/office-365-management-api/office-365-management-activity-api-reference).</span></span> |
|<span data-ttu-id="4151a-162">isArchived</span><span class="sxs-lookup"><span data-stu-id="4151a-162">isArchived</span></span>|<span data-ttu-id="4151a-163">Boolean</span><span class="sxs-lookup"><span data-stu-id="4151a-163">Boolean</span></span>|<span data-ttu-id="4151a-164">このチームが読み取り専用モードかどうか。</span><span class="sxs-lookup"><span data-stu-id="4151a-164">Whether this team is in read-only mode.</span></span> |
|<span data-ttu-id="4151a-165">memberSettings</span><span class="sxs-lookup"><span data-stu-id="4151a-165">memberSettings</span></span>|[<span data-ttu-id="4151a-166">teamMemberSettings</span><span class="sxs-lookup"><span data-stu-id="4151a-166">teamMemberSettings</span></span>](teammembersettings.md) |<span data-ttu-id="4151a-167">メンバーが特定のアクション (チャネルの作成、ボットの追加など) をチーム内で実行できるかどうかを構成する設定。</span><span class="sxs-lookup"><span data-stu-id="4151a-167">Settings to configure whether members can perform certain actions, for example, create channels and add bots, in the team.</span></span>|
|<span data-ttu-id="4151a-168">messagingSettings</span><span class="sxs-lookup"><span data-stu-id="4151a-168">messagingSettings</span></span>|[<span data-ttu-id="4151a-169">teamMessagingSettings</span><span class="sxs-lookup"><span data-stu-id="4151a-169">teamMessagingSettings</span></span>](teammessagingsettings.md) |<span data-ttu-id="4151a-170">チームでメッセージとメンションを構成する設定。</span><span class="sxs-lookup"><span data-stu-id="4151a-170">Settings to configure messaging and mentions in the team.</span></span>|
|<span data-ttu-id="4151a-171">webUrl</span><span class="sxs-lookup"><span data-stu-id="4151a-171">webUrl</span></span>|<span data-ttu-id="4151a-172">string (読み取り専用)</span><span class="sxs-lookup"><span data-stu-id="4151a-172">string (readonly)</span></span> | <span data-ttu-id="4151a-173">Microsoft Teams クライアントのチームに移動するハイパーリンク。</span><span class="sxs-lookup"><span data-stu-id="4151a-173">A hyperlink that will go to the team in the Microsoft Teams client.</span></span> <span data-ttu-id="4151a-174">これは、Microsoft Teams クライアントでチームを右クリックし、**[Get link to team]** を選択すると作成される URL です。</span><span class="sxs-lookup"><span data-stu-id="4151a-174">This is the URL that you get when you right-click a team in the Microsoft Teams client and select **Get link to team**.</span></span> <span data-ttu-id="4151a-175">この URL は不透明 blob として扱われる必要があり、また解析されません。</span><span class="sxs-lookup"><span data-stu-id="4151a-175">This URL should be treated as an opaque blob, and not parsed.</span></span> |

## <a name="relationships"></a><span data-ttu-id="4151a-176">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="4151a-176">Relationships</span></span>

| <span data-ttu-id="4151a-177">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="4151a-177">Relationship</span></span> | <span data-ttu-id="4151a-178">型</span><span class="sxs-lookup"><span data-stu-id="4151a-178">Type</span></span>   | <span data-ttu-id="4151a-179">説明</span><span class="sxs-lookup"><span data-stu-id="4151a-179">Description</span></span> |
|:---------------|:--------|:----------|
|<span data-ttu-id="4151a-180">channels</span><span class="sxs-lookup"><span data-stu-id="4151a-180">channels</span></span>|<span data-ttu-id="4151a-181">[channel](channel.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="4151a-181">[channel](channel.md) collection</span></span>|<span data-ttu-id="4151a-182">チームに関連付けられているチャネルとメッセージのコレクション。</span><span class="sxs-lookup"><span data-stu-id="4151a-182">The collection of channels & messages associated with the team.</span></span>|
|<span data-ttu-id="4151a-183">installedApps</span><span class="sxs-lookup"><span data-stu-id="4151a-183">installedApps</span></span>|<span data-ttu-id="4151a-184">[teamsAppInstallation](teamsappinstallation.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="4151a-184">[teamsAppInstallation](teamsappinstallation.md) collection</span></span>|<span data-ttu-id="4151a-185">このチームにインストールされているアプリ。</span><span class="sxs-lookup"><span data-stu-id="4151a-185">The apps installed in this team.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="4151a-186">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="4151a-186">JSON representation</span></span>

<span data-ttu-id="4151a-187">リソースの JSON 表記を次に示します。</span><span class="sxs-lookup"><span data-stu-id="4151a-187">The following is a JSON representation of the resource.</span></span>

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
<!-- {
  "type": "#page.annotation",
  "description": "team resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

## <a name="see-also"></a><span data-ttu-id="4151a-188">関連項目</span><span class="sxs-lookup"><span data-stu-id="4151a-188">See Also</span></span>
- [<span data-ttu-id="4151a-189">チームを使用してグループを作成する</span><span class="sxs-lookup"><span data-stu-id="4151a-189">Creating a group with a team</span></span>](/graph/teams-create-group-and-team)
- [<span data-ttu-id="4151a-190">Teams API を使用する</span><span class="sxs-lookup"><span data-stu-id="4151a-190">Using Teams APIs</span></span>](teams-api-overview.md)
