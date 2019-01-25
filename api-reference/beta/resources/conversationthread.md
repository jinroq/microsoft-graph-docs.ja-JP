---
title: conversationThread リソースの種類
description: onversationThread は、投稿のコレクションです。
author: dkershaw10
localization_priority: Normal
ms.prod: groups
ms.openlocfilehash: 504b8b8d4e47f892da72ea7ef9588491d0642f21
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/24/2019
ms.locfileid: "29508175"
---
# <a name="conversationthread-resource-type"></a><span data-ttu-id="420f3-103">conversationThread リソースの種類</span><span class="sxs-lookup"><span data-stu-id="420f3-103">conversationThread resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="420f3-104">onversationThread は、[投稿](post.md)のコレクションです。</span><span class="sxs-lookup"><span data-stu-id="420f3-104">A conversationThread is a collection of [posts](post.md).</span></span>

<span data-ttu-id="420f3-p101">最後の投稿の受信者コレクションはスレッド全体の集計された受信者です。スレッドの受信者コレクションは増大する可能性があります。スレッドから受信者が削除されると、新しいスレッドが作成されます。</span><span class="sxs-lookup"><span data-stu-id="420f3-p101">The last post's recipients collection is the aggregated recipients of the entire thread. A thread can have a growing collection of recipients. A new thread is created when a recipient is removed from the thread.</span></span>

## <a name="methods"></a><span data-ttu-id="420f3-108">メソッド</span><span class="sxs-lookup"><span data-stu-id="420f3-108">Methods</span></span>

| <span data-ttu-id="420f3-109">メソッド</span><span class="sxs-lookup"><span data-stu-id="420f3-109">Method</span></span>       | <span data-ttu-id="420f3-110">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="420f3-110">Return Type</span></span>  |<span data-ttu-id="420f3-111">説明</span><span class="sxs-lookup"><span data-stu-id="420f3-111">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="420f3-112">スレッドを一覧表示する</span><span class="sxs-lookup"><span data-stu-id="420f3-112">List threads</span></span>](../api/group-list-threads.md) | <span data-ttu-id="420f3-113">[conversationThread](conversationthread.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="420f3-113">[conversationThread](conversationthread.md) collection</span></span> |<span data-ttu-id="420f3-114">グループのすべてのスレッドを取得します。</span><span class="sxs-lookup"><span data-stu-id="420f3-114">Get all the threads of a group.</span></span>|
|[<span data-ttu-id="420f3-115">スレッドを作成する</span><span class="sxs-lookup"><span data-stu-id="420f3-115">Create thread</span></span>](../api/group-post-threads.md) | [<span data-ttu-id="420f3-116">conversationThread</span><span class="sxs-lookup"><span data-stu-id="420f3-116">conversationThread</span></span>](conversationthread.md) |<span data-ttu-id="420f3-p102">最初にスレッドを作成して、新しい会話を開始します。グループには、新しい会話、会話スレッド、および投稿が作成されます。</span><span class="sxs-lookup"><span data-stu-id="420f3-p102">Start a new conversation by first creating a thread. A new conversation, conversation thread, and post are created in the group.</span></span>|
|[<span data-ttu-id="420f3-119">conversationThread を取得する</span><span class="sxs-lookup"><span data-stu-id="420f3-119">Get conversationThread</span></span>](../api/conversationthread-get.md) | [<span data-ttu-id="420f3-120">conversationThread</span><span class="sxs-lookup"><span data-stu-id="420f3-120">conversationThread</span></span>](conversationthread.md) |<span data-ttu-id="420f3-121">グループに属している特定のスレッドを取得します。</span><span class="sxs-lookup"><span data-stu-id="420f3-121">Get a specific thread that belongs to a group.</span></span> |
|[<span data-ttu-id="420f3-122">Update</span><span class="sxs-lookup"><span data-stu-id="420f3-122">Update</span></span>](../api/conversationthread-update.md) | [<span data-ttu-id="420f3-123">conversationThread</span><span class="sxs-lookup"><span data-stu-id="420f3-123">conversationThread</span></span>](conversationthread.md)  |<span data-ttu-id="420f3-124">conversationThread オブジェクトを更新します。</span><span class="sxs-lookup"><span data-stu-id="420f3-124">Update conversationThread object.</span></span> |
|[<span data-ttu-id="420f3-125">Delete</span><span class="sxs-lookup"><span data-stu-id="420f3-125">Delete</span></span>](../api/conversationthread-delete.md) | <span data-ttu-id="420f3-126">None</span><span class="sxs-lookup"><span data-stu-id="420f3-126">None</span></span> |<span data-ttu-id="420f3-127">conversationThread オブジェクトを削除します。</span><span class="sxs-lookup"><span data-stu-id="420f3-127">Delete conversationThread object.</span></span> |
|[<span data-ttu-id="420f3-128">返信</span><span class="sxs-lookup"><span data-stu-id="420f3-128">reply</span></span>](../api/conversationthread-reply.md)|<span data-ttu-id="420f3-129">なし</span><span class="sxs-lookup"><span data-stu-id="420f3-129">None</span></span>|<span data-ttu-id="420f3-130">新しい投稿のエンティティを作成して、このスレッドに返信します。</span><span class="sxs-lookup"><span data-stu-id="420f3-130">Reply to this thread by creating a new Post entity.</span></span>|
|[<span data-ttu-id="420f3-131">投稿を一覧表示する</span><span class="sxs-lookup"><span data-stu-id="420f3-131">List Posts</span></span>](../api/conversationthread-list-posts.md) |<span data-ttu-id="420f3-132">[post](post.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="420f3-132">[post](post.md) collection</span></span>| <span data-ttu-id="420f3-133">指定したスレッドの投稿を取得します。</span><span class="sxs-lookup"><span data-stu-id="420f3-133">Get the posts of the specified thread.</span></span> |

## <a name="properties"></a><span data-ttu-id="420f3-134">プロパティ</span><span class="sxs-lookup"><span data-stu-id="420f3-134">Properties</span></span>
| <span data-ttu-id="420f3-135">プロパティ</span><span class="sxs-lookup"><span data-stu-id="420f3-135">Property</span></span>     | <span data-ttu-id="420f3-136">型</span><span class="sxs-lookup"><span data-stu-id="420f3-136">Type</span></span>   |<span data-ttu-id="420f3-137">説明</span><span class="sxs-lookup"><span data-stu-id="420f3-137">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="420f3-138">id</span><span class="sxs-lookup"><span data-stu-id="420f3-138">id</span></span>|<span data-ttu-id="420f3-139">String</span><span class="sxs-lookup"><span data-stu-id="420f3-139">String</span></span>| <span data-ttu-id="420f3-140">読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="420f3-140">Read-only.</span></span>|
|<span data-ttu-id="420f3-141">toRecipients</span><span class="sxs-lookup"><span data-stu-id="420f3-141">toRecipients</span></span>|<span data-ttu-id="420f3-142">[recipient](recipient.md) collection</span><span class="sxs-lookup"><span data-stu-id="420f3-142">[recipient](recipient.md) collection</span></span>|<span data-ttu-id="420f3-143">スレッドの宛先の受信者。</span><span class="sxs-lookup"><span data-stu-id="420f3-143">The To: recipients for the thread.</span></span>|
|<span data-ttu-id="420f3-144">ccRecipients</span><span class="sxs-lookup"><span data-stu-id="420f3-144">ccRecipients</span></span>|<span data-ttu-id="420f3-145">[recipient](recipient.md) collection</span><span class="sxs-lookup"><span data-stu-id="420f3-145">[recipient](recipient.md) collection</span></span>|<span data-ttu-id="420f3-146">スレッドの CC の受信者。</span><span class="sxs-lookup"><span data-stu-id="420f3-146">The Cc: recipients for the thread.</span></span>|
|<span data-ttu-id="420f3-147">topic</span><span class="sxs-lookup"><span data-stu-id="420f3-147">topic</span></span>|<span data-ttu-id="420f3-148">String</span><span class="sxs-lookup"><span data-stu-id="420f3-148">String</span></span>|<span data-ttu-id="420f3-p103">会話のトピックです。会話の作成時にこのプロパティを設定できますが、更新することはできません。</span><span class="sxs-lookup"><span data-stu-id="420f3-p103">The topic of the conversation. This property can be set when the conversation is created, but it cannot be updated.</span></span>||
|<span data-ttu-id="420f3-151">hasAttachments</span><span class="sxs-lookup"><span data-stu-id="420f3-151">hasAttachments</span></span>|<span data-ttu-id="420f3-152">ブール値</span><span class="sxs-lookup"><span data-stu-id="420f3-152">Boolean</span></span>|<span data-ttu-id="420f3-153">このスレッド内のいずれかの投稿に添付ファイルが 1 つ以上あるかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="420f3-153">Indicates whether any of the posts within this thread has at least one attachment.</span></span>|
|<span data-ttu-id="420f3-154">lastDeliveredDateTime</span><span class="sxs-lookup"><span data-stu-id="420f3-154">lastDeliveredDateTime</span></span>|<span data-ttu-id="420f3-155">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="420f3-155">DateTimeOffset</span></span>|<span data-ttu-id="420f3-p104">Timestamp 型は、ISO 8601 形式を使用して日付と時刻の情報を表し、必ず UTC 時間です。たとえば、2014 年 1 月 1 日午前 0 時 (UTC) は、次のようになります。`'2014-01-01T00:00:00Z'`</span><span class="sxs-lookup"><span data-stu-id="420f3-p104">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time. For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|
|<span data-ttu-id="420f3-158">uniqueSenders</span><span class="sxs-lookup"><span data-stu-id="420f3-158">uniqueSenders</span></span>|<span data-ttu-id="420f3-159">String コレクション</span><span class="sxs-lookup"><span data-stu-id="420f3-159">String collection</span></span>|<span data-ttu-id="420f3-160">このスレッドにメッセージを送信したすべてのユーザー。</span><span class="sxs-lookup"><span data-stu-id="420f3-160">All the users that sent a message to this thread.</span></span>|
|<span data-ttu-id="420f3-161">preview</span><span class="sxs-lookup"><span data-stu-id="420f3-161">preview</span></span>|<span data-ttu-id="420f3-162">String</span><span class="sxs-lookup"><span data-stu-id="420f3-162">String</span></span>|<span data-ttu-id="420f3-163">この会話における最新投稿の本文からの短い概要。</span><span class="sxs-lookup"><span data-stu-id="420f3-163">A short summary from the body of the latest post in this converstaion.</span></span>|
|<span data-ttu-id="420f3-164">isLocked</span><span class="sxs-lookup"><span data-stu-id="420f3-164">isLocked</span></span>|<span data-ttu-id="420f3-165">Boolean</span><span class="sxs-lookup"><span data-stu-id="420f3-165">Boolean</span></span>|<span data-ttu-id="420f3-166">スレッドがロックされているかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="420f3-166">Indicates if the thread is locked.</span></span>|

## <a name="relationships"></a><span data-ttu-id="420f3-167">関係</span><span class="sxs-lookup"><span data-stu-id="420f3-167">Relationships</span></span>
| <span data-ttu-id="420f3-168">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="420f3-168">Relationship</span></span> | <span data-ttu-id="420f3-169">型</span><span class="sxs-lookup"><span data-stu-id="420f3-169">Type</span></span>   |<span data-ttu-id="420f3-170">説明</span><span class="sxs-lookup"><span data-stu-id="420f3-170">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="420f3-171">投稿</span><span class="sxs-lookup"><span data-stu-id="420f3-171">posts</span></span>|<span data-ttu-id="420f3-172">[post](post.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="420f3-172">[post](post.md) collection</span></span>| <span data-ttu-id="420f3-p105">読み取り専用です。Null 許容型。</span><span class="sxs-lookup"><span data-stu-id="420f3-p105">Read-only. Nullable.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="420f3-175">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="420f3-175">JSON representation</span></span>

<span data-ttu-id="420f3-176">以下は、リソースの JSON 表記です</span><span class="sxs-lookup"><span data-stu-id="420f3-176">Here is a JSON representation of the resource</span></span>

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
<!--
{
  "type": "#page.annotation",
  "description": "conversationThread resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/conversationthread.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
