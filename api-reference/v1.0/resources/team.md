# <a name="team-resource-type"></a><span data-ttu-id="81107-101">チーム リソースの種類</span><span class="sxs-lookup"><span data-stu-id="81107-101">team resource type</span></span>



<span data-ttu-id="81107-102">マイクロソフトのチームで、チームは、[チャネル](channel.md)のコレクションです。</span><span class="sxs-lookup"><span data-stu-id="81107-102">A team in Microsoft Teams is a collection of [channels](channel.md).</span></span> <span data-ttu-id="81107-103">チャネルでは、トピックとチーム内での議論の論理的分離を表します。</span><span class="sxs-lookup"><span data-stu-id="81107-103">A channel represents a topic, and therefore a logical isolation of discussion, within a team.</span></span>

<span data-ttu-id="81107-104">すべてのチームは、[グループ](../resources/group.md)に関連付けられます。</span><span class="sxs-lookup"><span data-stu-id="81107-104">Every team is associated with a [group](../resources/group.md).</span></span>
<span data-ttu-id="81107-105">グループは、チーム ・/groups/{id} などと同じ ID を持っているし、チームは、/teams/{id} と同じです。</span><span class="sxs-lookup"><span data-stu-id="81107-105">The group has the same ID as the team - for example, /groups/{id}/team is the same as /teams/{id}.</span></span>
<span data-ttu-id="81107-106">グループとチームのメンバーの詳細については、[マイクロソフトのチームで作業するのには Microsoft グラフ REST API を使用](teams_api_overview.md)を参照してください。</span><span class="sxs-lookup"><span data-stu-id="81107-106">For more information about working with groups and members in teams, see [Use the Microsoft Graph REST API to work with Microsoft Teams](teams_api_overview.md).</span></span>

## <a name="methods"></a><span data-ttu-id="81107-107">メソッド</span><span class="sxs-lookup"><span data-stu-id="81107-107">Methods</span></span>

| <span data-ttu-id="81107-108">メソッド</span><span class="sxs-lookup"><span data-stu-id="81107-108">Method</span></span>       | <span data-ttu-id="81107-109">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="81107-109">Return Type</span></span>  |<span data-ttu-id="81107-110">説明</span><span class="sxs-lookup"><span data-stu-id="81107-110">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="81107-111">チームを作成します。</span><span class="sxs-lookup"><span data-stu-id="81107-111">Create team</span></span>](../api/team_put_teams.md) | [<span data-ttu-id="81107-112">チーム</span><span class="sxs-lookup"><span data-stu-id="81107-112">team</span></span>](team.md) | <span data-ttu-id="81107-113">新しいチームを作成または既存のグループにチームを追加します。</span><span class="sxs-lookup"><span data-stu-id="81107-113">Create a new team, or add a team to an existing group.</span></span>|
|[<span data-ttu-id="81107-114">チームを取得します。</span><span class="sxs-lookup"><span data-stu-id="81107-114">Get team</span></span>](../api/team_get.md) | [<span data-ttu-id="81107-115">チーム</span><span class="sxs-lookup"><span data-stu-id="81107-115">team</span></span>](team.md) | <span data-ttu-id="81107-116">プロパティと指定されたチームの関係を取得します。</span><span class="sxs-lookup"><span data-stu-id="81107-116">Retrieve the properties and relationships of the specified team.</span></span>|
|[<span data-ttu-id="81107-117">チームを更新します。</span><span class="sxs-lookup"><span data-stu-id="81107-117">Update team</span></span>](../api/team_update.md) | [<span data-ttu-id="81107-118">チーム</span><span class="sxs-lookup"><span data-stu-id="81107-118">team</span></span>](team.md) |<span data-ttu-id="81107-119">指定されたチームのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="81107-119">Update the properties of the specified team.</span></span> |
|[<span data-ttu-id="81107-120">チームを削除します。</span><span class="sxs-lookup"><span data-stu-id="81107-120">Delete team</span></span>](../../v1.0/api/group_delete.md) | <span data-ttu-id="81107-121">なし</span><span class="sxs-lookup"><span data-stu-id="81107-121">None</span></span> |<span data-ttu-id="81107-122">チームおよびその関連付けられているグループを削除します。</span><span class="sxs-lookup"><span data-stu-id="81107-122">Delete the team and its associated group.</span></span> |
|[<span data-ttu-id="81107-123">チームのクローンを作成します。</span><span class="sxs-lookup"><span data-stu-id="81107-123">Clone team</span></span>](../api/team_clone.md) | [<span data-ttu-id="81107-124">teamsAsyncOperation</span><span class="sxs-lookup"><span data-stu-id="81107-124">teamsAsyncOperation</span></span>](../resources/teamsasyncoperation.md) |<span data-ttu-id="81107-125">チームおよびその関連付けられているグループをコピーします。</span><span class="sxs-lookup"><span data-stu-id="81107-125">Copy the team and its associated group.</span></span> |
|[<span data-ttu-id="81107-126">チームのアーカイブ</span><span class="sxs-lookup"><span data-stu-id="81107-126">Archive team</span></span>](../api/team_archive.md) | [<span data-ttu-id="81107-127">teamsAsyncOperation</span><span class="sxs-lookup"><span data-stu-id="81107-127">teamsAsyncOperation</span></span>](../resources/teamsasyncoperation.md) |<span data-ttu-id="81107-128">読み取り専用状態で、チームを配置します。</span><span class="sxs-lookup"><span data-stu-id="81107-128">Put the team in a read-only state.</span></span> |
|[<span data-ttu-id="81107-129">チームを unarchive します。</span><span class="sxs-lookup"><span data-stu-id="81107-129">Unarchive team</span></span>](../api/team_unarchive.md) | [<span data-ttu-id="81107-130">teamsAsyncOperation</span><span class="sxs-lookup"><span data-stu-id="81107-130">teamsAsyncOperation</span></span>](../resources/teamsasyncoperation.md) |<span data-ttu-id="81107-131">チームを読み取り/書き込み状態に復元します。</span><span class="sxs-lookup"><span data-stu-id="81107-131">Restore the team to a read-write state.</span></span> |
|[<span data-ttu-id="81107-132">チームの一覧を表示します。</span><span class="sxs-lookup"><span data-stu-id="81107-132">List your teams</span></span>](../api/user_list_joinedteams.md) | <span data-ttu-id="81107-133">[チーム](team.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="81107-133">[team](team.md) collection</span></span> | <span data-ttu-id="81107-134">チームのメンバーを一覧表示します。</span><span class="sxs-lookup"><span data-stu-id="81107-134">List the teams you are a member of.</span></span> |
|[<span data-ttu-id="81107-135">すべてのチームをリストします。</span><span class="sxs-lookup"><span data-stu-id="81107-135">List all teams</span></span>](../../../concepts/teams_list_all_teams.md) | <span data-ttu-id="81107-136">[group](group.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="81107-136">[group](group.md) collection</span></span> | <span data-ttu-id="81107-137">チームのすべてのグループを一覧表示します。</span><span class="sxs-lookup"><span data-stu-id="81107-137">List all groups that have teams.</span></span> |
|[<span data-ttu-id="81107-138">組織にアプリケーションを発行します。</span><span class="sxs-lookup"><span data-stu-id="81107-138">Publish apps to your organization</span></span>](../resources/teamsapp.md)| [<span data-ttu-id="81107-139">teamsApp</span><span class="sxs-lookup"><span data-stu-id="81107-139">teamsApp</span></span>](../resources/teamsapp.md) | <span data-ttu-id="81107-140">組織にのみ表示されているチームのアプリケーションを作成します。</span><span class="sxs-lookup"><span data-stu-id="81107-140">Create Teams apps visible only to your organization.</span></span> |
|[<span data-ttu-id="81107-141">アプリケーションをチームに追加します。</span><span class="sxs-lookup"><span data-stu-id="81107-141">Add app to team</span></span>](../api/teamsappinstallation_add.md) | [<span data-ttu-id="81107-142">teamsappinstallation</span><span class="sxs-lookup"><span data-stu-id="81107-142">teamsappinstallation</span></span>](teamsappinstallation.md) | <span data-ttu-id="81107-143">(インストール) を追加するチームにアプリです。</span><span class="sxs-lookup"><span data-stu-id="81107-143">Adds (installs) an app to a team.</span></span>|
|[<span data-ttu-id="81107-144">チャネルにタブを追加します。</span><span class="sxs-lookup"><span data-stu-id="81107-144">Add tab to channel</span></span>](../api/teamstab_add.md) | [<span data-ttu-id="81107-145">teamsTab</span><span class="sxs-lookup"><span data-stu-id="81107-145">teamsTab</span></span>](../resources/teamstab.md) | <span data-ttu-id="81107-146">(インストール) を追加するチャネル ・ チームのタブです。</span><span class="sxs-lookup"><span data-stu-id="81107-146">Adds (installs) a tab to a team's channel.</span></span>|

## <a name="properties"></a><span data-ttu-id="81107-147">プロパティ</span><span class="sxs-lookup"><span data-stu-id="81107-147">Properties</span></span>

| <span data-ttu-id="81107-148">プロパティ</span><span class="sxs-lookup"><span data-stu-id="81107-148">Property</span></span> | <span data-ttu-id="81107-149">型</span><span class="sxs-lookup"><span data-stu-id="81107-149">Type</span></span>   | <span data-ttu-id="81107-150">説明</span><span class="sxs-lookup"><span data-stu-id="81107-150">Description</span></span> |
|:---------------|:--------|:----------|
|<span data-ttu-id="81107-151">funSettings</span><span class="sxs-lookup"><span data-stu-id="81107-151">funSettings</span></span>|[<span data-ttu-id="81107-152">teamFunSettings</span><span class="sxs-lookup"><span data-stu-id="81107-152">teamFunSettings</span></span>](teamfunsettings.md) |<span data-ttu-id="81107-153">Giphy、memes、およびチームのステッカーを構成する設定を使用します。</span><span class="sxs-lookup"><span data-stu-id="81107-153">Settings to configure use of Giphy, memes, and stickers in the team.</span></span>|
|<span data-ttu-id="81107-154">guestSettings</span><span class="sxs-lookup"><span data-stu-id="81107-154">guestSettings</span></span>|[<span data-ttu-id="81107-155">teamGuestSettings</span><span class="sxs-lookup"><span data-stu-id="81107-155">teamGuestSettings</span></span>](teamguestsettings.md) |<span data-ttu-id="81107-156">来園者が作成、更新、またはチーム内のチャンネルを削除するかどうかを構成するのに設定します。</span><span class="sxs-lookup"><span data-stu-id="81107-156">Settings to configure whether guests can create, update, or delete channels in the team.</span></span>|
|<span data-ttu-id="81107-157">isArchived</span><span class="sxs-lookup"><span data-stu-id="81107-157">isArchived</span></span>|<span data-ttu-id="81107-158">Boolean</span><span class="sxs-lookup"><span data-stu-id="81107-158">Boolean</span></span>|<span data-ttu-id="81107-159">このチームが、読み取り専用モードでかどうかです。</span><span class="sxs-lookup"><span data-stu-id="81107-159">Whether this team is in read-only mode.</span></span> |
|<span data-ttu-id="81107-160">memberSettings</span><span class="sxs-lookup"><span data-stu-id="81107-160">memberSettings</span></span>|[<span data-ttu-id="81107-161">teamMemberSettings</span><span class="sxs-lookup"><span data-stu-id="81107-161">teamMemberSettings</span></span>](teammembersettings.md) |<span data-ttu-id="81107-162">など、メンバーが特定のアクションを実行するかどうかを構成する設定は、チャネルを作成し、チームにボットを追加します。</span><span class="sxs-lookup"><span data-stu-id="81107-162">Settings to configure whether members can perform certain actions, for example, create channels and add bots, in the team.</span></span>|
|<span data-ttu-id="81107-163">messagingSettings</span><span class="sxs-lookup"><span data-stu-id="81107-163">messagingSettings</span></span>|[<span data-ttu-id="81107-164">teamMessagingSettings</span><span class="sxs-lookup"><span data-stu-id="81107-164">teamMessagingSettings</span></span>](teammessagingsettings.md) |<span data-ttu-id="81107-165">メッセージングを構成する設定は、チーム内の参照。</span><span class="sxs-lookup"><span data-stu-id="81107-165">Settings to configure messaging and mentions in the team.</span></span>|
|<span data-ttu-id="81107-166">webUrl</span><span class="sxs-lookup"><span data-stu-id="81107-166">webUrl</span></span>|<span data-ttu-id="81107-167">文字列 (読み取り専用)</span><span class="sxs-lookup"><span data-stu-id="81107-167">string (readonly)</span></span> | <span data-ttu-id="81107-168">クライアントの Microsoft のチームにチームに移動するハイパーリンク。</span><span class="sxs-lookup"><span data-stu-id="81107-168">A hyperlink that will go to the team in the Microsoft Teams client.</span></span> <span data-ttu-id="81107-169">これは、クライアントの Microsoft のチームにチームを右クリックし、**チームへのリンクを取得する**を選択するときに表示される URL です。</span><span class="sxs-lookup"><span data-stu-id="81107-169">This is the URL that you get when you right-click a team in the Microsoft Teams client and select **Get link to team**.</span></span> <span data-ttu-id="81107-170">この URL は、非透過 blob として扱われます、解析されない必要があります。</span><span class="sxs-lookup"><span data-stu-id="81107-170">This URL should be treated as an opaque blob, and not parsed.</span></span> |

## <a name="relationships"></a><span data-ttu-id="81107-171">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="81107-171">Relationships</span></span>

| <span data-ttu-id="81107-172">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="81107-172">Relationship</span></span> | <span data-ttu-id="81107-173">型</span><span class="sxs-lookup"><span data-stu-id="81107-173">Type</span></span>   | <span data-ttu-id="81107-174">説明</span><span class="sxs-lookup"><span data-stu-id="81107-174">Description</span></span> |
|:---------------|:--------|:----------|
|<span data-ttu-id="81107-175">チャンネル</span><span class="sxs-lookup"><span data-stu-id="81107-175">channels</span></span>|<span data-ttu-id="81107-176">[チャネル](channel.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="81107-176">[channel](channel.md) collection</span></span>|<span data-ttu-id="81107-177">チャンネルとチームに関連付けられているメッセージのコレクションです。</span><span class="sxs-lookup"><span data-stu-id="81107-177">The collection of channels & messages associated with the team.</span></span>|
|<span data-ttu-id="81107-178">installedApps</span><span class="sxs-lookup"><span data-stu-id="81107-178">installedApps</span></span>|<span data-ttu-id="81107-179">[teamsAppInstallation](teamsappinstallation.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="81107-179">[teamsAppInstallation](teamsappinstallation.md) collection</span></span>|<span data-ttu-id="81107-180">このチームにインストールされているアプリケーションです。</span><span class="sxs-lookup"><span data-stu-id="81107-180">The apps installed in this team.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="81107-181">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="81107-181">JSON representation</span></span>

<span data-ttu-id="81107-182">リソースの JSON 表記を次に示します。</span><span class="sxs-lookup"><span data-stu-id="81107-182">The following is a JSON representation of the resource.</span></span>

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

## <a name="see-also"></a><span data-ttu-id="81107-183">関連項目</span><span class="sxs-lookup"><span data-stu-id="81107-183">See Also</span></span>
- [<span data-ttu-id="81107-184">チームのグループを作成</span><span class="sxs-lookup"><span data-stu-id="81107-184">Creating a group with a team</span></span>](../../../concepts/teams-create-group-and-team.md)
- [<span data-ttu-id="81107-185">チーム Api を使用します。</span><span class="sxs-lookup"><span data-stu-id="81107-185">Using Teams APIs</span></span>](teams_api_overview.md)
