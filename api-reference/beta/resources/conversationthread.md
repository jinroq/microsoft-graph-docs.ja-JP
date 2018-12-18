---
title: conversationThread リソースの種類
description: onversationThread は、投稿のコレクションです。
author: dkershaw10
ms.openlocfilehash: 10fc07863c0650cb3a92032d5de10da6cd7011c7
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 12/18/2018
ms.locfileid: "27323738"
---
# <a name="conversationthread-resource-type"></a><span data-ttu-id="27c67-103">conversationThread リソースの種類</span><span class="sxs-lookup"><span data-stu-id="27c67-103">conversationThread resource type</span></span>

> <span data-ttu-id="27c67-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="27c67-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="27c67-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="27c67-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="27c67-106">onversationThread は、[投稿](post.md)のコレクションです。</span><span class="sxs-lookup"><span data-stu-id="27c67-106">A conversationThread is a collection of [posts](post.md).</span></span>

<span data-ttu-id="27c67-p102">最後の投稿の受信者コレクションはスレッド全体の集計された受信者です。スレッドの受信者コレクションは増大する可能性があります。スレッドから受信者が削除されると、新しいスレッドが作成されます。</span><span class="sxs-lookup"><span data-stu-id="27c67-p102">The last post's recipients collection is the aggregated recipients of the entire thread. A thread can have a growing collection of recipients. A new thread is created when a recipient is removed from the thread.</span></span>

## <a name="methods"></a><span data-ttu-id="27c67-110">メソッド</span><span class="sxs-lookup"><span data-stu-id="27c67-110">Methods</span></span>

| <span data-ttu-id="27c67-111">メソッド</span><span class="sxs-lookup"><span data-stu-id="27c67-111">Method</span></span>       | <span data-ttu-id="27c67-112">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="27c67-112">Return Type</span></span>  |<span data-ttu-id="27c67-113">説明</span><span class="sxs-lookup"><span data-stu-id="27c67-113">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="27c67-114">スレッドを一覧表示する</span><span class="sxs-lookup"><span data-stu-id="27c67-114">List threads</span></span>](../api/group-list-threads.md) | <span data-ttu-id="27c67-115">[conversationThread](conversationthread.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="27c67-115">[conversationThread](conversationthread.md) collection</span></span> |<span data-ttu-id="27c67-116">グループのすべてのスレッドを取得します。</span><span class="sxs-lookup"><span data-stu-id="27c67-116">Get all the threads of a group.</span></span>|
|[<span data-ttu-id="27c67-117">スレッドを作成する</span><span class="sxs-lookup"><span data-stu-id="27c67-117">Create thread</span></span>](../api/group-post-threads.md) | [<span data-ttu-id="27c67-118">conversationThread</span><span class="sxs-lookup"><span data-stu-id="27c67-118">conversationThread</span></span>](conversationthread.md) |<span data-ttu-id="27c67-p103">最初にスレッドを作成して、新しい会話を開始します。グループには、新しい会話、会話スレッド、および投稿が作成されます。</span><span class="sxs-lookup"><span data-stu-id="27c67-p103">Start a new conversation by first creating a thread. A new conversation, conversation thread, and post are created in the group.</span></span>|
|[<span data-ttu-id="27c67-121">conversationThread を取得する</span><span class="sxs-lookup"><span data-stu-id="27c67-121">Get conversationThread</span></span>](../api/conversationthread-get.md) | [<span data-ttu-id="27c67-122">conversationThread</span><span class="sxs-lookup"><span data-stu-id="27c67-122">conversationThread</span></span>](conversationthread.md) |<span data-ttu-id="27c67-123">グループに属している特定のスレッドを取得します。</span><span class="sxs-lookup"><span data-stu-id="27c67-123">Get a specific thread that belongs to a group.</span></span> |
|[<span data-ttu-id="27c67-124">Update</span><span class="sxs-lookup"><span data-stu-id="27c67-124">Update</span></span>](../api/conversationthread-update.md) | [<span data-ttu-id="27c67-125">conversationThread</span><span class="sxs-lookup"><span data-stu-id="27c67-125">conversationThread</span></span>](conversationthread.md)  |<span data-ttu-id="27c67-126">conversationThread オブジェクトを更新します。</span><span class="sxs-lookup"><span data-stu-id="27c67-126">Update conversationThread object.</span></span> |
|[<span data-ttu-id="27c67-127">Delete</span><span class="sxs-lookup"><span data-stu-id="27c67-127">Delete</span></span>](../api/conversationthread-delete.md) | <span data-ttu-id="27c67-128">なし</span><span class="sxs-lookup"><span data-stu-id="27c67-128">None</span></span> |<span data-ttu-id="27c67-129">conversationThread オブジェクトを削除します。</span><span class="sxs-lookup"><span data-stu-id="27c67-129">Delete conversationThread object.</span></span> |
|[<span data-ttu-id="27c67-130">返信</span><span class="sxs-lookup"><span data-stu-id="27c67-130">reply</span></span>](../api/conversationthread-reply.md)|<span data-ttu-id="27c67-131">なし</span><span class="sxs-lookup"><span data-stu-id="27c67-131">None</span></span>|<span data-ttu-id="27c67-132">新しい投稿のエンティティを作成して、このスレッドに返信します。</span><span class="sxs-lookup"><span data-stu-id="27c67-132">Reply to this thread by creating a new Post entity.</span></span>|
|[<span data-ttu-id="27c67-133">投稿を一覧表示する</span><span class="sxs-lookup"><span data-stu-id="27c67-133">List Posts</span></span>](../api/conversationthread-list-posts.md) |<span data-ttu-id="27c67-134">[post](post.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="27c67-134">[post](post.md) collection</span></span>| <span data-ttu-id="27c67-135">指定したスレッドの投稿を取得します。</span><span class="sxs-lookup"><span data-stu-id="27c67-135">Get the posts of the specified thread.</span></span> |

## <a name="properties"></a><span data-ttu-id="27c67-136">プロパティ</span><span class="sxs-lookup"><span data-stu-id="27c67-136">Properties</span></span>
| <span data-ttu-id="27c67-137">プロパティ</span><span class="sxs-lookup"><span data-stu-id="27c67-137">Property</span></span>     | <span data-ttu-id="27c67-138">種類</span><span class="sxs-lookup"><span data-stu-id="27c67-138">Type</span></span>   |<span data-ttu-id="27c67-139">説明</span><span class="sxs-lookup"><span data-stu-id="27c67-139">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="27c67-140">ID</span><span class="sxs-lookup"><span data-stu-id="27c67-140">id</span></span>|<span data-ttu-id="27c67-141">String</span><span class="sxs-lookup"><span data-stu-id="27c67-141">String</span></span>| <span data-ttu-id="27c67-142">読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="27c67-142">Read-only.</span></span>|
|<span data-ttu-id="27c67-143">toRecipients</span><span class="sxs-lookup"><span data-stu-id="27c67-143">toRecipients</span></span>|<span data-ttu-id="27c67-144">[recipient](recipient.md) collection</span><span class="sxs-lookup"><span data-stu-id="27c67-144">[recipient](recipient.md) collection</span></span>|<span data-ttu-id="27c67-145">スレッドの宛先の受信者。</span><span class="sxs-lookup"><span data-stu-id="27c67-145">The To: recipients for the thread.</span></span>|
|<span data-ttu-id="27c67-146">ccRecipients</span><span class="sxs-lookup"><span data-stu-id="27c67-146">ccRecipients</span></span>|<span data-ttu-id="27c67-147">[recipient](recipient.md) collection</span><span class="sxs-lookup"><span data-stu-id="27c67-147">[recipient](recipient.md) collection</span></span>|<span data-ttu-id="27c67-148">スレッドの CC の受信者。</span><span class="sxs-lookup"><span data-stu-id="27c67-148">The Cc: recipients for the thread.</span></span>|
|<span data-ttu-id="27c67-149">topic</span><span class="sxs-lookup"><span data-stu-id="27c67-149">topic</span></span>|<span data-ttu-id="27c67-150">String</span><span class="sxs-lookup"><span data-stu-id="27c67-150">String</span></span>|<span data-ttu-id="27c67-p104">会話のトピックです。会話の作成時にこのプロパティを設定できますが、更新することはできません。</span><span class="sxs-lookup"><span data-stu-id="27c67-p104">The topic of the conversation. This property can be set when the conversation is created, but it cannot be updated.</span></span>||
|<span data-ttu-id="27c67-153">hasAttachments</span><span class="sxs-lookup"><span data-stu-id="27c67-153">hasAttachments</span></span>|<span data-ttu-id="27c67-154">Boolean</span><span class="sxs-lookup"><span data-stu-id="27c67-154">Boolean</span></span>|<span data-ttu-id="27c67-155">このスレッド内のいずれかの投稿に添付ファイルが 1 つ以上あるかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="27c67-155">Indicates whether any of the posts within this thread has at least one attachment.</span></span>|
|<span data-ttu-id="27c67-156">lastDeliveredDateTime</span><span class="sxs-lookup"><span data-stu-id="27c67-156">lastDeliveredDateTime</span></span>|<span data-ttu-id="27c67-157">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="27c67-157">DateTimeOffset</span></span>|<span data-ttu-id="27c67-p105">Timestamp 型は、ISO 8601 形式を使用して日付と時刻の情報を表し、必ず UTC 時間です。たとえば、2014 年 1 月 1 日午前 0 時 (UTC) は、次のようになります。`'2014-01-01T00:00:00Z'`</span><span class="sxs-lookup"><span data-stu-id="27c67-p105">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time. For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|
|<span data-ttu-id="27c67-160">uniqueSenders</span><span class="sxs-lookup"><span data-stu-id="27c67-160">uniqueSenders</span></span>|<span data-ttu-id="27c67-161">String コレクション</span><span class="sxs-lookup"><span data-stu-id="27c67-161">String collection</span></span>|<span data-ttu-id="27c67-162">このスレッドにメッセージを送信したすべてのユーザー。</span><span class="sxs-lookup"><span data-stu-id="27c67-162">All the users that sent a message to this thread.</span></span>|
|<span data-ttu-id="27c67-163">preview</span><span class="sxs-lookup"><span data-stu-id="27c67-163">preview</span></span>|<span data-ttu-id="27c67-164">String</span><span class="sxs-lookup"><span data-stu-id="27c67-164">String</span></span>|<span data-ttu-id="27c67-165">この会話における最新投稿の本文からの短い概要。</span><span class="sxs-lookup"><span data-stu-id="27c67-165">A short summary from the body of the latest post in this converstaion.</span></span>|
|<span data-ttu-id="27c67-166">isLocked</span><span class="sxs-lookup"><span data-stu-id="27c67-166">isLocked</span></span>|<span data-ttu-id="27c67-167">Boolean</span><span class="sxs-lookup"><span data-stu-id="27c67-167">Boolean</span></span>|<span data-ttu-id="27c67-168">スレッドがロックされているかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="27c67-168">Indicates if the thread is locked.</span></span>|

## <a name="relationships"></a><span data-ttu-id="27c67-169">関係</span><span class="sxs-lookup"><span data-stu-id="27c67-169">Relationships</span></span>
| <span data-ttu-id="27c67-170">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="27c67-170">Relationship</span></span> | <span data-ttu-id="27c67-171">型</span><span class="sxs-lookup"><span data-stu-id="27c67-171">Type</span></span>   |<span data-ttu-id="27c67-172">説明</span><span class="sxs-lookup"><span data-stu-id="27c67-172">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="27c67-173">投稿</span><span class="sxs-lookup"><span data-stu-id="27c67-173">posts</span></span>|<span data-ttu-id="27c67-174">[post](post.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="27c67-174">[post](post.md) collection</span></span>| <span data-ttu-id="27c67-p106">読み取り専用です。Null 許容型。</span><span class="sxs-lookup"><span data-stu-id="27c67-p106">Read-only. Nullable.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="27c67-177">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="27c67-177">JSON representation</span></span>

<span data-ttu-id="27c67-178">以下は、リソースの JSON 表記です</span><span class="sxs-lookup"><span data-stu-id="27c67-178">Here is a JSON representation of the resource</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [
    "posts"
  ],
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.conversationThread"
}-->

```json
{
  "ccRecipients": [{"@odata.type": "microsoft.graph.recipient"}],
  "hasAttachments": true,
  "id": "string (identifier)",
  "isLocked": true,
  "lastDeliveredDateTime": "String (timestamp)",
  "preview": "string",
  "toRecipients": [{"@odata.type": "microsoft.graph.recipient"}],
  "topic": "string",
  "uniqueSenders": ["string"]
}

```


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "conversationThread resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
