---
title: conversationThread リソースの種類
description: onversationThread は、投稿のコレクションです。
author: dkershaw10
localization_priority: Normal
ms.prod: groups
ms.openlocfilehash: a1a45f5ac6d26b58f1179616d3a6b9b76c6c1618
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32549889"
---
# <a name="conversationthread-resource-type"></a><span data-ttu-id="6d7e5-103">conversationThread リソースの種類</span><span class="sxs-lookup"><span data-stu-id="6d7e5-103">conversationThread resource type</span></span>
<span data-ttu-id="6d7e5-104">onversationThread は、[投稿](post.md)のコレクションです。</span><span class="sxs-lookup"><span data-stu-id="6d7e5-104">A conversationThread is a collection of [posts](post.md).</span></span>

<span data-ttu-id="6d7e5-p101">最後の投稿の受信者コレクションはスレッド全体の集計された受信者です。スレッドの受信者コレクションは増大する可能性があります。スレッドから受信者が削除されると、新しいスレッドが作成されます。</span><span class="sxs-lookup"><span data-stu-id="6d7e5-p101">The last post's recipients collection is the aggregated recipients of the entire thread. A thread can have a growing collection of recipients. A new thread is created when a recipient is removed from the thread.</span></span>

## <a name="methods"></a><span data-ttu-id="6d7e5-108">メソッド</span><span class="sxs-lookup"><span data-stu-id="6d7e5-108">Methods</span></span>

| <span data-ttu-id="6d7e5-109">メソッド</span><span class="sxs-lookup"><span data-stu-id="6d7e5-109">Method</span></span>       | <span data-ttu-id="6d7e5-110">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="6d7e5-110">Return Type</span></span>  |<span data-ttu-id="6d7e5-111">説明</span><span class="sxs-lookup"><span data-stu-id="6d7e5-111">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="6d7e5-112">スレッドを一覧表示する</span><span class="sxs-lookup"><span data-stu-id="6d7e5-112">List threads</span></span>](../api/group-list-threads.md) | <span data-ttu-id="6d7e5-113">[conversationThread](conversationthread.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="6d7e5-113">[conversationThread](conversationthread.md) collection</span></span> |<span data-ttu-id="6d7e5-114">グループのすべてのスレッドを取得します。</span><span class="sxs-lookup"><span data-stu-id="6d7e5-114">Get all the threads of a group.</span></span>|
|[<span data-ttu-id="6d7e5-115">スレッドを作成する</span><span class="sxs-lookup"><span data-stu-id="6d7e5-115">Create thread</span></span>](../api/group-post-threads.md) | [<span data-ttu-id="6d7e5-116">conversationThread</span><span class="sxs-lookup"><span data-stu-id="6d7e5-116">conversationThread</span></span>](conversationthread.md) |<span data-ttu-id="6d7e5-p102">最初にスレッドを作成して、新しい会話を開始します。グループには、新しい会話、会話スレッド、および投稿が作成されます。</span><span class="sxs-lookup"><span data-stu-id="6d7e5-p102">Start a new conversation by first creating a thread. A new conversation, conversation thread, and post are created in the group.</span></span>|
|[<span data-ttu-id="6d7e5-119">conversationThread を取得する</span><span class="sxs-lookup"><span data-stu-id="6d7e5-119">Get conversationThread</span></span>](../api/conversationthread-get.md) | [<span data-ttu-id="6d7e5-120">conversationThread</span><span class="sxs-lookup"><span data-stu-id="6d7e5-120">conversationThread</span></span>](conversationthread.md) |<span data-ttu-id="6d7e5-121">グループに属している特定のスレッドを取得します。</span><span class="sxs-lookup"><span data-stu-id="6d7e5-121">Get a specific thread that belongs to a group.</span></span> |
|[<span data-ttu-id="6d7e5-122">Update</span><span class="sxs-lookup"><span data-stu-id="6d7e5-122">Update</span></span>](../api/conversationthread-update.md) | [<span data-ttu-id="6d7e5-123">conversationThread</span><span class="sxs-lookup"><span data-stu-id="6d7e5-123">conversationThread</span></span>](conversationthread.md)  |<span data-ttu-id="6d7e5-124">conversationThread オブジェクトを更新します。</span><span class="sxs-lookup"><span data-stu-id="6d7e5-124">Update conversationThread object.</span></span> |
|[<span data-ttu-id="6d7e5-125">削除</span><span class="sxs-lookup"><span data-stu-id="6d7e5-125">Delete</span></span>](../api/conversationthread-delete.md) | <span data-ttu-id="6d7e5-126">なし</span><span class="sxs-lookup"><span data-stu-id="6d7e5-126">None</span></span> |<span data-ttu-id="6d7e5-127">conversationThread オブジェクトを削除します。</span><span class="sxs-lookup"><span data-stu-id="6d7e5-127">Delete conversationThread object.</span></span> |
|[<span data-ttu-id="6d7e5-128">Reply</span><span class="sxs-lookup"><span data-stu-id="6d7e5-128">Reply</span></span>](../api/conversationthread-reply.md)|<span data-ttu-id="6d7e5-129">なし</span><span class="sxs-lookup"><span data-stu-id="6d7e5-129">None</span></span>|<span data-ttu-id="6d7e5-130">新しい投稿のエンティティを作成して、このスレッドに返信します。</span><span class="sxs-lookup"><span data-stu-id="6d7e5-130">Reply to this thread by creating a new Post entity.</span></span>|
|[<span data-ttu-id="6d7e5-131">投稿を一覧表示する</span><span class="sxs-lookup"><span data-stu-id="6d7e5-131">List Posts</span></span>](../api/conversationthread-list-posts.md) |<span data-ttu-id="6d7e5-132">[post](post.md) collection</span><span class="sxs-lookup"><span data-stu-id="6d7e5-132">[post](post.md) collection</span></span>| <span data-ttu-id="6d7e5-133">指定したスレッドの投稿を取得します。</span><span class="sxs-lookup"><span data-stu-id="6d7e5-133">Get the posts of the specified thread.</span></span> |

## <a name="properties"></a><span data-ttu-id="6d7e5-134">プロパティ</span><span class="sxs-lookup"><span data-stu-id="6d7e5-134">Properties</span></span>
| <span data-ttu-id="6d7e5-135">プロパティ</span><span class="sxs-lookup"><span data-stu-id="6d7e5-135">Property</span></span>     | <span data-ttu-id="6d7e5-136">型</span><span class="sxs-lookup"><span data-stu-id="6d7e5-136">Type</span></span>   |<span data-ttu-id="6d7e5-137">説明</span><span class="sxs-lookup"><span data-stu-id="6d7e5-137">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="6d7e5-138">id</span><span class="sxs-lookup"><span data-stu-id="6d7e5-138">id</span></span>|<span data-ttu-id="6d7e5-139">String</span><span class="sxs-lookup"><span data-stu-id="6d7e5-139">String</span></span>| <span data-ttu-id="6d7e5-140">読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="6d7e5-140">Read-only.</span></span>|
|<span data-ttu-id="6d7e5-141">toRecipients</span><span class="sxs-lookup"><span data-stu-id="6d7e5-141">toRecipients</span></span>|<span data-ttu-id="6d7e5-142">[recipient](recipient.md) collection</span><span class="sxs-lookup"><span data-stu-id="6d7e5-142">[recipient](recipient.md) collection</span></span>|<span data-ttu-id="6d7e5-143">スレッドの宛先の受信者。</span><span class="sxs-lookup"><span data-stu-id="6d7e5-143">The To: recipients for the thread.</span></span>|
|<span data-ttu-id="6d7e5-144">ccRecipients</span><span class="sxs-lookup"><span data-stu-id="6d7e5-144">ccRecipients</span></span>|<span data-ttu-id="6d7e5-145">[recipient](recipient.md) collection</span><span class="sxs-lookup"><span data-stu-id="6d7e5-145">[recipient](recipient.md) collection</span></span>|<span data-ttu-id="6d7e5-146">スレッドの CC の受信者。</span><span class="sxs-lookup"><span data-stu-id="6d7e5-146">The Cc: recipients for the thread.</span></span>|
|<span data-ttu-id="6d7e5-147">topic</span><span class="sxs-lookup"><span data-stu-id="6d7e5-147">topic</span></span>|<span data-ttu-id="6d7e5-148">String</span><span class="sxs-lookup"><span data-stu-id="6d7e5-148">String</span></span>|<span data-ttu-id="6d7e5-p103">会話のトピックです。会話の作成時にこのプロパティを設定できますが、更新することはできません。</span><span class="sxs-lookup"><span data-stu-id="6d7e5-p103">The topic of the conversation. This property can be set when the conversation is created, but it cannot be updated.</span></span>||
|<span data-ttu-id="6d7e5-151">hasAttachments</span><span class="sxs-lookup"><span data-stu-id="6d7e5-151">hasAttachments</span></span>|<span data-ttu-id="6d7e5-152">ブール値</span><span class="sxs-lookup"><span data-stu-id="6d7e5-152">Boolean</span></span>|<span data-ttu-id="6d7e5-153">このスレッド内のいずれかの投稿に添付ファイルが 1 つ以上あるかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="6d7e5-153">Indicates whether any of the posts within this thread has at least one attachment.</span></span>|
|<span data-ttu-id="6d7e5-154">lastDeliveredDateTime</span><span class="sxs-lookup"><span data-stu-id="6d7e5-154">lastDeliveredDateTime</span></span>|<span data-ttu-id="6d7e5-155">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="6d7e5-155">DateTimeOffset</span></span>|<span data-ttu-id="6d7e5-p104">Timestamp 型は、ISO 8601 形式を使用して日付と時刻の情報を表し、必ず UTC 時間です。たとえば、2014 年 1 月 1 日午前 0 時 (UTC) は、次のようになります。`'2014-01-01T00:00:00Z'`</span><span class="sxs-lookup"><span data-stu-id="6d7e5-p104">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time. For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|
|<span data-ttu-id="6d7e5-158">uniqueSenders</span><span class="sxs-lookup"><span data-stu-id="6d7e5-158">uniqueSenders</span></span>|<span data-ttu-id="6d7e5-159">String collection</span><span class="sxs-lookup"><span data-stu-id="6d7e5-159">String collection</span></span>|<span data-ttu-id="6d7e5-160">このスレッドにメッセージを送信したすべてのユーザー。</span><span class="sxs-lookup"><span data-stu-id="6d7e5-160">All the users that sent a message to this thread.</span></span>|
|<span data-ttu-id="6d7e5-161">preview</span><span class="sxs-lookup"><span data-stu-id="6d7e5-161">preview</span></span>|<span data-ttu-id="6d7e5-162">String</span><span class="sxs-lookup"><span data-stu-id="6d7e5-162">String</span></span>|<span data-ttu-id="6d7e5-163">この会話における最新投稿の本文からの短い概要。</span><span class="sxs-lookup"><span data-stu-id="6d7e5-163">A short summary from the body of the latest post in this converstaion.</span></span>|
|<span data-ttu-id="6d7e5-164">resource.islocked</span><span class="sxs-lookup"><span data-stu-id="6d7e5-164">isLocked</span></span>|<span data-ttu-id="6d7e5-165">ブール値</span><span class="sxs-lookup"><span data-stu-id="6d7e5-165">Boolean</span></span>|<span data-ttu-id="6d7e5-166">スレッドがロックされているかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="6d7e5-166">Indicates if the thread is locked.</span></span>|

## <a name="relationships"></a><span data-ttu-id="6d7e5-167">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="6d7e5-167">Relationships</span></span>
| <span data-ttu-id="6d7e5-168">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="6d7e5-168">Relationship</span></span> | <span data-ttu-id="6d7e5-169">型</span><span class="sxs-lookup"><span data-stu-id="6d7e5-169">Type</span></span>   |<span data-ttu-id="6d7e5-170">説明</span><span class="sxs-lookup"><span data-stu-id="6d7e5-170">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="6d7e5-171">投稿</span><span class="sxs-lookup"><span data-stu-id="6d7e5-171">posts</span></span>|<span data-ttu-id="6d7e5-172">[post](post.md) collection</span><span class="sxs-lookup"><span data-stu-id="6d7e5-172">[post](post.md) collection</span></span>| <span data-ttu-id="6d7e5-p105">読み取り専用です。Null 許容型。</span><span class="sxs-lookup"><span data-stu-id="6d7e5-p105">Read-only. Nullable.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="6d7e5-175">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="6d7e5-175">JSON representation</span></span>

<span data-ttu-id="6d7e5-176">以下は、リソースの JSON 表記です</span><span class="sxs-lookup"><span data-stu-id="6d7e5-176">Here is a JSON representation of the resource</span></span>

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
