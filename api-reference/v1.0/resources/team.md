---
title: team リソースの種類
description: 'Microsoft Teams のチームは、チャネルのコレクションです。 '
author: nkramer
localization_priority: Priority
ms.prod: microsoft-teams
ms.openlocfilehash: ff264052fd1a30c12935a3b7cf0d9e250597a434
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32534452"
---
# <a name="team-resource-type"></a><span data-ttu-id="2c8da-103">team リソースの種類</span><span class="sxs-lookup"><span data-stu-id="2c8da-103">team resource type</span></span>



<span data-ttu-id="2c8da-104">Microsoft Teams のチームは、[channel](channel.md) オブジェクトのコレクションです。</span><span class="sxs-lookup"><span data-stu-id="2c8da-104">A team in Microsoft Teams is a collection of [channel](channel.md) objects.</span></span> <span data-ttu-id="2c8da-105">チャネルは 1 つのトピック、つまりチーム内でのディスカッションの論理的分離を表します。</span><span class="sxs-lookup"><span data-stu-id="2c8da-105">A channel represents a topic, and therefore a logical isolation of discussion, within a team.</span></span>

<span data-ttu-id="2c8da-106">各チームには[グループ](../resources/group.md)が関連付けられています。</span><span class="sxs-lookup"><span data-stu-id="2c8da-106">Every team is associated with a [group](../resources/group.md).</span></span>
<span data-ttu-id="2c8da-107">グループの ID はチームと同じです。たとえば、/groups/{id}/team は /teams/{id} と同じです。</span><span class="sxs-lookup"><span data-stu-id="2c8da-107">The group has the same ID as the team - for example, /groups/{id}/team is the same as /teams/{id}.</span></span>
<span data-ttu-id="2c8da-108">チームのメンバーおよびグループの操作の詳細については、「[Microsoft Graph REST API を使用して Microsoft Teams を操作する](teams-api-overview.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="2c8da-108">For more information about working with groups and members in teams, see [Use the Microsoft Graph REST API to work with Microsoft Teams](teams-api-overview.md).</span></span>

## <a name="methods"></a><span data-ttu-id="2c8da-109">メソッド</span><span class="sxs-lookup"><span data-stu-id="2c8da-109">Methods</span></span>

| <span data-ttu-id="2c8da-110">メソッド</span><span class="sxs-lookup"><span data-stu-id="2c8da-110">Method</span></span>       | <span data-ttu-id="2c8da-111">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="2c8da-111">Return Type</span></span>  |<span data-ttu-id="2c8da-112">説明</span><span class="sxs-lookup"><span data-stu-id="2c8da-112">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="2c8da-113">チームを作成する</span><span class="sxs-lookup"><span data-stu-id="2c8da-113">Create team</span></span>](../api/team-put-teams.md) | [<span data-ttu-id="2c8da-114">team</span><span class="sxs-lookup"><span data-stu-id="2c8da-114">team</span></span>](team.md) | <span data-ttu-id="2c8da-115">新しいチームを作成するか、既存のグループにチームを追加します。</span><span class="sxs-lookup"><span data-stu-id="2c8da-115">Create a new team, or add a team to an existing group.</span></span>|
|[<span data-ttu-id="2c8da-116">チームを取得する</span><span class="sxs-lookup"><span data-stu-id="2c8da-116">Get team</span></span>](../api/team-get.md) | [<span data-ttu-id="2c8da-117">team</span><span class="sxs-lookup"><span data-stu-id="2c8da-117">team</span></span>](team.md) | <span data-ttu-id="2c8da-118">指定したチームのプロパティとリレーションシップを取得します。</span><span class="sxs-lookup"><span data-stu-id="2c8da-118">Retrieve the properties and relationships of the specified team.</span></span>|
|[<span data-ttu-id="2c8da-119">チームを更新する</span><span class="sxs-lookup"><span data-stu-id="2c8da-119">Update team</span></span>](../api/team-update.md) | [<span data-ttu-id="2c8da-120">team</span><span class="sxs-lookup"><span data-stu-id="2c8da-120">team</span></span>](team.md) |<span data-ttu-id="2c8da-121">指定されたチームのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="2c8da-121">Update the properties of the specified team.</span></span> |
|[<span data-ttu-id="2c8da-122">チームを削除する</span><span class="sxs-lookup"><span data-stu-id="2c8da-122">Delete team</span></span>](/graph/api/group-delete?view=graph-rest-1.0) | <span data-ttu-id="2c8da-123">なし</span><span class="sxs-lookup"><span data-stu-id="2c8da-123">None</span></span> |<span data-ttu-id="2c8da-124">チームとその関連グループを削除します。</span><span class="sxs-lookup"><span data-stu-id="2c8da-124">Delete the team and its associated group.</span></span> |
|[<span data-ttu-id="2c8da-125">チームを複製する</span><span class="sxs-lookup"><span data-stu-id="2c8da-125">Clone team</span></span>](../api/team-clone.md) | [<span data-ttu-id="2c8da-126">teamsAsyncOperation</span><span class="sxs-lookup"><span data-stu-id="2c8da-126">teamsAsyncOperation</span></span>](../resources/teamsasyncoperation.md) |<span data-ttu-id="2c8da-127">チームとその関連グループをコピーします。</span><span class="sxs-lookup"><span data-stu-id="2c8da-127">Copy the team and its associated group.</span></span> |
|[<span data-ttu-id="2c8da-128">チームをアーカイブする</span><span class="sxs-lookup"><span data-stu-id="2c8da-128">Archive team</span></span>](../api/team-archive.md) | [<span data-ttu-id="2c8da-129">teamsAsyncOperation</span><span class="sxs-lookup"><span data-stu-id="2c8da-129">teamsAsyncOperation</span></span>](../resources/teamsasyncoperation.md) |<span data-ttu-id="2c8da-130">チームを読み取り専用状態にします。</span><span class="sxs-lookup"><span data-stu-id="2c8da-130">Put the team in a read-only state.</span></span> |
|[<span data-ttu-id="2c8da-131">チームを展開する</span><span class="sxs-lookup"><span data-stu-id="2c8da-131">Unarchive team</span></span>](../api/team-unarchive.md) | [<span data-ttu-id="2c8da-132">teamsAsyncOperation</span><span class="sxs-lookup"><span data-stu-id="2c8da-132">teamsAsyncOperation</span></span>](../resources/teamsasyncoperation.md) |<span data-ttu-id="2c8da-133">チームを読み取り/書き込み状態に復元します。</span><span class="sxs-lookup"><span data-stu-id="2c8da-133">Restore the team to a read-write state.</span></span> |
|[<span data-ttu-id="2c8da-134">チームを一覧表示する</span><span class="sxs-lookup"><span data-stu-id="2c8da-134">List your teams</span></span>](../api/user-list-joinedteams.md) | <span data-ttu-id="2c8da-135">[team](team.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="2c8da-135">[team](team.md) collection</span></span> | <span data-ttu-id="2c8da-136">メンバーであるチームの一覧を表示します。</span><span class="sxs-lookup"><span data-stu-id="2c8da-136">List the teams you are a member of.</span></span> |
|[<span data-ttu-id="2c8da-137">すべてのチームのリストを作成する</span><span class="sxs-lookup"><span data-stu-id="2c8da-137">List all teams</span></span>](/graph/teams-list-all-teams) | <span data-ttu-id="2c8da-138">[group](group.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="2c8da-138">[group](group.md) collection</span></span> | <span data-ttu-id="2c8da-139">チームを持つすべてのグループを一覧表示します。</span><span class="sxs-lookup"><span data-stu-id="2c8da-139">List all groups that have teams.</span></span> |
|[<span data-ttu-id="2c8da-140">組織に対してアプリを公開する</span><span class="sxs-lookup"><span data-stu-id="2c8da-140">Publish apps to your organization</span></span>](../resources/teamsapp.md)| [<span data-ttu-id="2c8da-141">teamsApp</span><span class="sxs-lookup"><span data-stu-id="2c8da-141">teamsApp</span></span>](../resources/teamsapp.md) | <span data-ttu-id="2c8da-142">所属組織のみに表示する Teams アプリを作成します。</span><span class="sxs-lookup"><span data-stu-id="2c8da-142">Create Teams apps visible only to your organization.</span></span> |
|[<span data-ttu-id="2c8da-143">アプリをチームに追加する</span><span class="sxs-lookup"><span data-stu-id="2c8da-143">Add app to team</span></span>](../api/teamsappinstallation-add.md) | [<span data-ttu-id="2c8da-144">teamsAppInstallation</span><span class="sxs-lookup"><span data-stu-id="2c8da-144">teamsAppInstallation</span></span>](teamsappinstallation.md) | <span data-ttu-id="2c8da-145">アプリをチームに追加 (インストール) します。</span><span class="sxs-lookup"><span data-stu-id="2c8da-145">Adds (installs) an app to a team.</span></span>|
|[<span data-ttu-id="2c8da-146">チャネルにタブを追加する</span><span class="sxs-lookup"><span data-stu-id="2c8da-146">Add tab to channel</span></span>](../api/teamstab-add.md) | [<span data-ttu-id="2c8da-147">teamsTab</span><span class="sxs-lookup"><span data-stu-id="2c8da-147">teamsTab</span></span>](../resources/teamstab.md) | <span data-ttu-id="2c8da-148">タブをチームのチャネルに追加 (インストール) します。</span><span class="sxs-lookup"><span data-stu-id="2c8da-148">Adds (installs) a tab to a team's channel.</span></span>|

## <a name="properties"></a><span data-ttu-id="2c8da-149">プロパティ</span><span class="sxs-lookup"><span data-stu-id="2c8da-149">Properties</span></span>

| <span data-ttu-id="2c8da-150">プロパティ</span><span class="sxs-lookup"><span data-stu-id="2c8da-150">Property</span></span> | <span data-ttu-id="2c8da-151">型</span><span class="sxs-lookup"><span data-stu-id="2c8da-151">Type</span></span>   | <span data-ttu-id="2c8da-152">説明</span><span class="sxs-lookup"><span data-stu-id="2c8da-152">Description</span></span> |
|:---------------|:--------|:----------|
|<span data-ttu-id="2c8da-153">funSettings</span><span class="sxs-lookup"><span data-stu-id="2c8da-153">funSettings</span></span>|[<span data-ttu-id="2c8da-154">teamFunSettings</span><span class="sxs-lookup"><span data-stu-id="2c8da-154">teamFunSettings</span></span>](teamfunsettings.md) |<span data-ttu-id="2c8da-155">チームでの Giphy、ミーム、およびステッカーの使用を構成する設定。</span><span class="sxs-lookup"><span data-stu-id="2c8da-155">Settings to configure use of Giphy, memes, and stickers in the team.</span></span>|
|<span data-ttu-id="2c8da-156">guestSettings</span><span class="sxs-lookup"><span data-stu-id="2c8da-156">guestSettings</span></span>|[<span data-ttu-id="2c8da-157">teamGuestSettings</span><span class="sxs-lookup"><span data-stu-id="2c8da-157">teamGuestSettings</span></span>](teamguestsettings.md) |<span data-ttu-id="2c8da-158">ゲストがチームでチャネルを作成、更新、削除できるかどうかを構成する設定。</span><span class="sxs-lookup"><span data-stu-id="2c8da-158">Settings to configure whether guests can create, update, or delete channels in the team.</span></span>|
|<span data-ttu-id="2c8da-159">InternalId</span><span class="sxs-lookup"><span data-stu-id="2c8da-159">internalId</span></span> | <span data-ttu-id="2c8da-160">string</span><span class="sxs-lookup"><span data-stu-id="2c8da-160">string</span></span> | <span data-ttu-id="2c8da-161">監査ログまたは [Office 365 マネージメント アクティビティ API](https://docs.microsoft.com/ja-JP/office/office-365-management-api/office-365-management-activity-api-reference) など、いくつかの場所で使用されているチームの一意の ID。</span><span class="sxs-lookup"><span data-stu-id="2c8da-161">A unique ID for the team that has been used in a few places such as the audit log/[Office 365 Management Activity API](https://docs.microsoft.com/ja-JP/office/office-365-management-api/office-365-management-activity-api-reference).</span></span> |
|<span data-ttu-id="2c8da-162">isArchived</span><span class="sxs-lookup"><span data-stu-id="2c8da-162">isArchived</span></span>|<span data-ttu-id="2c8da-163">Boolean</span><span class="sxs-lookup"><span data-stu-id="2c8da-163">Boolean</span></span>|<span data-ttu-id="2c8da-164">このチームが読み取り専用モードかどうか。</span><span class="sxs-lookup"><span data-stu-id="2c8da-164">Whether this team is in read-only mode.</span></span> |
|<span data-ttu-id="2c8da-165">memberSettings</span><span class="sxs-lookup"><span data-stu-id="2c8da-165">memberSettings</span></span>|[<span data-ttu-id="2c8da-166">teamMemberSettings</span><span class="sxs-lookup"><span data-stu-id="2c8da-166">teamMemberSettings</span></span>](teammembersettings.md) |<span data-ttu-id="2c8da-167">メンバーが特定のアクション (チャネルの作成、ボットの追加など) をチーム内で実行できるかどうかを構成する設定。</span><span class="sxs-lookup"><span data-stu-id="2c8da-167">Settings to configure whether members can perform certain actions, for example, create channels and add bots, in the team.</span></span>|
|<span data-ttu-id="2c8da-168">messagingSettings</span><span class="sxs-lookup"><span data-stu-id="2c8da-168">messagingSettings</span></span>|[<span data-ttu-id="2c8da-169">teamMessagingSettings</span><span class="sxs-lookup"><span data-stu-id="2c8da-169">teamMessagingSettings</span></span>](teammessagingsettings.md) |<span data-ttu-id="2c8da-170">チームでメッセージとメンションを構成する設定。</span><span class="sxs-lookup"><span data-stu-id="2c8da-170">Settings to configure messaging and mentions in the team.</span></span>|
|<span data-ttu-id="2c8da-171">webUrl</span><span class="sxs-lookup"><span data-stu-id="2c8da-171">webUrl</span></span>|<span data-ttu-id="2c8da-172">string (読み取り専用)</span><span class="sxs-lookup"><span data-stu-id="2c8da-172">string (readonly)</span></span> | <span data-ttu-id="2c8da-173">Microsoft Teams クライアントのチームに移動するハイパーリンク。</span><span class="sxs-lookup"><span data-stu-id="2c8da-173">A hyperlink that will go to the team in the Microsoft Teams client.</span></span> <span data-ttu-id="2c8da-174">これは、Microsoft Teams クライアントでチームを右クリックし、**[Get link to team]** を選択すると作成される URL です。</span><span class="sxs-lookup"><span data-stu-id="2c8da-174">This is the URL that you get when you right-click a team in the Microsoft Teams client and select **Get link to team**.</span></span> <span data-ttu-id="2c8da-175">この URL は不透明 blob として扱われる必要があり、また解析されません。</span><span class="sxs-lookup"><span data-stu-id="2c8da-175">This URL should be treated as an opaque blob, and not parsed.</span></span> |

## <a name="relationships"></a><span data-ttu-id="2c8da-176">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="2c8da-176">Relationships</span></span>

| <span data-ttu-id="2c8da-177">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="2c8da-177">Relationship</span></span> | <span data-ttu-id="2c8da-178">型</span><span class="sxs-lookup"><span data-stu-id="2c8da-178">Type</span></span>   | <span data-ttu-id="2c8da-179">説明</span><span class="sxs-lookup"><span data-stu-id="2c8da-179">Description</span></span> |
|:---------------|:--------|:----------|
|<span data-ttu-id="2c8da-180">channels</span><span class="sxs-lookup"><span data-stu-id="2c8da-180">channels</span></span>|<span data-ttu-id="2c8da-181">[channel](channel.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="2c8da-181">[channel](channel.md) collection</span></span>|<span data-ttu-id="2c8da-182">チームに関連付けられているチャネルとメッセージのコレクション。</span><span class="sxs-lookup"><span data-stu-id="2c8da-182">The collection of channels & messages associated with the team.</span></span>|
|<span data-ttu-id="2c8da-183">installedApps</span><span class="sxs-lookup"><span data-stu-id="2c8da-183">installedApps</span></span>|<span data-ttu-id="2c8da-184">[teamsAppInstallation](teamsappinstallation.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="2c8da-184">[teamsAppInstallation](teamsappinstallation.md) collection</span></span>|<span data-ttu-id="2c8da-185">このチームにインストールされているアプリ。</span><span class="sxs-lookup"><span data-stu-id="2c8da-185">The apps installed in this team.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="2c8da-186">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="2c8da-186">JSON representation</span></span>

<span data-ttu-id="2c8da-187">リソースの JSON 表記を次に示します。</span><span class="sxs-lookup"><span data-stu-id="2c8da-187">The following is a JSON representation of the resource.</span></span>

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
  "internalId": "string",
  "isArchived": false,
  "webUrl": "string (URL)"
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

## <a name="see-also"></a><span data-ttu-id="2c8da-188">関連項目</span><span class="sxs-lookup"><span data-stu-id="2c8da-188">See Also</span></span>
- [<span data-ttu-id="2c8da-189">チームを使用してグループを作成する</span><span class="sxs-lookup"><span data-stu-id="2c8da-189">Creating a group with a team</span></span>](/graph/teams-create-group-and-team)
- [<span data-ttu-id="2c8da-190">Teams API を使用する</span><span class="sxs-lookup"><span data-stu-id="2c8da-190">Using Teams APIs</span></span>](teams-api-overview.md)
