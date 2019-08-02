---
title: チャネルのリソースの種類
description: 'チャネルは、チーム内の chatMessages のコレクションです。 '
author: nkramer
localization_priority: Priority
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: f78d6e8730e5f8168cbff94fa03dfbf5287dc5ef
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "36012990"
---
# <a name="channel-resource-type"></a><span data-ttu-id="7b38c-103">チャネルのリソースの種類</span><span class="sxs-lookup"><span data-stu-id="7b38c-103">channel resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="7b38c-104">[チーム](../resources/team.md)はチャネルで構成されています。チャネルは、チームのメンバーと会話する場所です。</span><span class="sxs-lookup"><span data-stu-id="7b38c-104">[Teams](../resources/team.md) are made up of channels, which are the conversations you have with your teammates.</span></span> <span data-ttu-id="7b38c-105">各チャネルは、特定のトピック、部門、プロジェクト専用です。</span><span class="sxs-lookup"><span data-stu-id="7b38c-105">Each channel is dedicated to a specific topic, department, or project.</span></span>
<span data-ttu-id="7b38c-106">チャネルは、実際に作業を行う場所、チーム全体に対してテキスト、音声、ビデオによる会話を公開する場所、ファイルを共有する場所、タブを追加する場所です。</span><span class="sxs-lookup"><span data-stu-id="7b38c-106">Channels are where the work actually gets done - where text, audio, and video conversations open to the whole team happen, where files are shared, and where tabs are added.</span></span>

## <a name="methods"></a><span data-ttu-id="7b38c-107">メソッド</span><span class="sxs-lookup"><span data-stu-id="7b38c-107">Methods</span></span>

| <span data-ttu-id="7b38c-108">メソッド</span><span class="sxs-lookup"><span data-stu-id="7b38c-108">Method</span></span>       | <span data-ttu-id="7b38c-109">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="7b38c-109">Return Type</span></span>  |<span data-ttu-id="7b38c-110">説明</span><span class="sxs-lookup"><span data-stu-id="7b38c-110">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="7b38c-111">チャネルを一覧表示する</span><span class="sxs-lookup"><span data-stu-id="7b38c-111">List channels</span></span>](../api/channel-list.md) | <span data-ttu-id="7b38c-112">[channel](channel.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="7b38c-112">[channel](channel.md) collection</span></span> | <span data-ttu-id="7b38c-113">このチーム内のチャネルの一覧を取得します。</span><span class="sxs-lookup"><span data-stu-id="7b38c-113">Get the list of channels in this team.</span></span>|
|[<span data-ttu-id="7b38c-114">チャネルを作成する</span><span class="sxs-lookup"><span data-stu-id="7b38c-114">Create channel</span></span>](../api/channel-post.md) | [<span data-ttu-id="7b38c-115">channel</span><span class="sxs-lookup"><span data-stu-id="7b38c-115">channel</span></span>](channel.md) | <span data-ttu-id="7b38c-116">表示名と説明を指定して新しいチャネルを作成します。</span><span class="sxs-lookup"><span data-stu-id="7b38c-116">Create a new channel by including the display name and description.</span></span>|
|[<span data-ttu-id="7b38c-117">チャネルを取得する</span><span class="sxs-lookup"><span data-stu-id="7b38c-117">Get channel</span></span>](../api/channel-get.md) | [<span data-ttu-id="7b38c-118">channel</span><span class="sxs-lookup"><span data-stu-id="7b38c-118">channel</span></span>](channel.md) | <span data-ttu-id="7b38c-119">チャネルのプロパティとリレーションシップを読み取ります。</span><span class="sxs-lookup"><span data-stu-id="7b38c-119">Read properties and relationships of the channel.</span></span>|
|[<span data-ttu-id="7b38c-120">チャネルを更新する</span><span class="sxs-lookup"><span data-stu-id="7b38c-120">Update channel</span></span>](../api/channel-patch.md) | [<span data-ttu-id="7b38c-121">channel</span><span class="sxs-lookup"><span data-stu-id="7b38c-121">channel</span></span>](channel.md) | <span data-ttu-id="7b38c-122">チャネルのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="7b38c-122">Update properties of the channel.</span></span>|
|[<span data-ttu-id="7b38c-123">チャネルを削除する</span><span class="sxs-lookup"><span data-stu-id="7b38c-123">Delete channel</span></span>](../api/channel-delete.md) | <span data-ttu-id="7b38c-124">なし</span><span class="sxs-lookup"><span data-stu-id="7b38c-124">None</span></span> | <span data-ttu-id="7b38c-125">チャネルを削除します。</span><span class="sxs-lookup"><span data-stu-id="7b38c-125">Delete a channel.</span></span>|
|[<span data-ttu-id="7b38c-126">チャネル メッセージを一覧表示する</span><span class="sxs-lookup"><span data-stu-id="7b38c-126">List channel messages</span></span>](../api/channel-list-messages.md)  | [<span data-ttu-id="7b38c-127">chatMessage</span><span class="sxs-lookup"><span data-stu-id="7b38c-127">chatMessage</span></span>](../resources/chatmessage.md) | <span data-ttu-id="7b38c-128">チャネルのメッセージを取得します。</span><span class="sxs-lookup"><span data-stu-id="7b38c-128">Get messages in a channel</span></span> |
|[<span data-ttu-id="7b38c-129">チャネルでの chatMessage の作成</span><span class="sxs-lookup"><span data-stu-id="7b38c-129">Create chatMessage in a channel</span></span>](../api/channel-post-messages.md) | [<span data-ttu-id="7b38c-130">chatMessage</span><span class="sxs-lookup"><span data-stu-id="7b38c-130">chatMessage</span></span>](../resources/chatmessage.md) | <span data-ttu-id="7b38c-131">メッセージをチャネルに送信します。</span><span class="sxs-lookup"><span data-stu-id="7b38c-131">Send a message to a channel</span></span> |
|[<span data-ttu-id="7b38c-132">チャネルでの chatMessage 返信の作成</span><span class="sxs-lookup"><span data-stu-id="7b38c-132">Create chatMessage reply in a channel</span></span>](../api/channel-post-messagereply.md) | [<span data-ttu-id="7b38c-133">chatMessage</span><span class="sxs-lookup"><span data-stu-id="7b38c-133">chatMessage</span></span>](../resources/chatmessage.md) | <span data-ttu-id="7b38c-134">チャネル内のメッセージに返信します。</span><span class="sxs-lookup"><span data-stu-id="7b38c-134">Reply to a message in a channel</span></span>|
|[<span data-ttu-id="7b38c-135">タブを一覧表示する</span><span class="sxs-lookup"><span data-stu-id="7b38c-135">List tabs</span></span>](../api/teamstab-list.md) | [<span data-ttu-id="7b38c-136">teamsTab</span><span class="sxs-lookup"><span data-stu-id="7b38c-136">teamsTab</span></span>](teamstab.md) | <span data-ttu-id="7b38c-137">チャネルにピン留めされているタブを一覧表示します。</span><span class="sxs-lookup"><span data-stu-id="7b38c-137">Lists tabs pinned to a channel.</span></span>|
|[<span data-ttu-id="7b38c-138">タブを取得する</span><span class="sxs-lookup"><span data-stu-id="7b38c-138">Get tab</span></span>](../api/teamstab-get.md) | [<span data-ttu-id="7b38c-139">teamsTab</span><span class="sxs-lookup"><span data-stu-id="7b38c-139">teamsTab</span></span>](teamstab.md) | <span data-ttu-id="7b38c-140">チャネルにピン留めされているタブを読み取ります。</span><span class="sxs-lookup"><span data-stu-id="7b38c-140">Reads a tab pinned to a channel.</span></span>|
|[<span data-ttu-id="7b38c-141">タブを追加する</span><span class="sxs-lookup"><span data-stu-id="7b38c-141">Add tab</span></span>](../api/teamstab-add.md) | [<span data-ttu-id="7b38c-142">teamsTab</span><span class="sxs-lookup"><span data-stu-id="7b38c-142">teamsTab</span></span>](teamstab.md) | <span data-ttu-id="7b38c-143">タブをチャネルに追加 (ピン留め) します。</span><span class="sxs-lookup"><span data-stu-id="7b38c-143">Adds (pins) a tab to a channel.</span></span>|
|[<span data-ttu-id="7b38c-144">タブを削除する</span><span class="sxs-lookup"><span data-stu-id="7b38c-144">Remove tab</span></span>](../api/teamstab-delete.md) | <span data-ttu-id="7b38c-145">なし</span><span class="sxs-lookup"><span data-stu-id="7b38c-145">None</span></span> | <span data-ttu-id="7b38c-146">チャネルからタブを削除します (ピン留めを外します)。</span><span class="sxs-lookup"><span data-stu-id="7b38c-146">Removes (unpins) a tab from a channel.</span></span>|
|[<span data-ttu-id="7b38c-147">タブを更新する</span><span class="sxs-lookup"><span data-stu-id="7b38c-147">Update tab</span></span>](../api/teamstab-update.md) | [<span data-ttu-id="7b38c-148">teamsTab</span><span class="sxs-lookup"><span data-stu-id="7b38c-148">teamsTab</span></span>](teamstab.md) | <span data-ttu-id="7b38c-149">タブのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="7b38c-149">Updates the tab properties.</span></span>|


## <a name="properties"></a><span data-ttu-id="7b38c-150">プロパティ</span><span class="sxs-lookup"><span data-stu-id="7b38c-150">Properties</span></span>
| <span data-ttu-id="7b38c-151">プロパティ</span><span class="sxs-lookup"><span data-stu-id="7b38c-151">Property</span></span>     | <span data-ttu-id="7b38c-152">型</span><span class="sxs-lookup"><span data-stu-id="7b38c-152">Type</span></span>   |<span data-ttu-id="7b38c-153">説明</span><span class="sxs-lookup"><span data-stu-id="7b38c-153">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="7b38c-154">description</span><span class="sxs-lookup"><span data-stu-id="7b38c-154">description</span></span>|<span data-ttu-id="7b38c-155">String</span><span class="sxs-lookup"><span data-stu-id="7b38c-155">String</span></span>|<span data-ttu-id="7b38c-156">チャネルの説明テキストです (省略可能)。</span><span class="sxs-lookup"><span data-stu-id="7b38c-156">Optional textual description for the channel.</span></span>|
|<span data-ttu-id="7b38c-157">displayName</span><span class="sxs-lookup"><span data-stu-id="7b38c-157">displayName</span></span>|<span data-ttu-id="7b38c-158">String</span><span class="sxs-lookup"><span data-stu-id="7b38c-158">String</span></span>|<span data-ttu-id="7b38c-159">Microsoft Teams でユーザーに対して表示されるチャネルの名前。</span><span class="sxs-lookup"><span data-stu-id="7b38c-159">Channel name as it will appear to the user in Microsoft Teams.</span></span>|
|<span data-ttu-id="7b38c-160">id</span><span class="sxs-lookup"><span data-stu-id="7b38c-160">id</span></span>|<span data-ttu-id="7b38c-161">String</span><span class="sxs-lookup"><span data-stu-id="7b38c-161">String</span></span>|<span data-ttu-id="7b38c-162">チャネルの一意の識別子。</span><span class="sxs-lookup"><span data-stu-id="7b38c-162">The channels's unique identifier.</span></span> <span data-ttu-id="7b38c-163">読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="7b38c-163">Read-only.</span></span>|
|<span data-ttu-id="7b38c-164">isFavoriteByDefault</span><span class="sxs-lookup"><span data-stu-id="7b38c-164">isFavoriteByDefault</span></span>|<span data-ttu-id="7b38c-165">Boolean</span><span class="sxs-lookup"><span data-stu-id="7b38c-165">Boolean</span></span>|<span data-ttu-id="7b38c-166">チームのメンバー全員に対してチャネルを「お気に入り」として自動的にマークするかどうか。</span><span class="sxs-lookup"><span data-stu-id="7b38c-166">Whether the channel should automatically be marked 'favorite' for all members of the team.</span></span> <span data-ttu-id="7b38c-167">既定値: `false`。</span><span class="sxs-lookup"><span data-stu-id="7b38c-167">Default: `false`.</span></span>|
|<span data-ttu-id="7b38c-168">メール</span><span class="sxs-lookup"><span data-stu-id="7b38c-168">email</span></span>|<span data-ttu-id="7b38c-169">String</span><span class="sxs-lookup"><span data-stu-id="7b38c-169">String</span></span>| <span data-ttu-id="7b38c-170">チャネルにメッセージを送信するときのメール アドレス。</span><span class="sxs-lookup"><span data-stu-id="7b38c-170">The email address for sending messages to the channel.</span></span> <span data-ttu-id="7b38c-171">読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="7b38c-171">Read-only.</span></span>|
|<span data-ttu-id="7b38c-172">webUrl</span><span class="sxs-lookup"><span data-stu-id="7b38c-172">webUrl</span></span>|<span data-ttu-id="7b38c-173">String</span><span class="sxs-lookup"><span data-stu-id="7b38c-173">String</span></span>|<span data-ttu-id="7b38c-174">Microsoft Teams のチャネルに移動するハイパーリンク。</span><span class="sxs-lookup"><span data-stu-id="7b38c-174">A hyperlink that will navigate to the channel in Microsoft Teams.</span></span> <span data-ttu-id="7b38c-175">これは、Microsoft Teams でチャネルを右クリックし、[チームへのリンクを取得] を選択すると作成される URL です。</span><span class="sxs-lookup"><span data-stu-id="7b38c-175">This is the URL that you get when you right-click a channel in Microsoft Teams and select Get link to channel.</span></span> <span data-ttu-id="7b38c-176">この URL は不透明 blob として扱われる必要があり、また解析されません。</span><span class="sxs-lookup"><span data-stu-id="7b38c-176">This URL should be treated as an opaque blob, and not parsed.</span></span> <span data-ttu-id="7b38c-177">読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="7b38c-177">Read-only.</span></span>|


## <a name="relationships"></a><span data-ttu-id="7b38c-178">関係</span><span class="sxs-lookup"><span data-stu-id="7b38c-178">Relationships</span></span>
| <span data-ttu-id="7b38c-179">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="7b38c-179">Relationship</span></span> | <span data-ttu-id="7b38c-180">型</span><span class="sxs-lookup"><span data-stu-id="7b38c-180">Type</span></span>   |<span data-ttu-id="7b38c-181">説明</span><span class="sxs-lookup"><span data-stu-id="7b38c-181">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="7b38c-182">messages</span><span class="sxs-lookup"><span data-stu-id="7b38c-182">messages</span></span>|<span data-ttu-id="7b38c-183">[chatMessage](chatmessage.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="7b38c-183">[chatMessage](chatmessage.md) collection</span></span>|<span data-ttu-id="7b38c-184">チャネル内のすべてのメッセージのコレクションです。</span><span class="sxs-lookup"><span data-stu-id="7b38c-184">A collection of all the messages in the channel.</span></span> <span data-ttu-id="7b38c-185">ナビゲーションのプロパティです。</span><span class="sxs-lookup"><span data-stu-id="7b38c-185">A navigation property.</span></span> <span data-ttu-id="7b38c-186">Null 許容型です。</span><span class="sxs-lookup"><span data-stu-id="7b38c-186">Nullable.</span></span> <span data-ttu-id="7b38c-187">現在この API では読み取りだけがサポートされていますが、最終的にはメッセージの作成もサポートされる予定です。</span><span class="sxs-lookup"><span data-stu-id="7b38c-187">Currently this API only supports reading but will eventually support writing messages too.</span></span>|
|<span data-ttu-id="7b38c-188">tabs</span><span class="sxs-lookup"><span data-stu-id="7b38c-188">tabs</span></span>|<span data-ttu-id="7b38c-189">[teamsTab](../resources/teamstab.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="7b38c-189">[teamsTab](../resources/teamstab.md) collection</span></span>|<span data-ttu-id="7b38c-190">チャネル内のすべてのタブのコレクションです。</span><span class="sxs-lookup"><span data-stu-id="7b38c-190">A collection of all the tabs in the channel.</span></span> <span data-ttu-id="7b38c-191">ナビゲーションのプロパティです。</span><span class="sxs-lookup"><span data-stu-id="7b38c-191">A navigation property.</span></span>|


## <a name="json-representation"></a><span data-ttu-id="7b38c-192">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="7b38c-192">JSON representation</span></span>

<span data-ttu-id="7b38c-193">以下は、リソースの JSON 表記です</span><span class="sxs-lookup"><span data-stu-id="7b38c-193">Here is a JSON representation of the resource</span></span>

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
