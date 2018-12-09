---
title: チャネル リソースの種類
description: 'チャネルは、チーム内での chatMessages のコレクションです。 '
ms.openlocfilehash: e69c0e7cdef347c59006b1dcce192e7949c2f07e
ms.sourcegitcommit: 12c6e82f1417022540e534ebadbd0e8d7fb5abde
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 12/08/2018
ms.locfileid: "27209713"
---
# <a name="channel-resource-type"></a><span data-ttu-id="2342a-103">チャネル リソースの種類</span><span class="sxs-lookup"><span data-stu-id="2342a-103">channel resource type</span></span>

> <span data-ttu-id="2342a-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="2342a-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="2342a-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="2342a-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="2342a-106">チャネルは、[チーム](../resources/team.md)内での[chatMessages](chatmessage.md)のコレクションです。</span><span class="sxs-lookup"><span data-stu-id="2342a-106">A channel is a collection of [chatMessages](chatmessage.md) within a [team](../resources/team.md).</span></span> <span data-ttu-id="2342a-107">チャネルでは、トピックとチーム内での議論の論理的分離を表します。</span><span class="sxs-lookup"><span data-stu-id="2342a-107">A channel represents a topic, and therefore a logical isolation of discussion, within a team.</span></span> <span data-ttu-id="2342a-108">例としては、「金曜日チーム ランチ」のチャネルとチャネルの「アーキテクチャの説明」にあります。</span><span class="sxs-lookup"><span data-stu-id="2342a-108">Examples can be "Friday Team Lunch" channel, and "Architecture Discussion" channel.</span></span>


## <a name="methods"></a><span data-ttu-id="2342a-109">Methods</span><span class="sxs-lookup"><span data-stu-id="2342a-109">Methods</span></span>

| <span data-ttu-id="2342a-110">メソッド</span><span class="sxs-lookup"><span data-stu-id="2342a-110">Method</span></span>       | <span data-ttu-id="2342a-111">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="2342a-111">Return Type</span></span>  |<span data-ttu-id="2342a-112">説明</span><span class="sxs-lookup"><span data-stu-id="2342a-112">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="2342a-113">チャネルのリスト</span><span class="sxs-lookup"><span data-stu-id="2342a-113">List channels</span></span>](../api/channel-list.md) | <span data-ttu-id="2342a-114">[チャネル](channel.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="2342a-114">[channel](channel.md) collection</span></span> | <span data-ttu-id="2342a-115">このチームでは、チャネルの一覧を取得します。</span><span class="sxs-lookup"><span data-stu-id="2342a-115">Get the list of channels in this team.</span></span>|
|[<span data-ttu-id="2342a-116">チャネルを作成します。</span><span class="sxs-lookup"><span data-stu-id="2342a-116">Create channel</span></span>](../api/channel-post.md) | [<span data-ttu-id="2342a-117">チャネル</span><span class="sxs-lookup"><span data-stu-id="2342a-117">channel</span></span>](channel.md) | <span data-ttu-id="2342a-118">表示名と説明を含めることで、新しいチャネルを作成します。</span><span class="sxs-lookup"><span data-stu-id="2342a-118">Create a new channel by including the display name and description.</span></span>|
|[<span data-ttu-id="2342a-119">チャネルを取得します。</span><span class="sxs-lookup"><span data-stu-id="2342a-119">Get channel</span></span>](../api/channel-get.md) | [<span data-ttu-id="2342a-120">チャネル</span><span class="sxs-lookup"><span data-stu-id="2342a-120">channel</span></span>](channel.md) | <span data-ttu-id="2342a-121">チャネルのプロパティと関係を参照してください。</span><span class="sxs-lookup"><span data-stu-id="2342a-121">Read properties and relationships of the channel.</span></span>|
|[<span data-ttu-id="2342a-122">チャネルを更新します。</span><span class="sxs-lookup"><span data-stu-id="2342a-122">Update channel</span></span>](../api/channel-patch.md) | [<span data-ttu-id="2342a-123">チャネル</span><span class="sxs-lookup"><span data-stu-id="2342a-123">channel</span></span>](channel.md) | <span data-ttu-id="2342a-124">チャネルのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="2342a-124">Update properties of the channel.</span></span>|
|[<span data-ttu-id="2342a-125">チャネルを削除します。</span><span class="sxs-lookup"><span data-stu-id="2342a-125">Delete channel</span></span>](../api/channel-delete.md) | <span data-ttu-id="2342a-126">なし</span><span class="sxs-lookup"><span data-stu-id="2342a-126">None</span></span> | <span data-ttu-id="2342a-127">チャネルを削除します。</span><span class="sxs-lookup"><span data-stu-id="2342a-127">Delete a channel.</span></span>|
|[<span data-ttu-id="2342a-128">リストからチャネルのメッセージ</span><span class="sxs-lookup"><span data-stu-id="2342a-128">List channel messages</span></span>](../api/channel-list-messages.md)  | [<span data-ttu-id="2342a-129">chatMessage</span><span class="sxs-lookup"><span data-stu-id="2342a-129">chatMessage</span></span>](../resources/chatmessage.md) | <span data-ttu-id="2342a-130">チャネルでメッセージを取得します。</span><span class="sxs-lookup"><span data-stu-id="2342a-130">Get messages in a channel</span></span> |
|[<span data-ttu-id="2342a-131">チャットのスレッドを作成します。</span><span class="sxs-lookup"><span data-stu-id="2342a-131">Create chat thread</span></span>](../api/channel-post-chatthreads.md) | <span data-ttu-id="2342a-132">[chatThread](chatthread.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="2342a-132">[chatThread](chatthread.md) collection</span></span>| <span data-ttu-id="2342a-133">指定したチャンネルでのチャットのスレッドを作成します。</span><span class="sxs-lookup"><span data-stu-id="2342a-133">Create a chat thread in the specified channel.</span></span>|

## <a name="properties"></a><span data-ttu-id="2342a-134">プロパティ</span><span class="sxs-lookup"><span data-stu-id="2342a-134">Properties</span></span>
| <span data-ttu-id="2342a-135">プロパティ</span><span class="sxs-lookup"><span data-stu-id="2342a-135">Property</span></span>     | <span data-ttu-id="2342a-136">種類</span><span class="sxs-lookup"><span data-stu-id="2342a-136">Type</span></span>   |<span data-ttu-id="2342a-137">説明</span><span class="sxs-lookup"><span data-stu-id="2342a-137">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="2342a-138">説明</span><span class="sxs-lookup"><span data-stu-id="2342a-138">description</span></span>|<span data-ttu-id="2342a-139">String</span><span class="sxs-lookup"><span data-stu-id="2342a-139">String</span></span>|<span data-ttu-id="2342a-140">チャネルの省略可能な説明です。</span><span class="sxs-lookup"><span data-stu-id="2342a-140">Optional textual description for the channel.</span></span>|
|<span data-ttu-id="2342a-141">displayName</span><span class="sxs-lookup"><span data-stu-id="2342a-141">displayName</span></span>|<span data-ttu-id="2342a-142">String</span><span class="sxs-lookup"><span data-stu-id="2342a-142">String</span></span>|<span data-ttu-id="2342a-143">チャネルの名前は、マイクロソフトのチーム内のユーザーに表示されます。</span><span class="sxs-lookup"><span data-stu-id="2342a-143">Channel name as it will appear to the user in Microsoft Teams.</span></span>|
|<span data-ttu-id="2342a-144">id</span><span class="sxs-lookup"><span data-stu-id="2342a-144">id</span></span>|<span data-ttu-id="2342a-145">String</span><span class="sxs-lookup"><span data-stu-id="2342a-145">String</span></span>|<span data-ttu-id="2342a-146">チャネルの一意の識別子です。</span><span class="sxs-lookup"><span data-stu-id="2342a-146">The channels's unique identifier.</span></span> <span data-ttu-id="2342a-147">取得のみ可能な値です。</span><span class="sxs-lookup"><span data-stu-id="2342a-147">Read-only.</span></span>|
|<span data-ttu-id="2342a-148">isFavoriteByDefault</span><span class="sxs-lookup"><span data-stu-id="2342a-148">isFavoriteByDefault</span></span>|<span data-ttu-id="2342a-149">ブール型</span><span class="sxs-lookup"><span data-stu-id="2342a-149">Boolean</span></span>|<span data-ttu-id="2342a-150">かどうかチャネルが自動的にマークされます 'お気に入り' チームのすべてのメンバーの。</span><span class="sxs-lookup"><span data-stu-id="2342a-150">Whether the channel should automatically be marked 'favorite' for all members of the team.</span></span> <span data-ttu-id="2342a-151">既定値: `false`。</span><span class="sxs-lookup"><span data-stu-id="2342a-151">Default: `false`.</span></span>|
|<span data-ttu-id="2342a-152">email</span><span class="sxs-lookup"><span data-stu-id="2342a-152">email</span></span>|<span data-ttu-id="2342a-153">ブール型</span><span class="sxs-lookup"><span data-stu-id="2342a-153">Boolean</span></span>| <span data-ttu-id="2342a-154">チャネルにメッセージを送信する電子メール アドレスです。</span><span class="sxs-lookup"><span data-stu-id="2342a-154">The email address for sending messages to the channel.</span></span> <span data-ttu-id="2342a-155">読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="2342a-155">Read-only.</span></span>|
|<span data-ttu-id="2342a-156">webUrl</span><span class="sxs-lookup"><span data-stu-id="2342a-156">webUrl</span></span>|<span data-ttu-id="2342a-157">String</span><span class="sxs-lookup"><span data-stu-id="2342a-157">String</span></span>|<span data-ttu-id="2342a-158">ハイパーリンクは、マイクロソフトのチーム内のチャネルに移動します。</span><span class="sxs-lookup"><span data-stu-id="2342a-158">A hyperlink that will navigate to the channel in Microsoft Teams.</span></span> <span data-ttu-id="2342a-159">これは、マイクロソフトのチームでチャネルを右クリックし、チャネルを取得] リンクを選択するときに表示される URL です。</span><span class="sxs-lookup"><span data-stu-id="2342a-159">This is the URL that you get when you right-click a channel in Microsoft Teams and select Get link to channel.</span></span> <span data-ttu-id="2342a-160">この URL は、非透過 blob として扱われます、解析されない必要があります。</span><span class="sxs-lookup"><span data-stu-id="2342a-160">This URL should be treated as an opaque blob, and not parsed.</span></span> <span data-ttu-id="2342a-161">読み取り専用。</span><span class="sxs-lookup"><span data-stu-id="2342a-161">Read-only.</span></span>|


## <a name="relationships"></a><span data-ttu-id="2342a-162">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="2342a-162">Relationships</span></span>
| <span data-ttu-id="2342a-163">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="2342a-163">Relationship</span></span> | <span data-ttu-id="2342a-164">型</span><span class="sxs-lookup"><span data-stu-id="2342a-164">Type</span></span>   |<span data-ttu-id="2342a-165">説明</span><span class="sxs-lookup"><span data-stu-id="2342a-165">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="2342a-166">messages</span><span class="sxs-lookup"><span data-stu-id="2342a-166">messages</span></span>|<span data-ttu-id="2342a-167">[chatMessage](chatmessage.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="2342a-167">[chatMessage](chatmessage.md) collection</span></span>|<span data-ttu-id="2342a-168">チャネル内のすべてのメッセージのコレクションです。</span><span class="sxs-lookup"><span data-stu-id="2342a-168">A collection of all the messages in the channel.</span></span> <span data-ttu-id="2342a-169">ナビゲーション プロパティです。</span><span class="sxs-lookup"><span data-stu-id="2342a-169">A navigation property.</span></span> <span data-ttu-id="2342a-170">Null 許容型。</span><span class="sxs-lookup"><span data-stu-id="2342a-170">Nullable.</span></span> <span data-ttu-id="2342a-171">現在この API のみの読み取りをサポートしていますは、ついに手書きのメッセージも。</span><span class="sxs-lookup"><span data-stu-id="2342a-171">Currently this API only supports reading but will eventually support writing messages too.</span></span>|
|<span data-ttu-id="2342a-172">chatThreads</span><span class="sxs-lookup"><span data-stu-id="2342a-172">chatThreads</span></span>|<span data-ttu-id="2342a-173">[chatThread](chatthread.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="2342a-173">[chatThread](chatthread.md) collection</span></span>|<span data-ttu-id="2342a-174">(これは、段階的に廃止のメッセージ プロパティを優先して) chatThreads は、新規メッセージの作成ができないメッセージの読み取りをサポートしています。</span><span class="sxs-lookup"><span data-stu-id="2342a-174">(This is being phased out in favor of the messages property) chatThreads supports creating new messages but not reading messages.</span></span> <span data-ttu-id="2342a-175">ChatThreads は、ナビゲーション プロパティで、null 値です。</span><span class="sxs-lookup"><span data-stu-id="2342a-175">ChatThreads is a navigation property, and is Nullable.</span></span>|
|<span data-ttu-id="2342a-176">タブ</span><span class="sxs-lookup"><span data-stu-id="2342a-176">tabs</span></span>|<span data-ttu-id="2342a-177">[teamsTab](../resources/teamstab.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="2342a-177">[teamsTab](../resources/teamstab.md) collection</span></span>|<span data-ttu-id="2342a-178">チャネル内のすべてのタブのコレクションです。</span><span class="sxs-lookup"><span data-stu-id="2342a-178">A collection of all the tabs in the channel.</span></span> <span data-ttu-id="2342a-179">ナビゲーション プロパティです。</span><span class="sxs-lookup"><span data-stu-id="2342a-179">A navigation property.</span></span>|


## <a name="json-representation"></a><span data-ttu-id="2342a-180">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="2342a-180">JSON representation</span></span>

<span data-ttu-id="2342a-181">以下は、リソースの JSON 表記です</span><span class="sxs-lookup"><span data-stu-id="2342a-181">Here is a JSON representation of the resource</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [
    "chatthreads"
  ],
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.channel"
}-->

```json
{
  "description": "string",
  "displayName": "string",
  "id": "string (identifier)",
}

```


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "channel resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
