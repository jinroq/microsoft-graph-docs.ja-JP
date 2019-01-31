---
title: team リソースの種類
description: 'Microsoft Teams のチームは、チャネルのコレクションです。 '
author: nkramer
localization_priority: Priority
ms.prod: microsoft-teams
ms.openlocfilehash: 0e8f5a7644e56d1f6f2be08385fc1e9a280828ac
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/24/2019
ms.locfileid: "29526208"
---
# <a name="team-resource-type"></a><span data-ttu-id="017a9-103">team リソースの種類</span><span class="sxs-lookup"><span data-stu-id="017a9-103">team resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="017a9-104">Microsoft Teams のチームは、[チャネル](channel.md) のコレクションです。</span><span class="sxs-lookup"><span data-stu-id="017a9-104">A team in Microsoft Teams is a collection of [channels](channel.md).</span></span> <span data-ttu-id="017a9-105">チャネルは 1 つのトピック、つまりチーム内でのディスカッションの論理的分離を表します。</span><span class="sxs-lookup"><span data-stu-id="017a9-105">A channel represents a topic, and therefore a logical isolation of discussion, within a team.</span></span>

<span data-ttu-id="017a9-106">各チームには[グループ](../resources/group.md)が関連付けられています。</span><span class="sxs-lookup"><span data-stu-id="017a9-106">Every team is associated with a [group](../resources/group.md).</span></span>
<span data-ttu-id="017a9-107">グループの ID はチームと同じです。たとえば、/groups/{id}/team は /teams/{id} と同じです。</span><span class="sxs-lookup"><span data-stu-id="017a9-107">The group has the same ID as the team - for example, /groups/{id}/team is the same as /teams/{id}.</span></span>
<span data-ttu-id="017a9-108">チームのメンバーおよびグループの操作の詳細については、「[Microsoft Graph REST API を使用して Microsoft Teams を操作する](teams-api-overview.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="017a9-108">For more information about working with groups and members in teams, see [Use the Microsoft Graph REST API to work with Microsoft Teams](teams-api-overview.md).</span></span>

## <a name="methods"></a><span data-ttu-id="017a9-109">メソッド</span><span class="sxs-lookup"><span data-stu-id="017a9-109">Methods</span></span>

| <span data-ttu-id="017a9-110">メソッド</span><span class="sxs-lookup"><span data-stu-id="017a9-110">Method</span></span>       | <span data-ttu-id="017a9-111">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="017a9-111">Return Type</span></span>  |<span data-ttu-id="017a9-112">説明</span><span class="sxs-lookup"><span data-stu-id="017a9-112">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="017a9-113">チームを作成する</span><span class="sxs-lookup"><span data-stu-id="017a9-113">Create team</span></span>](../api/team-post.md) | [<span data-ttu-id="017a9-114">teamsAsyncOperation</span><span class="sxs-lookup"><span data-stu-id="017a9-114">teamsAsyncOperation</span></span>](teamsasyncoperation.md) | <span data-ttu-id="017a9-115">チームを新規に作成します。</span><span class="sxs-lookup"><span data-stu-id="017a9-115">Create a team from scratch.</span></span> |
|[<span data-ttu-id="017a9-116">グループからチームを作成する</span><span class="sxs-lookup"><span data-stu-id="017a9-116">Create team from group</span></span>](../api/team-put-teams.md) | [<span data-ttu-id="017a9-117">team</span><span class="sxs-lookup"><span data-stu-id="017a9-117">team</span></span>](team.md) | <span data-ttu-id="017a9-118">新しいチームを作成するか、既存のグループにチームを追加します。</span><span class="sxs-lookup"><span data-stu-id="017a9-118">Create a new team, or add a team to an existing group.</span></span>|
|[<span data-ttu-id="017a9-119">チームを取得する</span><span class="sxs-lookup"><span data-stu-id="017a9-119">Get team</span></span>](../api/team-get.md) | [<span data-ttu-id="017a9-120">team</span><span class="sxs-lookup"><span data-stu-id="017a9-120">team</span></span>](team.md) | <span data-ttu-id="017a9-121">指定したチームのプロパティとリレーションシップを取得します。</span><span class="sxs-lookup"><span data-stu-id="017a9-121">Retrieve the properties and relationships of the specified team.</span></span>|
|[<span data-ttu-id="017a9-122">チームを更新する</span><span class="sxs-lookup"><span data-stu-id="017a9-122">Update team</span></span>](../api/team-update.md) | [<span data-ttu-id="017a9-123">team</span><span class="sxs-lookup"><span data-stu-id="017a9-123">team</span></span>](team.md) |<span data-ttu-id="017a9-124">指定されたチームのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="017a9-124">Update the properties of the specified team.</span></span> |
|[<span data-ttu-id="017a9-125">チームを削除する</span><span class="sxs-lookup"><span data-stu-id="017a9-125">Delete team</span></span>](/graph/api/group-delete?view=graph-rest-1.0) | <span data-ttu-id="017a9-126">なし</span><span class="sxs-lookup"><span data-stu-id="017a9-126">None</span></span> |<span data-ttu-id="017a9-127">チームとその関連グループを削除します。</span><span class="sxs-lookup"><span data-stu-id="017a9-127">Delete the team and its associated group.</span></span> |
|[<span data-ttu-id="017a9-128">チームを複製する</span><span class="sxs-lookup"><span data-stu-id="017a9-128">Clone team</span></span>](../api/team-clone.md) | [<span data-ttu-id="017a9-129">teamsAsyncOperation</span><span class="sxs-lookup"><span data-stu-id="017a9-129">teamsAsyncOperation</span></span>](../resources/teamsasyncoperation.md) |<span data-ttu-id="017a9-130">チームとその関連グループをコピーします。</span><span class="sxs-lookup"><span data-stu-id="017a9-130">Copy the team and its associated group.</span></span> |
|[<span data-ttu-id="017a9-131">チームをアーカイブする</span><span class="sxs-lookup"><span data-stu-id="017a9-131">Archive team</span></span>](../api/team-archive.md) | [<span data-ttu-id="017a9-132">teamsAsyncOperation</span><span class="sxs-lookup"><span data-stu-id="017a9-132">teamsAsyncOperation</span></span>](../resources/teamsasyncoperation.md) |<span data-ttu-id="017a9-133">チームを読み取り専用状態にします。</span><span class="sxs-lookup"><span data-stu-id="017a9-133">Put the team in a read-only state.</span></span> |
|[<span data-ttu-id="017a9-134">チームを展開する</span><span class="sxs-lookup"><span data-stu-id="017a9-134">Unarchive team</span></span>](../api/team-unarchive.md) | [<span data-ttu-id="017a9-135">teamsAsyncOperation</span><span class="sxs-lookup"><span data-stu-id="017a9-135">teamsAsyncOperation</span></span>](../resources/teamsasyncoperation.md) |<span data-ttu-id="017a9-136">チームを読み取り/書き込み状態に復元します。</span><span class="sxs-lookup"><span data-stu-id="017a9-136">Restore the team to a read-write state.</span></span> |
|[<span data-ttu-id="017a9-137">チームを一覧表示する</span><span class="sxs-lookup"><span data-stu-id="017a9-137">List your teams</span></span>](../api/user-list-joinedteams.md) | <span data-ttu-id="017a9-138">[team](team.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="017a9-138">[team](team.md) collection</span></span> | <span data-ttu-id="017a9-139">メンバーであるチームの一覧を表示します。</span><span class="sxs-lookup"><span data-stu-id="017a9-139">List the teams you are a member of.</span></span> |
|[<span data-ttu-id="017a9-140">すべてのチームのリストを作成する</span><span class="sxs-lookup"><span data-stu-id="017a9-140">List all teams</span></span>](/graph/teams-list-all-teams) | <span data-ttu-id="017a9-141">[group](group.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="017a9-141">[group](group.md) collection</span></span> | <span data-ttu-id="017a9-142">チームを持つすべてのグループを一覧表示します。</span><span class="sxs-lookup"><span data-stu-id="017a9-142">List all groups that have teams.</span></span> |
|[<span data-ttu-id="017a9-143">組織に対してアプリを公開する</span><span class="sxs-lookup"><span data-stu-id="017a9-143">Publish apps to your organization</span></span>](../resources/teamsapp.md)| [<span data-ttu-id="017a9-144">teamsApp</span><span class="sxs-lookup"><span data-stu-id="017a9-144">teamsApp</span></span>](../resources/teamsapp.md) | <span data-ttu-id="017a9-145">所属組織のみに表示する Teams アプリを作成します。</span><span class="sxs-lookup"><span data-stu-id="017a9-145">Create Teams apps visible only to your organization.</span></span> |
|[<span data-ttu-id="017a9-146">アプリをチームに追加する</span><span class="sxs-lookup"><span data-stu-id="017a9-146">Add app to team</span></span>](../api/teamsappinstallation-add.md) | [<span data-ttu-id="017a9-147">teamsappinstallation</span><span class="sxs-lookup"><span data-stu-id="017a9-147">teamsappinstallation</span></span>](teamsappinstallation.md) | <span data-ttu-id="017a9-148">アプリをチームに追加 (インストール) します。</span><span class="sxs-lookup"><span data-stu-id="017a9-148">Adds (installs) an app to a team.</span></span>|
|[<span data-ttu-id="017a9-149">チャネルにタブを追加する</span><span class="sxs-lookup"><span data-stu-id="017a9-149">Add tab to channel</span></span>](../api/teamstab-add.md) | [<span data-ttu-id="017a9-150">teamsTab</span><span class="sxs-lookup"><span data-stu-id="017a9-150">teamsTab</span></span>](../resources/teamstab.md) | <span data-ttu-id="017a9-151">タブをチームのチャネルに追加 (インストール) します。</span><span class="sxs-lookup"><span data-stu-id="017a9-151">Adds (installs) a tab to a team's channel.</span></span>|
|[<span data-ttu-id="017a9-152">チャネル メッセージを一覧表示する</span><span class="sxs-lookup"><span data-stu-id="017a9-152">List channel messages</span></span>](../api/channel-list-messages.md)  | [<span data-ttu-id="017a9-153">chatMessage</span><span class="sxs-lookup"><span data-stu-id="017a9-153">chatMessage</span></span>](../resources/chatmessage.md) | [<span data-ttu-id="017a9-154">チャネルのメッセージを取得する</span><span class="sxs-lookup"><span data-stu-id="017a9-154">Get messages in a channel</span></span>](../api/channel-list-messages.md) |

## <a name="properties"></a><span data-ttu-id="017a9-155">プロパティ</span><span class="sxs-lookup"><span data-stu-id="017a9-155">Properties</span></span>

| <span data-ttu-id="017a9-156">プロパティ</span><span class="sxs-lookup"><span data-stu-id="017a9-156">Property</span></span> | <span data-ttu-id="017a9-157">型</span><span class="sxs-lookup"><span data-stu-id="017a9-157">Type</span></span>   | <span data-ttu-id="017a9-158">説明</span><span class="sxs-lookup"><span data-stu-id="017a9-158">Description</span></span> |
|:---------------|:--------|:----------|
|<span data-ttu-id="017a9-159">displayName</span><span class="sxs-lookup"><span data-stu-id="017a9-159">displayName</span></span>|<span data-ttu-id="017a9-160">string</span><span class="sxs-lookup"><span data-stu-id="017a9-160">string</span></span>| <span data-ttu-id="017a9-161">チームの名前。</span><span class="sxs-lookup"><span data-stu-id="017a9-161">The name of the team.</span></span> |
|<span data-ttu-id="017a9-162">説明</span><span class="sxs-lookup"><span data-stu-id="017a9-162">description</span></span>|<span data-ttu-id="017a9-163">string</span><span class="sxs-lookup"><span data-stu-id="017a9-163">string</span></span>| <span data-ttu-id="017a9-164">チームに関するオプションの説明。</span><span class="sxs-lookup"><span data-stu-id="017a9-164">An optional description for the team.</span></span> |
|<span data-ttu-id="017a9-165">classification</span><span class="sxs-lookup"><span data-stu-id="017a9-165">classification</span></span>|<span data-ttu-id="017a9-166">string</span><span class="sxs-lookup"><span data-stu-id="017a9-166">string</span></span>| <span data-ttu-id="017a9-167">省略可能なラベル。</span><span class="sxs-lookup"><span data-stu-id="017a9-167">An optional label.</span></span> <span data-ttu-id="017a9-168">通常、チームのデータまたはビジネスの機密度を記述します。</span><span class="sxs-lookup"><span data-stu-id="017a9-168">Typically describes the data or business sensitivity of the team.</span></span> <span data-ttu-id="017a9-169">テナントのディレクトリで事前に構成されているセットのいずれかに一致する必要があります。</span><span class="sxs-lookup"><span data-stu-id="017a9-169">Must match one of a pre-configured set in the tenant's directory.</span></span> |
|<span data-ttu-id="017a9-170">specialization</span><span class="sxs-lookup"><span data-stu-id="017a9-170">specialization</span></span>|[<span data-ttu-id="017a9-171">teamSpecialization</span><span class="sxs-lookup"><span data-stu-id="017a9-171">teamSpecialization</span></span>](teamspecialization.md)| <span data-ttu-id="017a9-172">省略可能。</span><span class="sxs-lookup"><span data-stu-id="017a9-172">Optional.</span></span> <span data-ttu-id="017a9-173">チームが特定のユース ケースを目的としているかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="017a9-173">Indicates whether the team is intended for a particular use case.</span></span>  <span data-ttu-id="017a9-174">チーム専門分野ごとに、ユース ケースをターゲットとする一意の動作とエクスペリエンスにアクセスできます。</span><span class="sxs-lookup"><span data-stu-id="017a9-174">Each team specialization has access to unique behaviors and experiences targeted to its use case.</span></span> |
|<span data-ttu-id="017a9-175">visibility</span><span class="sxs-lookup"><span data-stu-id="017a9-175">visibility</span></span>|[<span data-ttu-id="017a9-176">teamVisibilityType</span><span class="sxs-lookup"><span data-stu-id="017a9-176">teamVisibilityType</span></span>](teamvisibilitytype.md)| <span data-ttu-id="017a9-177">グループとチームの可視性。</span><span class="sxs-lookup"><span data-stu-id="017a9-177">The visibility of a the group and team.</span></span> <span data-ttu-id="017a9-178">既定では Public です。</span><span class="sxs-lookup"><span data-stu-id="017a9-178">Defaults to Public.</span></span> |
|<span data-ttu-id="017a9-179">funSettings</span><span class="sxs-lookup"><span data-stu-id="017a9-179">funSettings</span></span>|[<span data-ttu-id="017a9-180">teamFunSettings</span><span class="sxs-lookup"><span data-stu-id="017a9-180">teamFunSettings</span></span>](teamfunsettings.md) |<span data-ttu-id="017a9-181">チームでの Giphy、ミーム、およびステッカーの使用を構成する設定。</span><span class="sxs-lookup"><span data-stu-id="017a9-181">Settings to configure use of Giphy, memes, and stickers in the team.</span></span>|
|<span data-ttu-id="017a9-182">guestSettings</span><span class="sxs-lookup"><span data-stu-id="017a9-182">guestSettings</span></span>|[<span data-ttu-id="017a9-183">teamGuestSettings</span><span class="sxs-lookup"><span data-stu-id="017a9-183">teamGuestSettings</span></span>](teamguestsettings.md) |<span data-ttu-id="017a9-184">ゲストがチームでチャネルを作成、更新、または削除できるかどうかを構成する設定。</span><span class="sxs-lookup"><span data-stu-id="017a9-184">Settings to configure whether guests can create, update, or delete channels in the team.</span></span>|
|<span data-ttu-id="017a9-185">isArchived</span><span class="sxs-lookup"><span data-stu-id="017a9-185">isArchived</span></span>|<span data-ttu-id="017a9-186">Boolean</span><span class="sxs-lookup"><span data-stu-id="017a9-186">Boolean</span></span>|<span data-ttu-id="017a9-187">このチームが読み取り専用モードかどうか。</span><span class="sxs-lookup"><span data-stu-id="017a9-187">Whether this team is in read-only mode.</span></span> |
|<span data-ttu-id="017a9-188">memberSettings</span><span class="sxs-lookup"><span data-stu-id="017a9-188">memberSettings</span></span>|[<span data-ttu-id="017a9-189">teamMemberSettings</span><span class="sxs-lookup"><span data-stu-id="017a9-189">teamMemberSettings</span></span>](teammembersettings.md) |<span data-ttu-id="017a9-190">メンバーが特定のアクション (チャネルの作成、ボットの追加など) をチーム内で実行できるかどうかを構成する設定。</span><span class="sxs-lookup"><span data-stu-id="017a9-190">Settings to configure whether members can perform certain actions, for example, create channels and add bots, in the team.</span></span>|
|<span data-ttu-id="017a9-191">messagingSettings</span><span class="sxs-lookup"><span data-stu-id="017a9-191">messagingSettings</span></span>|[<span data-ttu-id="017a9-192">teamMessagingSettings</span><span class="sxs-lookup"><span data-stu-id="017a9-192">teamMessagingSettings</span></span>](teammessagingsettings.md) |<span data-ttu-id="017a9-193">チームでメッセージとメンションを構成する設定。</span><span class="sxs-lookup"><span data-stu-id="017a9-193">Settings to configure messaging and mentions in the team.</span></span>|
|<span data-ttu-id="017a9-194">webUrl</span><span class="sxs-lookup"><span data-stu-id="017a9-194">webUrl</span></span>|<span data-ttu-id="017a9-195">string (読み取り専用)</span><span class="sxs-lookup"><span data-stu-id="017a9-195">string (readonly)</span></span> | <span data-ttu-id="017a9-196">Microsoft Teams クライアントのチームに移動するハイパーリンク。</span><span class="sxs-lookup"><span data-stu-id="017a9-196">A hyperlink that will go to the team in the Microsoft Teams client.</span></span> <span data-ttu-id="017a9-197">これは、Microsoft Teams クライアントでチームを右クリックし、**[Get link to team]** を選択すると作成される URL です。</span><span class="sxs-lookup"><span data-stu-id="017a9-197">This is the URL that you get when you right-click a team in the Microsoft Teams client and select **Get link to team**.</span></span> <span data-ttu-id="017a9-198">この URL は不透明 blob として扱われる必要があり、また解析されません。</span><span class="sxs-lookup"><span data-stu-id="017a9-198">This URL should be treated as an opaque blob, and not parsed.</span></span> |

## <a name="relationships"></a><span data-ttu-id="017a9-199">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="017a9-199">Relationships</span></span>

| <span data-ttu-id="017a9-200">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="017a9-200">Relationship</span></span> | <span data-ttu-id="017a9-201">型</span><span class="sxs-lookup"><span data-stu-id="017a9-201">Type</span></span>   | <span data-ttu-id="017a9-202">説明</span><span class="sxs-lookup"><span data-stu-id="017a9-202">Description</span></span> |
|:---------------|:--------|:----------|
|<span data-ttu-id="017a9-203">apps</span><span class="sxs-lookup"><span data-stu-id="017a9-203">apps</span></span>|<span data-ttu-id="017a9-204">[teamsApp](teamsapp.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="017a9-204">[teamsApp](teamsapp.md) collection</span></span>| <span data-ttu-id="017a9-205">(現在不使用) このチームにインストールされているアプリ。</span><span class="sxs-lookup"><span data-stu-id="017a9-205">(Obsolete) The apps installed in this team.</span></span>|
|<span data-ttu-id="017a9-206">channels</span><span class="sxs-lookup"><span data-stu-id="017a9-206">channels</span></span>|<span data-ttu-id="017a9-207">[channel](channel.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="017a9-207">[channel](channel.md) collection</span></span>|<span data-ttu-id="017a9-208">チームに関連付けられているチャネルとメッセージのコレクション。</span><span class="sxs-lookup"><span data-stu-id="017a9-208">The collection of channels & messages associated with the team.</span></span>|
|<span data-ttu-id="017a9-209">installedApps</span><span class="sxs-lookup"><span data-stu-id="017a9-209">installedApps</span></span>|<span data-ttu-id="017a9-210">[teamsAppInstallation](teamsappinstallation.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="017a9-210">[teamsAppInstallation](teamsappinstallation.md) collection</span></span>|<span data-ttu-id="017a9-211">このチームにインストールされているアプリ。</span><span class="sxs-lookup"><span data-stu-id="017a9-211">The apps installed in this team.</span></span>|
|<span data-ttu-id="017a9-212">owners</span><span class="sxs-lookup"><span data-stu-id="017a9-212">owners</span></span>|[<span data-ttu-id="017a9-213">user</span><span class="sxs-lookup"><span data-stu-id="017a9-213">user</span></span>](user.md)| <span data-ttu-id="017a9-214">このチームの所有者の一覧。</span><span class="sxs-lookup"><span data-stu-id="017a9-214">The list of this team's owners.</span></span> |
|<span data-ttu-id="017a9-215">template</span><span class="sxs-lookup"><span data-stu-id="017a9-215">template</span></span>|[<span data-ttu-id="017a9-216">teamsTemplate</span><span class="sxs-lookup"><span data-stu-id="017a9-216">teamsTemplate</span></span>](teamstemplate.md)| <span data-ttu-id="017a9-217">このチームの作成元テンプレート。</span><span class="sxs-lookup"><span data-stu-id="017a9-217">The template this team was created from.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="017a9-218">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="017a9-218">JSON representation</span></span>

<span data-ttu-id="017a9-219">リソースの JSON 表記を次に示します。</span><span class="sxs-lookup"><span data-stu-id="017a9-219">The following is a JSON representation of the resource.</span></span>

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

## <a name="see-also"></a><span data-ttu-id="017a9-220">関連項目</span><span class="sxs-lookup"><span data-stu-id="017a9-220">See Also</span></span>
- [<span data-ttu-id="017a9-221">チームを使用してグループを作成する</span><span class="sxs-lookup"><span data-stu-id="017a9-221">Creating a group with a team</span></span>](/graph/teams-create-group-and-team)
- [<span data-ttu-id="017a9-222">Teams API の概要</span><span class="sxs-lookup"><span data-stu-id="017a9-222">Teams API Overview</span></span>](teams-api-overview.md)
