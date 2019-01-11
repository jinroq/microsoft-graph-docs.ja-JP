---
title: チーム リソースの種類
description: 'マイクロソフトのチームで、チームは、チャネルのコレクションです。 '
author: nkramer
localization_priority: Priority
ms.openlocfilehash: 85694e18771ac17873f97cedf68d074ee550f787
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/11/2019
ms.locfileid: "27878548"
---
# <a name="team-resource-type"></a><span data-ttu-id="8c6aa-103">チーム リソースの種類</span><span class="sxs-lookup"><span data-stu-id="8c6aa-103">team resource type</span></span>



<span data-ttu-id="8c6aa-104">マイクロソフトのチームで、チームは、[チャネル](channel.md)のコレクションです。</span><span class="sxs-lookup"><span data-stu-id="8c6aa-104">A team in Microsoft Teams is a collection of [channels](channel.md).</span></span> <span data-ttu-id="8c6aa-105">チャネルでは、トピックとチーム内での議論の論理的分離を表します。</span><span class="sxs-lookup"><span data-stu-id="8c6aa-105">A channel represents a topic, and therefore a logical isolation of discussion, within a team.</span></span>

<span data-ttu-id="8c6aa-106">すべてのチームは、[グループ](../resources/group.md)に関連付けられます。</span><span class="sxs-lookup"><span data-stu-id="8c6aa-106">Every team is associated with a [group](../resources/group.md).</span></span>
<span data-ttu-id="8c6aa-107">グループは、チーム ・/groups/{id} などと同じ ID を持っているし、チームは、/teams/{id} と同じです。</span><span class="sxs-lookup"><span data-stu-id="8c6aa-107">The group has the same ID as the team - for example, /groups/{id}/team is the same as /teams/{id}.</span></span>
<span data-ttu-id="8c6aa-108">グループとチームのメンバーの詳細については、[マイクロソフトのチームで作業するのには Microsoft グラフ REST API を使用](teams-api-overview.md)を参照してください。</span><span class="sxs-lookup"><span data-stu-id="8c6aa-108">For more information about working with groups and members in teams, see [Use the Microsoft Graph REST API to work with Microsoft Teams](teams-api-overview.md).</span></span>

## <a name="methods"></a><span data-ttu-id="8c6aa-109">メソッド</span><span class="sxs-lookup"><span data-stu-id="8c6aa-109">Methods</span></span>

| <span data-ttu-id="8c6aa-110">メソッド</span><span class="sxs-lookup"><span data-stu-id="8c6aa-110">Method</span></span>       | <span data-ttu-id="8c6aa-111">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="8c6aa-111">Return Type</span></span>  |<span data-ttu-id="8c6aa-112">説明</span><span class="sxs-lookup"><span data-stu-id="8c6aa-112">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="8c6aa-113">チームを作成します。</span><span class="sxs-lookup"><span data-stu-id="8c6aa-113">Create team</span></span>](../api/team-put-teams.md) | [<span data-ttu-id="8c6aa-114">チーム</span><span class="sxs-lookup"><span data-stu-id="8c6aa-114">team</span></span>](team.md) | <span data-ttu-id="8c6aa-115">新しいチームを作成または既存のグループにチームを追加します。</span><span class="sxs-lookup"><span data-stu-id="8c6aa-115">Create a new team, or add a team to an existing group.</span></span>|
|[<span data-ttu-id="8c6aa-116">チームを取得します。</span><span class="sxs-lookup"><span data-stu-id="8c6aa-116">Get team</span></span>](../api/team-get.md) | [<span data-ttu-id="8c6aa-117">チーム</span><span class="sxs-lookup"><span data-stu-id="8c6aa-117">team</span></span>](team.md) | <span data-ttu-id="8c6aa-118">プロパティと指定されたチームの関係を取得します。</span><span class="sxs-lookup"><span data-stu-id="8c6aa-118">Retrieve the properties and relationships of the specified team.</span></span>|
|[<span data-ttu-id="8c6aa-119">チームを更新します。</span><span class="sxs-lookup"><span data-stu-id="8c6aa-119">Update team</span></span>](../api/team-update.md) | [<span data-ttu-id="8c6aa-120">チーム</span><span class="sxs-lookup"><span data-stu-id="8c6aa-120">team</span></span>](team.md) |<span data-ttu-id="8c6aa-121">指定されたチームのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="8c6aa-121">Update the properties of the specified team.</span></span> |
|[<span data-ttu-id="8c6aa-122">チームを削除します。</span><span class="sxs-lookup"><span data-stu-id="8c6aa-122">Delete team</span></span>](/graph/api/group-delete?view=graph-rest-1.0) | <span data-ttu-id="8c6aa-123">なし</span><span class="sxs-lookup"><span data-stu-id="8c6aa-123">None</span></span> |<span data-ttu-id="8c6aa-124">チームおよびその関連付けられているグループを削除します。</span><span class="sxs-lookup"><span data-stu-id="8c6aa-124">Delete the team and its associated group.</span></span> |
|[<span data-ttu-id="8c6aa-125">チームのクローンを作成します。</span><span class="sxs-lookup"><span data-stu-id="8c6aa-125">Clone team</span></span>](../api/team-clone.md) | [<span data-ttu-id="8c6aa-126">teamsAsyncOperation</span><span class="sxs-lookup"><span data-stu-id="8c6aa-126">teamsAsyncOperation</span></span>](../resources/teamsasyncoperation.md) |<span data-ttu-id="8c6aa-127">チームおよびその関連付けられているグループをコピーします。</span><span class="sxs-lookup"><span data-stu-id="8c6aa-127">Copy the team and its associated group.</span></span> |
|[<span data-ttu-id="8c6aa-128">チームのアーカイブ</span><span class="sxs-lookup"><span data-stu-id="8c6aa-128">Archive team</span></span>](../api/team-archive.md) | [<span data-ttu-id="8c6aa-129">teamsAsyncOperation</span><span class="sxs-lookup"><span data-stu-id="8c6aa-129">teamsAsyncOperation</span></span>](../resources/teamsasyncoperation.md) |<span data-ttu-id="8c6aa-130">読み取り専用状態で、チームを配置します。</span><span class="sxs-lookup"><span data-stu-id="8c6aa-130">Put the team in a read-only state.</span></span> |
|[<span data-ttu-id="8c6aa-131">チームを unarchive します。</span><span class="sxs-lookup"><span data-stu-id="8c6aa-131">Unarchive team</span></span>](../api/team-unarchive.md) | [<span data-ttu-id="8c6aa-132">teamsAsyncOperation</span><span class="sxs-lookup"><span data-stu-id="8c6aa-132">teamsAsyncOperation</span></span>](../resources/teamsasyncoperation.md) |<span data-ttu-id="8c6aa-133">チームを読み取り/書き込み状態に復元します。</span><span class="sxs-lookup"><span data-stu-id="8c6aa-133">Restore the team to a read-write state.</span></span> |
|[<span data-ttu-id="8c6aa-134">チームの一覧を表示します。</span><span class="sxs-lookup"><span data-stu-id="8c6aa-134">List your teams</span></span>](../api/user-list-joinedteams.md) | <span data-ttu-id="8c6aa-135">[チーム](team.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="8c6aa-135">[team](team.md) collection</span></span> | <span data-ttu-id="8c6aa-136">チームのメンバーを一覧表示します。</span><span class="sxs-lookup"><span data-stu-id="8c6aa-136">List the teams you are a member of.</span></span> |
|[<span data-ttu-id="8c6aa-137">すべてのチームをリストします。</span><span class="sxs-lookup"><span data-stu-id="8c6aa-137">List all teams</span></span>](/graph/teams-list-all-teams) | <span data-ttu-id="8c6aa-138">[group](group.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="8c6aa-138">[group](group.md) collection</span></span> | <span data-ttu-id="8c6aa-139">チームのすべてのグループを一覧表示します。</span><span class="sxs-lookup"><span data-stu-id="8c6aa-139">List all groups that have teams.</span></span> |
|[<span data-ttu-id="8c6aa-140">組織にアプリケーションを発行します。</span><span class="sxs-lookup"><span data-stu-id="8c6aa-140">Publish apps to your organization</span></span>](../resources/teamsapp.md)| [<span data-ttu-id="8c6aa-141">teamsApp</span><span class="sxs-lookup"><span data-stu-id="8c6aa-141">teamsApp</span></span>](../resources/teamsapp.md) | <span data-ttu-id="8c6aa-142">組織にのみ表示されているチームのアプリケーションを作成します。</span><span class="sxs-lookup"><span data-stu-id="8c6aa-142">Create Teams apps visible only to your organization.</span></span> |
|[<span data-ttu-id="8c6aa-143">アプリケーションをチームに追加します。</span><span class="sxs-lookup"><span data-stu-id="8c6aa-143">Add app to team</span></span>](../api/teamsappinstallation-add.md) | [<span data-ttu-id="8c6aa-144">teamsappinstallation</span><span class="sxs-lookup"><span data-stu-id="8c6aa-144">teamsappinstallation</span></span>](teamsappinstallation.md) | <span data-ttu-id="8c6aa-145">(インストール) を追加するチームにアプリです。</span><span class="sxs-lookup"><span data-stu-id="8c6aa-145">Adds (installs) an app to a team.</span></span>|
|[<span data-ttu-id="8c6aa-146">チャネルにタブを追加します。</span><span class="sxs-lookup"><span data-stu-id="8c6aa-146">Add tab to channel</span></span>](../api/teamstab-add.md) | [<span data-ttu-id="8c6aa-147">teamsTab</span><span class="sxs-lookup"><span data-stu-id="8c6aa-147">teamsTab</span></span>](../resources/teamstab.md) | <span data-ttu-id="8c6aa-148">(インストール) を追加するチャネル ・ チームのタブです。</span><span class="sxs-lookup"><span data-stu-id="8c6aa-148">Adds (installs) a tab to a team's channel.</span></span>|

## <a name="properties"></a><span data-ttu-id="8c6aa-149">プロパティ</span><span class="sxs-lookup"><span data-stu-id="8c6aa-149">Properties</span></span>

| <span data-ttu-id="8c6aa-150">プロパティ</span><span class="sxs-lookup"><span data-stu-id="8c6aa-150">Property</span></span> | <span data-ttu-id="8c6aa-151">種類</span><span class="sxs-lookup"><span data-stu-id="8c6aa-151">Type</span></span>   | <span data-ttu-id="8c6aa-152">説明</span><span class="sxs-lookup"><span data-stu-id="8c6aa-152">Description</span></span> |
|:---------------|:--------|:----------|
|<span data-ttu-id="8c6aa-153">funSettings</span><span class="sxs-lookup"><span data-stu-id="8c6aa-153">funSettings</span></span>|[<span data-ttu-id="8c6aa-154">teamFunSettings</span><span class="sxs-lookup"><span data-stu-id="8c6aa-154">teamFunSettings</span></span>](teamfunsettings.md) |<span data-ttu-id="8c6aa-155">Giphy、memes、およびチームのステッカーを構成する設定を使用します。</span><span class="sxs-lookup"><span data-stu-id="8c6aa-155">Settings to configure use of Giphy, memes, and stickers in the team.</span></span>|
|<span data-ttu-id="8c6aa-156">guestSettings</span><span class="sxs-lookup"><span data-stu-id="8c6aa-156">guestSettings</span></span>|[<span data-ttu-id="8c6aa-157">teamGuestSettings</span><span class="sxs-lookup"><span data-stu-id="8c6aa-157">teamGuestSettings</span></span>](teamguestsettings.md) |<span data-ttu-id="8c6aa-158">来園者が作成、更新、またはチーム内のチャンネルを削除するかどうかを構成するのに設定します。</span><span class="sxs-lookup"><span data-stu-id="8c6aa-158">Settings to configure whether guests can create, update, or delete channels in the team.</span></span>|
|<span data-ttu-id="8c6aa-159">isArchived</span><span class="sxs-lookup"><span data-stu-id="8c6aa-159">isArchived</span></span>|<span data-ttu-id="8c6aa-160">ブール型</span><span class="sxs-lookup"><span data-stu-id="8c6aa-160">Boolean</span></span>|<span data-ttu-id="8c6aa-161">このチームが、読み取り専用モードでかどうかです。</span><span class="sxs-lookup"><span data-stu-id="8c6aa-161">Whether this team is in read-only mode.</span></span> |
|<span data-ttu-id="8c6aa-162">memberSettings</span><span class="sxs-lookup"><span data-stu-id="8c6aa-162">memberSettings</span></span>|[<span data-ttu-id="8c6aa-163">teamMemberSettings</span><span class="sxs-lookup"><span data-stu-id="8c6aa-163">teamMemberSettings</span></span>](teammembersettings.md) |<span data-ttu-id="8c6aa-164">など、メンバーが特定のアクションを実行するかどうかを構成する設定は、チャネルを作成し、チームにボットを追加します。</span><span class="sxs-lookup"><span data-stu-id="8c6aa-164">Settings to configure whether members can perform certain actions, for example, create channels and add bots, in the team.</span></span>|
|<span data-ttu-id="8c6aa-165">messagingSettings</span><span class="sxs-lookup"><span data-stu-id="8c6aa-165">messagingSettings</span></span>|[<span data-ttu-id="8c6aa-166">teamMessagingSettings</span><span class="sxs-lookup"><span data-stu-id="8c6aa-166">teamMessagingSettings</span></span>](teammessagingsettings.md) |<span data-ttu-id="8c6aa-167">メッセージングを構成する設定は、チーム内の参照。</span><span class="sxs-lookup"><span data-stu-id="8c6aa-167">Settings to configure messaging and mentions in the team.</span></span>|
|<span data-ttu-id="8c6aa-168">webUrl</span><span class="sxs-lookup"><span data-stu-id="8c6aa-168">webUrl</span></span>|<span data-ttu-id="8c6aa-169">文字列 (読み取り専用)</span><span class="sxs-lookup"><span data-stu-id="8c6aa-169">string (readonly)</span></span> | <span data-ttu-id="8c6aa-170">クライアントの Microsoft のチームにチームに移動するハイパーリンク。</span><span class="sxs-lookup"><span data-stu-id="8c6aa-170">A hyperlink that will go to the team in the Microsoft Teams client.</span></span> <span data-ttu-id="8c6aa-171">これは、クライアントの Microsoft のチームにチームを右クリックし、**チームへのリンクを取得する**を選択するときに表示される URL です。</span><span class="sxs-lookup"><span data-stu-id="8c6aa-171">This is the URL that you get when you right-click a team in the Microsoft Teams client and select **Get link to team**.</span></span> <span data-ttu-id="8c6aa-172">この URL は、非透過 blob として扱われます、解析されない必要があります。</span><span class="sxs-lookup"><span data-stu-id="8c6aa-172">This URL should be treated as an opaque blob, and not parsed.</span></span> |

## <a name="relationships"></a><span data-ttu-id="8c6aa-173">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="8c6aa-173">Relationships</span></span>

| <span data-ttu-id="8c6aa-174">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="8c6aa-174">Relationship</span></span> | <span data-ttu-id="8c6aa-175">型</span><span class="sxs-lookup"><span data-stu-id="8c6aa-175">Type</span></span>   | <span data-ttu-id="8c6aa-176">説明</span><span class="sxs-lookup"><span data-stu-id="8c6aa-176">Description</span></span> |
|:---------------|:--------|:----------|
|<span data-ttu-id="8c6aa-177">チャンネル</span><span class="sxs-lookup"><span data-stu-id="8c6aa-177">channels</span></span>|<span data-ttu-id="8c6aa-178">[チャネル](channel.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="8c6aa-178">[channel](channel.md) collection</span></span>|<span data-ttu-id="8c6aa-179">チャンネルとチームに関連付けられているメッセージのコレクションです。</span><span class="sxs-lookup"><span data-stu-id="8c6aa-179">The collection of channels & messages associated with the team.</span></span>|
|<span data-ttu-id="8c6aa-180">installedApps</span><span class="sxs-lookup"><span data-stu-id="8c6aa-180">installedApps</span></span>|<span data-ttu-id="8c6aa-181">[teamsAppInstallation](teamsappinstallation.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="8c6aa-181">[teamsAppInstallation](teamsappinstallation.md) collection</span></span>|<span data-ttu-id="8c6aa-182">このチームにインストールされているアプリケーションです。</span><span class="sxs-lookup"><span data-stu-id="8c6aa-182">The apps installed in this team.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="8c6aa-183">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="8c6aa-183">JSON representation</span></span>

<span data-ttu-id="8c6aa-184">リソースの JSON 表記を次に示します。</span><span class="sxs-lookup"><span data-stu-id="8c6aa-184">The following is a JSON representation of the resource.</span></span>

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

## <a name="see-also"></a><span data-ttu-id="8c6aa-185">関連項目</span><span class="sxs-lookup"><span data-stu-id="8c6aa-185">See Also</span></span>
- [<span data-ttu-id="8c6aa-186">チームのグループを作成</span><span class="sxs-lookup"><span data-stu-id="8c6aa-186">Creating a group with a team</span></span>](/graph/teams-create-group-and-team)
- [<span data-ttu-id="8c6aa-187">チーム Api を使用します。</span><span class="sxs-lookup"><span data-stu-id="8c6aa-187">Using Teams APIs</span></span>](teams-api-overview.md)
