---
title: チャネルのリソースの種類
description: 'チャネルは、チーム内の chatMessages のコレクションです。 '
author: nkramer
localization_priority: Priority
ms.prod: microsoft-teams
ms.openlocfilehash: 1b77afb1560ed451683838a617123db013b71cd6
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/26/2019
ms.locfileid: "33338762"
---
# <a name="channel-resource-type"></a><span data-ttu-id="30ccc-103">チャネルのリソースの種類</span><span class="sxs-lookup"><span data-stu-id="30ccc-103">channel resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="30ccc-104">[チーム](../resources/team.md)はチャネルで構成されています。チャネルは、チームのメンバーと会話する場所です。</span><span class="sxs-lookup"><span data-stu-id="30ccc-104">[Teams](../resources/team.md) are made up of channels, which are the conversations you have with your teammates.</span></span> <span data-ttu-id="30ccc-105">各チャネルは、特定のトピック、部門、プロジェクト専用です。</span><span class="sxs-lookup"><span data-stu-id="30ccc-105">Each channel is dedicated to a specific topic, department, or project.</span></span>
<span data-ttu-id="30ccc-106">チャネルは、実際に作業を行う場所、チーム全体に対してテキスト、音声、ビデオによる会話を公開する場所、ファイルを共有する場所、タブを追加する場所です。</span><span class="sxs-lookup"><span data-stu-id="30ccc-106">Channels are where the work actually gets done - where text, audio, and video conversations open to the whole team happen, where files are shared, and where tabs are added.</span></span>

## <a name="methods"></a><span data-ttu-id="30ccc-107">メソッド</span><span class="sxs-lookup"><span data-stu-id="30ccc-107">Methods</span></span>

| <span data-ttu-id="30ccc-108">メソッド</span><span class="sxs-lookup"><span data-stu-id="30ccc-108">Method</span></span>       | <span data-ttu-id="30ccc-109">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="30ccc-109">Return Type</span></span>  |<span data-ttu-id="30ccc-110">説明</span><span class="sxs-lookup"><span data-stu-id="30ccc-110">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="30ccc-111">チャネルを一覧表示する</span><span class="sxs-lookup"><span data-stu-id="30ccc-111">List channels</span></span>](../api/channel-list.md) | <span data-ttu-id="30ccc-112">[channel](channel.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="30ccc-112">[channel](channel.md) collection</span></span> | <span data-ttu-id="30ccc-113">このチーム内のチャネルの一覧を取得します。</span><span class="sxs-lookup"><span data-stu-id="30ccc-113">Get the list of channels in this team.</span></span>|
|[<span data-ttu-id="30ccc-114">チャネルを作成する</span><span class="sxs-lookup"><span data-stu-id="30ccc-114">Create channel</span></span>](../api/channel-post.md) | [<span data-ttu-id="30ccc-115">channel</span><span class="sxs-lookup"><span data-stu-id="30ccc-115">channel</span></span>](channel.md) | <span data-ttu-id="30ccc-116">表示名と説明を指定して新しいチャネルを作成します。</span><span class="sxs-lookup"><span data-stu-id="30ccc-116">Create a new channel by including the display name and description.</span></span>|
|[<span data-ttu-id="30ccc-117">チャネルを取得する</span><span class="sxs-lookup"><span data-stu-id="30ccc-117">Get channel</span></span>](../api/channel-get.md) | [<span data-ttu-id="30ccc-118">channel</span><span class="sxs-lookup"><span data-stu-id="30ccc-118">channel</span></span>](channel.md) | <span data-ttu-id="30ccc-119">チャネルのプロパティとリレーションシップを読み取ります。</span><span class="sxs-lookup"><span data-stu-id="30ccc-119">Read properties and relationships of the channel.</span></span>|
|[<span data-ttu-id="30ccc-120">チャネルを更新する</span><span class="sxs-lookup"><span data-stu-id="30ccc-120">Update channel</span></span>](../api/channel-patch.md) | [<span data-ttu-id="30ccc-121">channel</span><span class="sxs-lookup"><span data-stu-id="30ccc-121">channel</span></span>](channel.md) | <span data-ttu-id="30ccc-122">チャネルのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="30ccc-122">Update properties of the channel.</span></span>|
|[<span data-ttu-id="30ccc-123">チャネルを削除する</span><span class="sxs-lookup"><span data-stu-id="30ccc-123">Delete channel</span></span>](../api/channel-delete.md) | <span data-ttu-id="30ccc-124">なし</span><span class="sxs-lookup"><span data-stu-id="30ccc-124">None</span></span> | <span data-ttu-id="30ccc-125">チャネルを削除します。</span><span class="sxs-lookup"><span data-stu-id="30ccc-125">Delete a channel.</span></span>|
|[<span data-ttu-id="30ccc-126">チャネル メッセージを一覧表示する</span><span class="sxs-lookup"><span data-stu-id="30ccc-126">List channel messages</span></span>](../api/channel-list-messages.md)  | [<span data-ttu-id="30ccc-127">chatMessage</span><span class="sxs-lookup"><span data-stu-id="30ccc-127">chatMessage</span></span>](../resources/chatmessage.md) | <span data-ttu-id="30ccc-128">チャネルのメッセージを取得します。</span><span class="sxs-lookup"><span data-stu-id="30ccc-128">Get messages in a channel</span></span> |
|[<span data-ttu-id="30ccc-129">チャネル メッセージを送信する</span><span class="sxs-lookup"><span data-stu-id="30ccc-129">Send channel message</span></span>](../api/channel-post-chatmessage.md)  | [<span data-ttu-id="30ccc-130">chatMessage</span><span class="sxs-lookup"><span data-stu-id="30ccc-130">chatMessage</span></span>](../resources/chatmessage.md) | [<span data-ttu-id="30ccc-131">メッセージをチャネルに送信する</span><span class="sxs-lookup"><span data-stu-id="30ccc-131">Send a message to a channel</span></span>](../api/channel-post-chatmessage.md) |
|[<span data-ttu-id="30ccc-132">タブを一覧表示する</span><span class="sxs-lookup"><span data-stu-id="30ccc-132">List tabs</span></span>](../api/teamstab-list.md) | [<span data-ttu-id="30ccc-133">teamsTab</span><span class="sxs-lookup"><span data-stu-id="30ccc-133">teamsTab</span></span>](teamstab.md) | <span data-ttu-id="30ccc-134">チャネルにピン留めされているタブを一覧表示します。</span><span class="sxs-lookup"><span data-stu-id="30ccc-134">Lists tabs pinned to a channel.</span></span>|
|[<span data-ttu-id="30ccc-135">タブを取得する</span><span class="sxs-lookup"><span data-stu-id="30ccc-135">Get tab</span></span>](../api/teamstab-get.md) | [<span data-ttu-id="30ccc-136">teamsTab</span><span class="sxs-lookup"><span data-stu-id="30ccc-136">teamsTab</span></span>](teamstab.md) | <span data-ttu-id="30ccc-137">チャネルにピン留めされているタブを読み取ります。</span><span class="sxs-lookup"><span data-stu-id="30ccc-137">Reads a tab pinned to a channel.</span></span>|
|[<span data-ttu-id="30ccc-138">タブを追加する</span><span class="sxs-lookup"><span data-stu-id="30ccc-138">Add tab</span></span>](../api/teamstab-add.md) | [<span data-ttu-id="30ccc-139">teamsTab</span><span class="sxs-lookup"><span data-stu-id="30ccc-139">teamsTab</span></span>](teamstab.md) | <span data-ttu-id="30ccc-140">タブをチャネルに追加 (ピン留め) します。</span><span class="sxs-lookup"><span data-stu-id="30ccc-140">Adds (installs) a tab to a team's channel.</span></span>|
|[<span data-ttu-id="30ccc-141">タブを削除する</span><span class="sxs-lookup"><span data-stu-id="30ccc-141">Remove tab</span></span>](../api/teamstab-delete.md) | <span data-ttu-id="30ccc-142">なし</span><span class="sxs-lookup"><span data-stu-id="30ccc-142">None</span></span> | <span data-ttu-id="30ccc-143">チャネルからタブを削除します (ピン留めを外します)。</span><span class="sxs-lookup"><span data-stu-id="30ccc-143">Removes (unpins) a tab from a channel.</span></span>|
|[<span data-ttu-id="30ccc-144">タブを更新する</span><span class="sxs-lookup"><span data-stu-id="30ccc-144">Update tab</span></span>](../api/teamstab-update.md) | [<span data-ttu-id="30ccc-145">teamsTab</span><span class="sxs-lookup"><span data-stu-id="30ccc-145">teamsTab</span></span>](teamstab.md) | <span data-ttu-id="30ccc-146">タブのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="30ccc-146">Updates the tab properties.</span></span>|


## <a name="properties"></a><span data-ttu-id="30ccc-147">プロパティ</span><span class="sxs-lookup"><span data-stu-id="30ccc-147">Properties</span></span>
| <span data-ttu-id="30ccc-148">プロパティ</span><span class="sxs-lookup"><span data-stu-id="30ccc-148">Property</span></span>     | <span data-ttu-id="30ccc-149">型</span><span class="sxs-lookup"><span data-stu-id="30ccc-149">Type</span></span>   |<span data-ttu-id="30ccc-150">説明</span><span class="sxs-lookup"><span data-stu-id="30ccc-150">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="30ccc-151">description</span><span class="sxs-lookup"><span data-stu-id="30ccc-151">description</span></span>|<span data-ttu-id="30ccc-152">String</span><span class="sxs-lookup"><span data-stu-id="30ccc-152">String</span></span>|<span data-ttu-id="30ccc-153">チャネルの説明テキストです (省略可能)。</span><span class="sxs-lookup"><span data-stu-id="30ccc-153">Optional textual description for the channel.</span></span>|
|<span data-ttu-id="30ccc-154">displayName</span><span class="sxs-lookup"><span data-stu-id="30ccc-154">displayName</span></span>|<span data-ttu-id="30ccc-155">String</span><span class="sxs-lookup"><span data-stu-id="30ccc-155">String</span></span>|<span data-ttu-id="30ccc-156">Microsoft Teams でユーザーに対して表示されるチャネルの名前。</span><span class="sxs-lookup"><span data-stu-id="30ccc-156">Channel name as it will appear to the user in Microsoft Teams.</span></span>|
|<span data-ttu-id="30ccc-157">id</span><span class="sxs-lookup"><span data-stu-id="30ccc-157">id</span></span>|<span data-ttu-id="30ccc-158">String</span><span class="sxs-lookup"><span data-stu-id="30ccc-158">String</span></span>|<span data-ttu-id="30ccc-159">チャネルの一意の識別子。</span><span class="sxs-lookup"><span data-stu-id="30ccc-159">The channels's unique identifier.</span></span> <span data-ttu-id="30ccc-160">読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="30ccc-160">Read-only.</span></span>|
|<span data-ttu-id="30ccc-161">isFavoriteByDefault</span><span class="sxs-lookup"><span data-stu-id="30ccc-161">isFavoriteByDefault</span></span>|<span data-ttu-id="30ccc-162">Boolean</span><span class="sxs-lookup"><span data-stu-id="30ccc-162">Boolean</span></span>|<span data-ttu-id="30ccc-163">チームのメンバー全員に対してチャネルを「お気に入り」として自動的にマークするかどうか。</span><span class="sxs-lookup"><span data-stu-id="30ccc-163">Whether the channel should automatically be marked 'favorite' for all members of the team.</span></span> <span data-ttu-id="30ccc-164">既定値: `false`。</span><span class="sxs-lookup"><span data-stu-id="30ccc-164">Default: `false`.</span></span>|
|<span data-ttu-id="30ccc-165">メール</span><span class="sxs-lookup"><span data-stu-id="30ccc-165">email</span></span>|<span data-ttu-id="30ccc-166">String</span><span class="sxs-lookup"><span data-stu-id="30ccc-166">String</span></span>| <span data-ttu-id="30ccc-167">チャネルにメッセージを送信するときのメール アドレス。</span><span class="sxs-lookup"><span data-stu-id="30ccc-167">The email address for sending messages to the channel.</span></span> <span data-ttu-id="30ccc-168">読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="30ccc-168">Read-only.</span></span>|
|<span data-ttu-id="30ccc-169">webUrl</span><span class="sxs-lookup"><span data-stu-id="30ccc-169">webUrl</span></span>|<span data-ttu-id="30ccc-170">String</span><span class="sxs-lookup"><span data-stu-id="30ccc-170">String</span></span>|<span data-ttu-id="30ccc-171">Microsoft Teams のチャネルに移動するハイパーリンク。</span><span class="sxs-lookup"><span data-stu-id="30ccc-171">A hyperlink that will navigate to the channel in Microsoft Teams.</span></span> <span data-ttu-id="30ccc-172">これは、Microsoft Teams でチャネルを右クリックし、[チームへのリンクを取得] を選択すると作成される URL です。</span><span class="sxs-lookup"><span data-stu-id="30ccc-172">This is the URL that you get when you right-click a channel in Microsoft Teams and select Get link to channel.</span></span> <span data-ttu-id="30ccc-173">この URL は不透明 blob として扱われる必要があり、また解析されません。</span><span class="sxs-lookup"><span data-stu-id="30ccc-173">This URL should be treated as an opaque blob, and not parsed.</span></span> <span data-ttu-id="30ccc-174">読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="30ccc-174">Read-only.</span></span>|


## <a name="relationships"></a><span data-ttu-id="30ccc-175">関係</span><span class="sxs-lookup"><span data-stu-id="30ccc-175">Relationships</span></span>
| <span data-ttu-id="30ccc-176">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="30ccc-176">Relationship</span></span> | <span data-ttu-id="30ccc-177">型</span><span class="sxs-lookup"><span data-stu-id="30ccc-177">Type</span></span>   |<span data-ttu-id="30ccc-178">説明</span><span class="sxs-lookup"><span data-stu-id="30ccc-178">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="30ccc-179">messages</span><span class="sxs-lookup"><span data-stu-id="30ccc-179">messages</span></span>|<span data-ttu-id="30ccc-180">[chatMessage](chatmessage.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="30ccc-180">[chatMessage](chatmessage.md) collection</span></span>|<span data-ttu-id="30ccc-181">チャネル内のすべてのメッセージのコレクションです。</span><span class="sxs-lookup"><span data-stu-id="30ccc-181">A collection of all the messages in the channel.</span></span> <span data-ttu-id="30ccc-182">ナビゲーションのプロパティです。</span><span class="sxs-lookup"><span data-stu-id="30ccc-182">A navigation property.</span></span> <span data-ttu-id="30ccc-183">Null 許容型です。</span><span class="sxs-lookup"><span data-stu-id="30ccc-183">Nullable.</span></span> <span data-ttu-id="30ccc-184">現在この API では読み取りだけがサポートされていますが、最終的にはメッセージの作成もサポートされる予定です。</span><span class="sxs-lookup"><span data-stu-id="30ccc-184">Currently this API only supports reading but will eventually support writing messages too.</span></span>|
|<span data-ttu-id="30ccc-185">tabs</span><span class="sxs-lookup"><span data-stu-id="30ccc-185">tabs</span></span>|<span data-ttu-id="30ccc-186">[teamsTab](../resources/teamstab.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="30ccc-186">[teamsTab](../resources/teamstab.md) collection</span></span>|<span data-ttu-id="30ccc-187">チャネル内のすべてのタブのコレクションです。</span><span class="sxs-lookup"><span data-stu-id="30ccc-187">A collection of all the tabs in the channel.</span></span> <span data-ttu-id="30ccc-188">ナビゲーションのプロパティです。</span><span class="sxs-lookup"><span data-stu-id="30ccc-188">A navigation property.</span></span>|


## <a name="json-representation"></a><span data-ttu-id="30ccc-189">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="30ccc-189">JSON representation</span></span>

<span data-ttu-id="30ccc-190">以下は、リソースの JSON 表記です</span><span class="sxs-lookup"><span data-stu-id="30ccc-190">Here is a JSON representation of the resource</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [
    "messages"
  ],
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.channel"
}-->

```json
{
  "description": "string",
  "displayName": "string",
  "id": "string (identifier)",
  "isFavoriteByDefault": true,
  "email": "string",
  "webUrl": "string"
}
```


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "channel resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
