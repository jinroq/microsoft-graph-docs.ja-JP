---
title: チャネル リソースの種類
description: 'チャネルは、チーム内での chatMessages のコレクションです。 '
ms.openlocfilehash: 90a2c6641a79829e340f2487d7f0381998d2a205
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27073624"
---
# <a name="channel-resource-type"></a><span data-ttu-id="98167-103">チャネル リソースの種類</span><span class="sxs-lookup"><span data-stu-id="98167-103">channel resource type</span></span>

> <span data-ttu-id="98167-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="98167-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="98167-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="98167-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="98167-106">チャネルは、[チーム](../resources/team.md)内での[chatMessages](chatmessage.md)のコレクションです。</span><span class="sxs-lookup"><span data-stu-id="98167-106">A channel is a collection of [chatMessages](chatmessage.md) within a [team](../resources/team.md).</span></span> <span data-ttu-id="98167-107">チャネルでは、トピックとチーム内での議論の論理的分離を表します。</span><span class="sxs-lookup"><span data-stu-id="98167-107">A channel represents a topic, and therefore a logical isolation of discussion, within a team.</span></span> <span data-ttu-id="98167-108">例としては、「金曜日チーム ランチ」のチャネルとチャネルの「アーキテクチャの説明」にあります。</span><span class="sxs-lookup"><span data-stu-id="98167-108">Examples can be "Friday Team Lunch" channel, and "Architecture Discussion" channel.</span></span>


## <a name="methods"></a><span data-ttu-id="98167-109">メソッド</span><span class="sxs-lookup"><span data-stu-id="98167-109">Methods</span></span>

| <span data-ttu-id="98167-110">メソッド</span><span class="sxs-lookup"><span data-stu-id="98167-110">Method</span></span>       | <span data-ttu-id="98167-111">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="98167-111">Return Type</span></span>  |<span data-ttu-id="98167-112">説明</span><span class="sxs-lookup"><span data-stu-id="98167-112">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="98167-113">チャネルのリスト</span><span class="sxs-lookup"><span data-stu-id="98167-113">List channels</span></span>](../api/channel-list.md) | <span data-ttu-id="98167-114">[チャネル](channel.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="98167-114">[channel](channel.md) collection</span></span> | <span data-ttu-id="98167-115">このチームでは、チャネルの一覧を取得します。</span><span class="sxs-lookup"><span data-stu-id="98167-115">Get the list of channels in this team.</span></span>|
|[<span data-ttu-id="98167-116">チャネルを作成します。</span><span class="sxs-lookup"><span data-stu-id="98167-116">Create channel</span></span>](../api/channel-post.md) | [<span data-ttu-id="98167-117">チャネル</span><span class="sxs-lookup"><span data-stu-id="98167-117">channel</span></span>](channel.md) | <span data-ttu-id="98167-118">表示名と説明を含めることで、新しいチャネルを作成します。</span><span class="sxs-lookup"><span data-stu-id="98167-118">Create a new channel by including the display name and description.</span></span>|
|[<span data-ttu-id="98167-119">チャネルを取得します。</span><span class="sxs-lookup"><span data-stu-id="98167-119">Get channel</span></span>](../api/channel-get.md) | [<span data-ttu-id="98167-120">チャネル</span><span class="sxs-lookup"><span data-stu-id="98167-120">channel</span></span>](channel.md) | <span data-ttu-id="98167-121">チャネルのプロパティと関係を参照してください。</span><span class="sxs-lookup"><span data-stu-id="98167-121">Read properties and relationships of the channel.</span></span>|
|[<span data-ttu-id="98167-122">チャネルを更新します。</span><span class="sxs-lookup"><span data-stu-id="98167-122">Update channel</span></span>](../api/channel-patch.md) | [<span data-ttu-id="98167-123">チャネル</span><span class="sxs-lookup"><span data-stu-id="98167-123">channel</span></span>](channel.md) | <span data-ttu-id="98167-124">チャネルのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="98167-124">Update properties of the channel.</span></span>|
|[<span data-ttu-id="98167-125">チャネルを削除します。</span><span class="sxs-lookup"><span data-stu-id="98167-125">Delete channel</span></span>](../api/channel-delete.md) | <span data-ttu-id="98167-126">なし</span><span class="sxs-lookup"><span data-stu-id="98167-126">None</span></span> | <span data-ttu-id="98167-127">チャネルを削除します。</span><span class="sxs-lookup"><span data-stu-id="98167-127">Delete a channel.</span></span>|
|[<span data-ttu-id="98167-128">リストからチャネルのメッセージ</span><span class="sxs-lookup"><span data-stu-id="98167-128">List channel messages</span></span>](../api/channel-list-messages.md)  | [<span data-ttu-id="98167-129">chatMessage</span><span class="sxs-lookup"><span data-stu-id="98167-129">chatMessage</span></span>](../resources/chatmessage.md) | <span data-ttu-id="98167-130">チャネルでメッセージを取得します。</span><span class="sxs-lookup"><span data-stu-id="98167-130">Get messages in a channel</span></span> |
|[<span data-ttu-id="98167-131">チャットのスレッドを作成します。</span><span class="sxs-lookup"><span data-stu-id="98167-131">Create chat thread</span></span>](../api/channel-post-chatthreads.md) | <span data-ttu-id="98167-132">[chatThread](chatthread.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="98167-132">[chatThread](chatthread.md) collection</span></span>| <span data-ttu-id="98167-133">指定したチャンネルでのチャットのスレッドを作成します。</span><span class="sxs-lookup"><span data-stu-id="98167-133">Create a chat thread in the specified channel.</span></span>|

## <a name="properties"></a><span data-ttu-id="98167-134">プロパティ</span><span class="sxs-lookup"><span data-stu-id="98167-134">Properties</span></span>
| <span data-ttu-id="98167-135">プロパティ</span><span class="sxs-lookup"><span data-stu-id="98167-135">Property</span></span>     | <span data-ttu-id="98167-136">型</span><span class="sxs-lookup"><span data-stu-id="98167-136">Type</span></span>   |<span data-ttu-id="98167-137">説明</span><span class="sxs-lookup"><span data-stu-id="98167-137">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="98167-138">説明</span><span class="sxs-lookup"><span data-stu-id="98167-138">description</span></span>|<span data-ttu-id="98167-139">String</span><span class="sxs-lookup"><span data-stu-id="98167-139">String</span></span>|<span data-ttu-id="98167-140">チャネルの省略可能な説明です。</span><span class="sxs-lookup"><span data-stu-id="98167-140">Optional textual description for the channel.</span></span>|
|<span data-ttu-id="98167-141">displayName</span><span class="sxs-lookup"><span data-stu-id="98167-141">displayName</span></span>|<span data-ttu-id="98167-142">String</span><span class="sxs-lookup"><span data-stu-id="98167-142">String</span></span>|<span data-ttu-id="98167-143">チャネルの名前は、マイクロソフトのチーム内のユーザーに表示されます。</span><span class="sxs-lookup"><span data-stu-id="98167-143">Channel name as it will appear to the user in Microsoft Teams.</span></span>|
|<span data-ttu-id="98167-144">id</span><span class="sxs-lookup"><span data-stu-id="98167-144">id</span></span>|<span data-ttu-id="98167-145">String</span><span class="sxs-lookup"><span data-stu-id="98167-145">String</span></span>|<span data-ttu-id="98167-146">チャネルの一意の識別子です。</span><span class="sxs-lookup"><span data-stu-id="98167-146">The channels's unique identifier.</span></span> <span data-ttu-id="98167-147">読み取り専用。</span><span class="sxs-lookup"><span data-stu-id="98167-147">Read-only.</span></span>|

## <a name="relationships"></a><span data-ttu-id="98167-148">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="98167-148">Relationships</span></span>
| <span data-ttu-id="98167-149">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="98167-149">Relationship</span></span> | <span data-ttu-id="98167-150">型</span><span class="sxs-lookup"><span data-stu-id="98167-150">Type</span></span>   |<span data-ttu-id="98167-151">説明</span><span class="sxs-lookup"><span data-stu-id="98167-151">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="98167-152">messages</span><span class="sxs-lookup"><span data-stu-id="98167-152">messages</span></span>|<span data-ttu-id="98167-153">[chatMessage](chatmessage.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="98167-153">[chatMessage](chatmessage.md) collection</span></span>|<span data-ttu-id="98167-154">チャネル内のすべてのメッセージのコレクションです。</span><span class="sxs-lookup"><span data-stu-id="98167-154">A collection of all the messages in the channel.</span></span> <span data-ttu-id="98167-155">ナビゲーション プロパティです。</span><span class="sxs-lookup"><span data-stu-id="98167-155">A navigation property.</span></span> <span data-ttu-id="98167-156">Null 許容型。</span><span class="sxs-lookup"><span data-stu-id="98167-156">Nullable.</span></span> <span data-ttu-id="98167-157">現在この API のみの読み取りをサポートしていますは、ついに手書きのメッセージも。</span><span class="sxs-lookup"><span data-stu-id="98167-157">Currently this API only supports reading but will eventually support writing messages too.</span></span>|
|<span data-ttu-id="98167-158">chatThreads</span><span class="sxs-lookup"><span data-stu-id="98167-158">chatThreads</span></span>|<span data-ttu-id="98167-159">[chatThread](chatthread.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="98167-159">[chatThread](chatthread.md) collection</span></span>|<span data-ttu-id="98167-160">(これは、段階的に廃止のメッセージ プロパティを優先して) chatThreads は、新規メッセージの作成ができないメッセージの読み取りをサポートしています。</span><span class="sxs-lookup"><span data-stu-id="98167-160">(This is being phased out in favor of the messages property) chatThreads supports creating new messages but not reading messages.</span></span> <span data-ttu-id="98167-161">ChatThreads は、ナビゲーション プロパティで、null 値です。</span><span class="sxs-lookup"><span data-stu-id="98167-161">ChatThreads is a navigation property, and is Nullable.</span></span>|
|<span data-ttu-id="98167-162">タブ</span><span class="sxs-lookup"><span data-stu-id="98167-162">tabs</span></span>|<span data-ttu-id="98167-163">[teamsTab](../resources/teamstab.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="98167-163">[teamsTab](../resources/teamstab.md) collection</span></span>|<span data-ttu-id="98167-164">チャネル内のすべてのタブのコレクションです。</span><span class="sxs-lookup"><span data-stu-id="98167-164">A collection of all the tabs in the channel.</span></span> <span data-ttu-id="98167-165">ナビゲーション プロパティです。</span><span class="sxs-lookup"><span data-stu-id="98167-165">A navigation property.</span></span>|


## <a name="json-representation"></a><span data-ttu-id="98167-166">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="98167-166">JSON representation</span></span>

<span data-ttu-id="98167-167">以下は、リソースの JSON 表記です</span><span class="sxs-lookup"><span data-stu-id="98167-167">Here is a JSON representation of the resource</span></span>

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
