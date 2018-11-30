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
# <a name="team-resource-type"></a><span data-ttu-id="8eef3-103">チーム リソースの種類</span><span class="sxs-lookup"><span data-stu-id="8eef3-103">team resource type</span></span>

> <span data-ttu-id="8eef3-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="8eef3-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="8eef3-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="8eef3-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="8eef3-106">マイクロソフトのチームで、チームは、[チャネル](channel.md)のコレクションです。</span><span class="sxs-lookup"><span data-stu-id="8eef3-106">A team in Microsoft Teams is a collection of [channels](channel.md).</span></span> <span data-ttu-id="8eef3-107">チャネルでは、トピックとチーム内での議論の論理的分離を表します。</span><span class="sxs-lookup"><span data-stu-id="8eef3-107">A channel represents a topic, and therefore a logical isolation of discussion, within a team.</span></span>

<span data-ttu-id="8eef3-108">すべてのチームは、[グループ](../resources/group.md)に関連付けられます。</span><span class="sxs-lookup"><span data-stu-id="8eef3-108">Every team is associated with a [group](../resources/group.md).</span></span>
<span data-ttu-id="8eef3-109">グループは、チーム ・/groups/{id} などと同じ ID を持っているし、チームは、/teams/{id} と同じです。</span><span class="sxs-lookup"><span data-stu-id="8eef3-109">The group has the same ID as the team - for example, /groups/{id}/team is the same as /teams/{id}.</span></span>
<span data-ttu-id="8eef3-110">グループとチームのメンバーの詳細については、[マイクロソフトのチームで作業するのには Microsoft グラフ REST API を使用](teams-api-overview.md)を参照してください。</span><span class="sxs-lookup"><span data-stu-id="8eef3-110">For more information about working with groups and members in teams, see [Use the Microsoft Graph REST API to work with Microsoft Teams](teams-api-overview.md).</span></span>

## <a name="methods"></a><span data-ttu-id="8eef3-111">メソッド</span><span class="sxs-lookup"><span data-stu-id="8eef3-111">Methods</span></span>

| <span data-ttu-id="8eef3-112">メソッド</span><span class="sxs-lookup"><span data-stu-id="8eef3-112">Method</span></span>       | <span data-ttu-id="8eef3-113">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="8eef3-113">Return Type</span></span>  |<span data-ttu-id="8eef3-114">説明</span><span class="sxs-lookup"><span data-stu-id="8eef3-114">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="8eef3-115">チームを作成します。</span><span class="sxs-lookup"><span data-stu-id="8eef3-115">Create team</span></span>](../api/team-put-teams.md) | [<span data-ttu-id="8eef3-116">チーム</span><span class="sxs-lookup"><span data-stu-id="8eef3-116">team</span></span>](team.md) | <span data-ttu-id="8eef3-117">新しいチームを作成または既存のグループにチームを追加します。</span><span class="sxs-lookup"><span data-stu-id="8eef3-117">Create a new team, or add a team to an existing group.</span></span>|
|[<span data-ttu-id="8eef3-118">チームを取得します。</span><span class="sxs-lookup"><span data-stu-id="8eef3-118">Get team</span></span>](../api/team-get.md) | [<span data-ttu-id="8eef3-119">チーム</span><span class="sxs-lookup"><span data-stu-id="8eef3-119">team</span></span>](team.md) | <span data-ttu-id="8eef3-120">プロパティと指定されたチームの関係を取得します。</span><span class="sxs-lookup"><span data-stu-id="8eef3-120">Retrieve the properties and relationships of the specified team.</span></span>|
|[<span data-ttu-id="8eef3-121">チームを更新します。</span><span class="sxs-lookup"><span data-stu-id="8eef3-121">Update team</span></span>](../api/team-update.md) | [<span data-ttu-id="8eef3-122">チーム</span><span class="sxs-lookup"><span data-stu-id="8eef3-122">team</span></span>](team.md) |<span data-ttu-id="8eef3-123">指定されたチームのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="8eef3-123">Update the properties of the specified team.</span></span> |
|[<span data-ttu-id="8eef3-124">チームを削除します。</span><span class="sxs-lookup"><span data-stu-id="8eef3-124">Delete team</span></span>](/graph/api/group-delete?view=graph-rest-1.0) | <span data-ttu-id="8eef3-125">なし</span><span class="sxs-lookup"><span data-stu-id="8eef3-125">None</span></span> |<span data-ttu-id="8eef3-126">チームおよびその関連付けられているグループを削除します。</span><span class="sxs-lookup"><span data-stu-id="8eef3-126">Delete the team and its associated group.</span></span> |
|[<span data-ttu-id="8eef3-127">チームのクローンを作成します。</span><span class="sxs-lookup"><span data-stu-id="8eef3-127">Clone team</span></span>](../api/team-clone.md) | [<span data-ttu-id="8eef3-128">teamsAsyncOperation</span><span class="sxs-lookup"><span data-stu-id="8eef3-128">teamsAsyncOperation</span></span>](../resources/teamsasyncoperation.md) |<span data-ttu-id="8eef3-129">チームおよびその関連付けられているグループをコピーします。</span><span class="sxs-lookup"><span data-stu-id="8eef3-129">Copy the team and its associated group.</span></span> |
|[<span data-ttu-id="8eef3-130">チームのアーカイブ</span><span class="sxs-lookup"><span data-stu-id="8eef3-130">Archive team</span></span>](../api/team-archive.md) | [<span data-ttu-id="8eef3-131">teamsAsyncOperation</span><span class="sxs-lookup"><span data-stu-id="8eef3-131">teamsAsyncOperation</span></span>](../resources/teamsasyncoperation.md) |<span data-ttu-id="8eef3-132">読み取り専用状態で、チームを配置します。</span><span class="sxs-lookup"><span data-stu-id="8eef3-132">Put the team in a read-only state.</span></span> |
|[<span data-ttu-id="8eef3-133">チームを unarchive します。</span><span class="sxs-lookup"><span data-stu-id="8eef3-133">Unarchive team</span></span>](../api/team-unarchive.md) | [<span data-ttu-id="8eef3-134">teamsAsyncOperation</span><span class="sxs-lookup"><span data-stu-id="8eef3-134">teamsAsyncOperation</span></span>](../resources/teamsasyncoperation.md) |<span data-ttu-id="8eef3-135">チームを読み取り/書き込み状態に復元します。</span><span class="sxs-lookup"><span data-stu-id="8eef3-135">Restore the team to a read-write state.</span></span> |
|[<span data-ttu-id="8eef3-136">チームの一覧を表示します。</span><span class="sxs-lookup"><span data-stu-id="8eef3-136">List your teams</span></span>](../api/user-list-joinedteams.md) | <span data-ttu-id="8eef3-137">[チーム](team.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="8eef3-137">[team](team.md) collection</span></span> | <span data-ttu-id="8eef3-138">チームのメンバーを一覧表示します。</span><span class="sxs-lookup"><span data-stu-id="8eef3-138">List the teams you are a member of.</span></span> |
|[<span data-ttu-id="8eef3-139">すべてのチームをリストします。</span><span class="sxs-lookup"><span data-stu-id="8eef3-139">List all teams</span></span>](/graph/teams-list-all-teams) | <span data-ttu-id="8eef3-140">[group](group.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="8eef3-140">[group](group.md) collection</span></span> | <span data-ttu-id="8eef3-141">チームのすべてのグループを一覧表示します。</span><span class="sxs-lookup"><span data-stu-id="8eef3-141">List all groups that have teams.</span></span> |
|[<span data-ttu-id="8eef3-142">組織にアプリケーションを発行します。</span><span class="sxs-lookup"><span data-stu-id="8eef3-142">Publish apps to your organization</span></span>](../resources/teamsapp.md)| [<span data-ttu-id="8eef3-143">teamsApp</span><span class="sxs-lookup"><span data-stu-id="8eef3-143">teamsApp</span></span>](../resources/teamsapp.md) | <span data-ttu-id="8eef3-144">組織にのみ表示されているチームのアプリケーションを作成します。</span><span class="sxs-lookup"><span data-stu-id="8eef3-144">Create Teams apps visible only to your organization.</span></span> |
|[<span data-ttu-id="8eef3-145">アプリケーションをチームに追加します。</span><span class="sxs-lookup"><span data-stu-id="8eef3-145">Add app to team</span></span>](../api/teamsappinstallation-add.md) | [<span data-ttu-id="8eef3-146">teamsappinstallation</span><span class="sxs-lookup"><span data-stu-id="8eef3-146">teamsappinstallation</span></span>](teamsappinstallation.md) | <span data-ttu-id="8eef3-147">(インストール) を追加するチームにアプリです。</span><span class="sxs-lookup"><span data-stu-id="8eef3-147">Adds (installs) an app to a team.</span></span>|
|[<span data-ttu-id="8eef3-148">チャネルにタブを追加します。</span><span class="sxs-lookup"><span data-stu-id="8eef3-148">Add tab to channel</span></span>](../api/teamstab-add.md) | [<span data-ttu-id="8eef3-149">teamsTab</span><span class="sxs-lookup"><span data-stu-id="8eef3-149">teamsTab</span></span>](../resources/teamstab.md) | <span data-ttu-id="8eef3-150">(インストール) を追加するチャネル ・ チームのタブです。</span><span class="sxs-lookup"><span data-stu-id="8eef3-150">Adds (installs) a tab to a team's channel.</span></span>|
|[<span data-ttu-id="8eef3-151">リストからチャネルのメッセージ</span><span class="sxs-lookup"><span data-stu-id="8eef3-151">List channel messages</span></span>](../api/channel-list-messages.md)  | [<span data-ttu-id="8eef3-152">chatMessage</span><span class="sxs-lookup"><span data-stu-id="8eef3-152">chatMessage</span></span>](../resources/chatmessage.md) | [<span data-ttu-id="8eef3-153">チャネルでメッセージを取得します。</span><span class="sxs-lookup"><span data-stu-id="8eef3-153">Get messages in a channel</span></span>](../api/channel-list-messages.md) |

## <a name="properties"></a><span data-ttu-id="8eef3-154">プロパティ</span><span class="sxs-lookup"><span data-stu-id="8eef3-154">Properties</span></span>

| <span data-ttu-id="8eef3-155">プロパティ</span><span class="sxs-lookup"><span data-stu-id="8eef3-155">Property</span></span> | <span data-ttu-id="8eef3-156">型</span><span class="sxs-lookup"><span data-stu-id="8eef3-156">Type</span></span>   | <span data-ttu-id="8eef3-157">説明</span><span class="sxs-lookup"><span data-stu-id="8eef3-157">Description</span></span> |
|:---------------|:--------|:----------|
|<span data-ttu-id="8eef3-158">funSettings</span><span class="sxs-lookup"><span data-stu-id="8eef3-158">funSettings</span></span>|[<span data-ttu-id="8eef3-159">teamFunSettings</span><span class="sxs-lookup"><span data-stu-id="8eef3-159">teamFunSettings</span></span>](teamfunsettings.md) |<span data-ttu-id="8eef3-160">Giphy、memes、およびチームのステッカーを構成する設定を使用します。</span><span class="sxs-lookup"><span data-stu-id="8eef3-160">Settings to configure use of Giphy, memes, and stickers in the team.</span></span>|
|<span data-ttu-id="8eef3-161">guestSettings</span><span class="sxs-lookup"><span data-stu-id="8eef3-161">guestSettings</span></span>|[<span data-ttu-id="8eef3-162">teamGuestSettings</span><span class="sxs-lookup"><span data-stu-id="8eef3-162">teamGuestSettings</span></span>](teamguestsettings.md) |<span data-ttu-id="8eef3-163">来園者が作成、更新、またはチーム内のチャンネルを削除するかどうかを構成するのに設定します。</span><span class="sxs-lookup"><span data-stu-id="8eef3-163">Settings to configure whether guests can create, update, or delete channels in the team.</span></span>|
|<span data-ttu-id="8eef3-164">isArchived</span><span class="sxs-lookup"><span data-stu-id="8eef3-164">isArchived</span></span>|<span data-ttu-id="8eef3-165">ブール値</span><span class="sxs-lookup"><span data-stu-id="8eef3-165">Boolean</span></span>|<span data-ttu-id="8eef3-166">このチームが、読み取り専用モードでかどうかです。</span><span class="sxs-lookup"><span data-stu-id="8eef3-166">Whether this team is in read-only mode.</span></span> |
|<span data-ttu-id="8eef3-167">memberSettings</span><span class="sxs-lookup"><span data-stu-id="8eef3-167">memberSettings</span></span>|[<span data-ttu-id="8eef3-168">teamMemberSettings</span><span class="sxs-lookup"><span data-stu-id="8eef3-168">teamMemberSettings</span></span>](teammembersettings.md) |<span data-ttu-id="8eef3-169">など、メンバーが特定のアクションを実行するかどうかを構成する設定は、チャネルを作成し、チームにボットを追加します。</span><span class="sxs-lookup"><span data-stu-id="8eef3-169">Settings to configure whether members can perform certain actions, for example, create channels and add bots, in the team.</span></span>|
|<span data-ttu-id="8eef3-170">messagingSettings</span><span class="sxs-lookup"><span data-stu-id="8eef3-170">messagingSettings</span></span>|[<span data-ttu-id="8eef3-171">teamMessagingSettings</span><span class="sxs-lookup"><span data-stu-id="8eef3-171">teamMessagingSettings</span></span>](teammessagingsettings.md) |<span data-ttu-id="8eef3-172">メッセージングを構成する設定は、チーム内の参照。</span><span class="sxs-lookup"><span data-stu-id="8eef3-172">Settings to configure messaging and mentions in the team.</span></span>|
|<span data-ttu-id="8eef3-173">webUrl</span><span class="sxs-lookup"><span data-stu-id="8eef3-173">webUrl</span></span>|<span data-ttu-id="8eef3-174">文字列 (読み取り専用)</span><span class="sxs-lookup"><span data-stu-id="8eef3-174">string (readonly)</span></span> | <span data-ttu-id="8eef3-175">クライアントの Microsoft のチームにチームに移動するハイパーリンク。</span><span class="sxs-lookup"><span data-stu-id="8eef3-175">A hyperlink that will go to the team in the Microsoft Teams client.</span></span> <span data-ttu-id="8eef3-176">これは、クライアントの Microsoft のチームにチームを右クリックし、**チームへのリンクを取得する**を選択するときに表示される URL です。</span><span class="sxs-lookup"><span data-stu-id="8eef3-176">This is the URL that you get when you right-click a team in the Microsoft Teams client and select **Get link to team**.</span></span> <span data-ttu-id="8eef3-177">この URL は、非透過 blob として扱われます、解析されない必要があります。</span><span class="sxs-lookup"><span data-stu-id="8eef3-177">This URL should be treated as an opaque blob, and not parsed.</span></span> |

## <a name="relationships"></a><span data-ttu-id="8eef3-178">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="8eef3-178">Relationships</span></span>

| <span data-ttu-id="8eef3-179">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="8eef3-179">Relationship</span></span> | <span data-ttu-id="8eef3-180">型</span><span class="sxs-lookup"><span data-stu-id="8eef3-180">Type</span></span>   | <span data-ttu-id="8eef3-181">説明</span><span class="sxs-lookup"><span data-stu-id="8eef3-181">Description</span></span> |
|:---------------|:--------|:----------|
|<span data-ttu-id="8eef3-182">apps</span><span class="sxs-lookup"><span data-stu-id="8eef3-182">apps</span></span>|<span data-ttu-id="8eef3-183">[teamsApp](teamsapp.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="8eef3-183">[teamsApp](teamsapp.md) collection</span></span>| <span data-ttu-id="8eef3-184">(古い形式)このチームにインストールされているアプリケーションです。</span><span class="sxs-lookup"><span data-stu-id="8eef3-184">(Obsolete) The apps installed in this team.</span></span>|
|<span data-ttu-id="8eef3-185">チャンネル</span><span class="sxs-lookup"><span data-stu-id="8eef3-185">channels</span></span>|<span data-ttu-id="8eef3-186">[チャネル](channel.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="8eef3-186">[channel](channel.md) collection</span></span>|<span data-ttu-id="8eef3-187">チャンネルとチームに関連付けられているメッセージのコレクションです。</span><span class="sxs-lookup"><span data-stu-id="8eef3-187">The collection of channels & messages associated with the team.</span></span>|
|<span data-ttu-id="8eef3-188">installedApps</span><span class="sxs-lookup"><span data-stu-id="8eef3-188">installedApps</span></span>|<span data-ttu-id="8eef3-189">[teamsAppInstallation](teamsappinstallation.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="8eef3-189">[teamsAppInstallation](teamsappinstallation.md) collection</span></span>|<span data-ttu-id="8eef3-190">このチームにインストールされているアプリケーションです。</span><span class="sxs-lookup"><span data-stu-id="8eef3-190">The apps installed in this team.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="8eef3-191">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="8eef3-191">JSON representation</span></span>

<span data-ttu-id="8eef3-192">リソースの JSON 表記を次に示します。</span><span class="sxs-lookup"><span data-stu-id="8eef3-192">The following is a JSON representation of the resource.</span></span>

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

## <a name="see-also"></a><span data-ttu-id="8eef3-193">関連項目</span><span class="sxs-lookup"><span data-stu-id="8eef3-193">See Also</span></span>
- [<span data-ttu-id="8eef3-194">チームのグループを作成</span><span class="sxs-lookup"><span data-stu-id="8eef3-194">Creating a group with a team</span></span>](/graph/teams-create-group-and-team)
- [<span data-ttu-id="8eef3-195">チーム API の概要</span><span class="sxs-lookup"><span data-stu-id="8eef3-195">Teams API Overview</span></span>](teams-api-overview.md)
