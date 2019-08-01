---
title: conversationThread リソースの種類
description: onversationThread は、投稿のコレクションです。
author: dkershaw10
localization_priority: Normal
ms.prod: groups
doc_type: resourcePageType
ms.openlocfilehash: 59e54733a0ece0c6fa4bef31282cf30939b676ba
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "36032824"
---
# <a name="conversationthread-resource-type"></a><span data-ttu-id="1859d-103">conversationThread リソースの種類</span><span class="sxs-lookup"><span data-stu-id="1859d-103">conversationThread resource type</span></span>
<span data-ttu-id="1859d-104">onversationThread は、[投稿](post.md)のコレクションです。</span><span class="sxs-lookup"><span data-stu-id="1859d-104">A conversationThread is a collection of [posts](post.md).</span></span>

<span data-ttu-id="1859d-p101">最後の投稿の受信者コレクションはスレッド全体の集計された受信者です。スレッドの受信者コレクションは増大する可能性があります。スレッドから受信者が削除されると、新しいスレッドが作成されます。</span><span class="sxs-lookup"><span data-stu-id="1859d-p101">The last post's recipients collection is the aggregated recipients of the entire thread. A thread can have a growing collection of recipients. A new thread is created when a recipient is removed from the thread.</span></span>

## <a name="methods"></a><span data-ttu-id="1859d-108">メソッド</span><span class="sxs-lookup"><span data-stu-id="1859d-108">Methods</span></span>

| <span data-ttu-id="1859d-109">メソッド</span><span class="sxs-lookup"><span data-stu-id="1859d-109">Method</span></span>       | <span data-ttu-id="1859d-110">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="1859d-110">Return Type</span></span>  |<span data-ttu-id="1859d-111">説明</span><span class="sxs-lookup"><span data-stu-id="1859d-111">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="1859d-112">スレッドを一覧表示する</span><span class="sxs-lookup"><span data-stu-id="1859d-112">List threads</span></span>](../api/group-list-threads.md) | <span data-ttu-id="1859d-113">[conversationThread](conversationthread.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="1859d-113">[conversationThread](conversationthread.md) collection</span></span> |<span data-ttu-id="1859d-114">グループのすべてのスレッドを取得します。</span><span class="sxs-lookup"><span data-stu-id="1859d-114">Get all the threads of a group.</span></span>|
|[<span data-ttu-id="1859d-115">スレッドを作成する</span><span class="sxs-lookup"><span data-stu-id="1859d-115">Create thread</span></span>](../api/group-post-threads.md) | [<span data-ttu-id="1859d-116">conversationThread</span><span class="sxs-lookup"><span data-stu-id="1859d-116">conversationThread</span></span>](conversationthread.md) |<span data-ttu-id="1859d-p102">最初にスレッドを作成して、新しい会話を開始します。グループには、新しい会話、会話スレッド、および投稿が作成されます。</span><span class="sxs-lookup"><span data-stu-id="1859d-p102">Start a new conversation by first creating a thread. A new conversation, conversation thread, and post are created in the group.</span></span>|
|[<span data-ttu-id="1859d-119">conversationThread を取得する</span><span class="sxs-lookup"><span data-stu-id="1859d-119">Get conversationThread</span></span>](../api/conversationthread-get.md) | [<span data-ttu-id="1859d-120">conversationThread</span><span class="sxs-lookup"><span data-stu-id="1859d-120">conversationThread</span></span>](conversationthread.md) |<span data-ttu-id="1859d-121">グループに属している特定のスレッドを取得します。</span><span class="sxs-lookup"><span data-stu-id="1859d-121">Get a specific thread that belongs to a group.</span></span> |
|[<span data-ttu-id="1859d-122">Update</span><span class="sxs-lookup"><span data-stu-id="1859d-122">Update</span></span>](../api/conversationthread-update.md) | [<span data-ttu-id="1859d-123">conversationThread</span><span class="sxs-lookup"><span data-stu-id="1859d-123">conversationThread</span></span>](conversationthread.md)  |<span data-ttu-id="1859d-124">conversationThread オブジェクトを更新します。</span><span class="sxs-lookup"><span data-stu-id="1859d-124">Update conversationThread object.</span></span> |
|[<span data-ttu-id="1859d-125">Delete</span><span class="sxs-lookup"><span data-stu-id="1859d-125">Delete</span></span>](../api/conversationthread-delete.md) | <span data-ttu-id="1859d-126">None</span><span class="sxs-lookup"><span data-stu-id="1859d-126">None</span></span> |<span data-ttu-id="1859d-127">conversationThread オブジェクトを削除します。</span><span class="sxs-lookup"><span data-stu-id="1859d-127">Delete conversationThread object.</span></span> |
|[<span data-ttu-id="1859d-128">Reply</span><span class="sxs-lookup"><span data-stu-id="1859d-128">Reply</span></span>](../api/conversationthread-reply.md)|<span data-ttu-id="1859d-129">なし</span><span class="sxs-lookup"><span data-stu-id="1859d-129">None</span></span>|<span data-ttu-id="1859d-130">新しい投稿のエンティティを作成して、このスレッドに返信します。</span><span class="sxs-lookup"><span data-stu-id="1859d-130">Reply to this thread by creating a new Post entity.</span></span>|
|[<span data-ttu-id="1859d-131">投稿を一覧表示する</span><span class="sxs-lookup"><span data-stu-id="1859d-131">List Posts</span></span>](../api/conversationthread-list-posts.md) |<span data-ttu-id="1859d-132">[post](post.md) collection</span><span class="sxs-lookup"><span data-stu-id="1859d-132">[post](post.md) collection</span></span>| <span data-ttu-id="1859d-133">指定したスレッドの投稿を取得します。</span><span class="sxs-lookup"><span data-stu-id="1859d-133">Get the posts of the specified thread.</span></span> |

## <a name="properties"></a><span data-ttu-id="1859d-134">プロパティ</span><span class="sxs-lookup"><span data-stu-id="1859d-134">Properties</span></span>
| <span data-ttu-id="1859d-135">プロパティ</span><span class="sxs-lookup"><span data-stu-id="1859d-135">Property</span></span>     | <span data-ttu-id="1859d-136">型</span><span class="sxs-lookup"><span data-stu-id="1859d-136">Type</span></span>   |<span data-ttu-id="1859d-137">説明</span><span class="sxs-lookup"><span data-stu-id="1859d-137">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="1859d-138">id</span><span class="sxs-lookup"><span data-stu-id="1859d-138">id</span></span>|<span data-ttu-id="1859d-139">String</span><span class="sxs-lookup"><span data-stu-id="1859d-139">String</span></span>| <span data-ttu-id="1859d-140">読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="1859d-140">Read-only.</span></span>|
|<span data-ttu-id="1859d-141">toRecipients</span><span class="sxs-lookup"><span data-stu-id="1859d-141">toRecipients</span></span>|<span data-ttu-id="1859d-142">[recipient](recipient.md) collection</span><span class="sxs-lookup"><span data-stu-id="1859d-142">[recipient](recipient.md) collection</span></span>|<span data-ttu-id="1859d-143">スレッドの宛先の受信者。</span><span class="sxs-lookup"><span data-stu-id="1859d-143">The To: recipients for the thread.</span></span>|
|<span data-ttu-id="1859d-144">ccRecipients</span><span class="sxs-lookup"><span data-stu-id="1859d-144">ccRecipients</span></span>|<span data-ttu-id="1859d-145">[recipient](recipient.md) collection</span><span class="sxs-lookup"><span data-stu-id="1859d-145">[recipient](recipient.md) collection</span></span>|<span data-ttu-id="1859d-146">スレッドの CC の受信者。</span><span class="sxs-lookup"><span data-stu-id="1859d-146">The Cc: recipients for the thread.</span></span>|
|<span data-ttu-id="1859d-147">topic</span><span class="sxs-lookup"><span data-stu-id="1859d-147">topic</span></span>|<span data-ttu-id="1859d-148">String</span><span class="sxs-lookup"><span data-stu-id="1859d-148">String</span></span>|<span data-ttu-id="1859d-p103">会話のトピックです。会話の作成時にこのプロパティを設定できますが、更新することはできません。</span><span class="sxs-lookup"><span data-stu-id="1859d-p103">The topic of the conversation. This property can be set when the conversation is created, but it cannot be updated.</span></span>||
|<span data-ttu-id="1859d-151">hasAttachments</span><span class="sxs-lookup"><span data-stu-id="1859d-151">hasAttachments</span></span>|<span data-ttu-id="1859d-152">Boolean</span><span class="sxs-lookup"><span data-stu-id="1859d-152">Boolean</span></span>|<span data-ttu-id="1859d-153">このスレッド内のいずれかの投稿に添付ファイルが 1 つ以上あるかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="1859d-153">Indicates whether any of the posts within this thread has at least one attachment.</span></span>|
|<span data-ttu-id="1859d-154">lastDeliveredDateTime</span><span class="sxs-lookup"><span data-stu-id="1859d-154">lastDeliveredDateTime</span></span>|<span data-ttu-id="1859d-155">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="1859d-155">DateTimeOffset</span></span>|<span data-ttu-id="1859d-p104">Timestamp 型は、ISO 8601 形式を使用して日付と時刻の情報を表し、必ず UTC 時間です。たとえば、2014 年 1 月 1 日午前 0 時 (UTC) は、次のようになります。`'2014-01-01T00:00:00Z'`</span><span class="sxs-lookup"><span data-stu-id="1859d-p104">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time. For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|
|<span data-ttu-id="1859d-158">uniqueSenders</span><span class="sxs-lookup"><span data-stu-id="1859d-158">uniqueSenders</span></span>|<span data-ttu-id="1859d-159">String collection</span><span class="sxs-lookup"><span data-stu-id="1859d-159">String collection</span></span>|<span data-ttu-id="1859d-160">このスレッドにメッセージを送信したすべてのユーザー。</span><span class="sxs-lookup"><span data-stu-id="1859d-160">All the users that sent a message to this thread.</span></span>|
|<span data-ttu-id="1859d-161">preview</span><span class="sxs-lookup"><span data-stu-id="1859d-161">preview</span></span>|<span data-ttu-id="1859d-162">String</span><span class="sxs-lookup"><span data-stu-id="1859d-162">String</span></span>|<span data-ttu-id="1859d-163">この会話における最新投稿の本文からの短い概要。</span><span class="sxs-lookup"><span data-stu-id="1859d-163">A short summary from the body of the latest post in this converstaion.</span></span>|
|<span data-ttu-id="1859d-164">Resource.islocked</span><span class="sxs-lookup"><span data-stu-id="1859d-164">isLocked</span></span>|<span data-ttu-id="1859d-165">ブール値</span><span class="sxs-lookup"><span data-stu-id="1859d-165">Boolean</span></span>|<span data-ttu-id="1859d-166">スレッドがロックされているかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="1859d-166">Indicates if the thread is locked.</span></span>|

## <a name="relationships"></a><span data-ttu-id="1859d-167">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="1859d-167">Relationships</span></span>
| <span data-ttu-id="1859d-168">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="1859d-168">Relationship</span></span> | <span data-ttu-id="1859d-169">型</span><span class="sxs-lookup"><span data-stu-id="1859d-169">Type</span></span>   |<span data-ttu-id="1859d-170">説明</span><span class="sxs-lookup"><span data-stu-id="1859d-170">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="1859d-171">投稿</span><span class="sxs-lookup"><span data-stu-id="1859d-171">posts</span></span>|<span data-ttu-id="1859d-172">[post](post.md) collection</span><span class="sxs-lookup"><span data-stu-id="1859d-172">[post](post.md) collection</span></span>| <span data-ttu-id="1859d-p105">読み取り専用。Null 許容型です。</span><span class="sxs-lookup"><span data-stu-id="1859d-p105">Read-only. Nullable.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="1859d-175">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="1859d-175">JSON representation</span></span>

<span data-ttu-id="1859d-176">以下は、リソースの JSON 表記です</span><span class="sxs-lookup"><span data-stu-id="1859d-176">Here is a JSON representation of the resource</span></span>

<!--{
  "blockType": "resource",
  "optionalProperties": [
    "posts"
  ],
  "keyProperty": "id",
  "baseType": "microsoft.graph.entity",
  "@odata.type": "microsoft.graph.conversationThread",
  "@odata.annotations": [
    {
      "property": "posts",
      "capabilities": {
        "changeTracking": false,
        "deletable": false,
        "insertable": false,
        "searchable": false,
        "updatable": false
      }
    }
  ]
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
