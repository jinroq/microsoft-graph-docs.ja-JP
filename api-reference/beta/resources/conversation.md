---
title: 会話リソースの種類
description: 会話はスレッドのコレクションです。スレッドにはそのスレッドへの投稿が含まれています。会話のすべてのスレッドと投稿は同じ件名を共有します。
localization_priority: Normal
author: dkershaw10
ms.prod: groups
ms.openlocfilehash: 5cacad2b9539c398251ffd07899df7beb3c2f378
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/12/2019
ms.locfileid: "27991441"
---
# <a name="conversation-resource-type"></a><span data-ttu-id="990ed-104">会話リソースの種類</span><span class="sxs-lookup"><span data-stu-id="990ed-104">conversation resource type</span></span>

> <span data-ttu-id="990ed-105">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="990ed-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="990ed-106">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="990ed-106">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="990ed-p103">会話は[スレッド](conversationthread.md)のコレクションです。スレッドにはそのスレッドへの投稿が含まれています。会話のすべてのスレッドと投稿は同じ件名を共有します。</span><span class="sxs-lookup"><span data-stu-id="990ed-p103">A conversation is a collection of [threads](conversationthread.md), and a thread contains posts to that thread. All threads and posts in a conversation share the same subject.</span></span>

<span data-ttu-id="990ed-109">このリソースは、[変更通知](/graph/webhooks)をサブスクライブするをサポートします。</span><span class="sxs-lookup"><span data-stu-id="990ed-109">This resource supports subscribing to [change notifications](/graph/webhooks).</span></span>

## <a name="methods"></a><span data-ttu-id="990ed-110">メソッド</span><span class="sxs-lookup"><span data-stu-id="990ed-110">Methods</span></span>

| <span data-ttu-id="990ed-111">メソッド</span><span class="sxs-lookup"><span data-stu-id="990ed-111">Method</span></span>       | <span data-ttu-id="990ed-112">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="990ed-112">Return Type</span></span>  |<span data-ttu-id="990ed-113">説明</span><span class="sxs-lookup"><span data-stu-id="990ed-113">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="990ed-114">会話を一覧表示する</span><span class="sxs-lookup"><span data-stu-id="990ed-114">List conversations</span></span>](../api/group-list-conversations.md) | <span data-ttu-id="990ed-115">[conversation](conversation.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="990ed-115">[conversation](conversation.md) collection</span></span> |<span data-ttu-id="990ed-116">このグループの会話の一覧を取得します。</span><span class="sxs-lookup"><span data-stu-id="990ed-116">Get the list of conversations in this group.</span></span>|
|[<span data-ttu-id="990ed-117">Create</span><span class="sxs-lookup"><span data-stu-id="990ed-117">Create</span></span>](../api/group-post-conversations.md) |[<span data-ttu-id="990ed-118">conversation</span><span class="sxs-lookup"><span data-stu-id="990ed-118">conversation</span></span>](conversation.md)| <span data-ttu-id="990ed-119">スレッドと投稿を含めて、新しい会話を作成します。</span><span class="sxs-lookup"><span data-stu-id="990ed-119">Create a new conversation by including a thread and a post.</span></span>|
|[<span data-ttu-id="990ed-120">会話を取得する</span><span class="sxs-lookup"><span data-stu-id="990ed-120">Get conversation</span></span>](../api/conversation-get.md) | [<span data-ttu-id="990ed-121">conversation</span><span class="sxs-lookup"><span data-stu-id="990ed-121">conversation</span></span>](conversation.md) |<span data-ttu-id="990ed-122">会話オブジェクトのプロパティと関係を読み取ります。</span><span class="sxs-lookup"><span data-stu-id="990ed-122">Read properties and relationships of conversation object.</span></span>|
|[<span data-ttu-id="990ed-123">Delete</span><span class="sxs-lookup"><span data-stu-id="990ed-123">Delete</span></span>](../api/conversation-delete.md) | <span data-ttu-id="990ed-124">なし</span><span class="sxs-lookup"><span data-stu-id="990ed-124">None</span></span> |<span data-ttu-id="990ed-125">会話オブジェクトを削除します。</span><span class="sxs-lookup"><span data-stu-id="990ed-125">Delete conversation object.</span></span> |
|[<span data-ttu-id="990ed-126">会話スレッドを一覧表示する</span><span class="sxs-lookup"><span data-stu-id="990ed-126">List conversation threads</span></span>](../api/conversation-list-threads.md) |<span data-ttu-id="990ed-127">[conversationThread](conversationthread.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="990ed-127">[conversationThread](conversationthread.md) collection</span></span>| <span data-ttu-id="990ed-128">グループの会話のすべてのスレッドを取得します。</span><span class="sxs-lookup"><span data-stu-id="990ed-128">Get all the threads in a group conversation.</span></span>|
|[<span data-ttu-id="990ed-129">会話スレッドを作成する</span><span class="sxs-lookup"><span data-stu-id="990ed-129">Create conversation thread</span></span>](../api/conversation-post-threads.md) |<span data-ttu-id="990ed-130">[conversationThread](conversationthread.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="990ed-130">[conversationThread](conversationthread.md) collection</span></span>| <span data-ttu-id="990ed-131">指定した会話にスレッドを作成します。</span><span class="sxs-lookup"><span data-stu-id="990ed-131">Create a thread in the specified conversation.</span></span>|

## <a name="properties"></a><span data-ttu-id="990ed-132">プロパティ</span><span class="sxs-lookup"><span data-stu-id="990ed-132">Properties</span></span>
| <span data-ttu-id="990ed-133">プロパティ</span><span class="sxs-lookup"><span data-stu-id="990ed-133">Property</span></span>     | <span data-ttu-id="990ed-134">型</span><span class="sxs-lookup"><span data-stu-id="990ed-134">Type</span></span>   |<span data-ttu-id="990ed-135">説明</span><span class="sxs-lookup"><span data-stu-id="990ed-135">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="990ed-136">hasAttachments</span><span class="sxs-lookup"><span data-stu-id="990ed-136">hasAttachments</span></span>|<span data-ttu-id="990ed-137">Boolean</span><span class="sxs-lookup"><span data-stu-id="990ed-137">Boolean</span></span>|<span data-ttu-id="990ed-138">この会話内のいずれかの投稿に添付ファイルが 1 つ以上あるかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="990ed-138">Indicates whether any of the posts within this Conversation has at least one attachment.</span></span>|
|<span data-ttu-id="990ed-139">id</span><span class="sxs-lookup"><span data-stu-id="990ed-139">id</span></span>|<span data-ttu-id="990ed-140">String</span><span class="sxs-lookup"><span data-stu-id="990ed-140">String</span></span>|<span data-ttu-id="990ed-p104">会話の一意識別子。読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="990ed-p104">The conversations's unique identifier. Read-only.</span></span>|
|<span data-ttu-id="990ed-143">lastDeliveredDateTime</span><span class="sxs-lookup"><span data-stu-id="990ed-143">lastDeliveredDateTime</span></span>|<span data-ttu-id="990ed-144">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="990ed-144">DateTimeOffset</span></span>|<span data-ttu-id="990ed-p105">Timestamp 型は、ISO 8601 形式を使用して日付と時刻の情報を表し、必ず UTC 時間です。たとえば、2014 年 1 月 1 日午前 0 時 (UTC) は、次のようになります。`'2014-01-01T00:00:00Z'`</span><span class="sxs-lookup"><span data-stu-id="990ed-p105">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time. For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|
|<span data-ttu-id="990ed-147">preview</span><span class="sxs-lookup"><span data-stu-id="990ed-147">preview</span></span>|<span data-ttu-id="990ed-148">String</span><span class="sxs-lookup"><span data-stu-id="990ed-148">String</span></span>|<span data-ttu-id="990ed-149">この会話における最新投稿の本文からの短い概要。</span><span class="sxs-lookup"><span data-stu-id="990ed-149">A short summary from the body of the latest post in this converstaion.</span></span>|
|<span data-ttu-id="990ed-150">topic</span><span class="sxs-lookup"><span data-stu-id="990ed-150">topic</span></span>|<span data-ttu-id="990ed-151">String</span><span class="sxs-lookup"><span data-stu-id="990ed-151">String</span></span>|<span data-ttu-id="990ed-p106">会話のトピックです。会話の作成時にこのプロパティを設定できますが、更新することはできません。</span><span class="sxs-lookup"><span data-stu-id="990ed-p106">The topic of the conversation. This property can be set when the conversation is created, but it cannot be updated.</span></span>|
|<span data-ttu-id="990ed-154">uniqueSenders</span><span class="sxs-lookup"><span data-stu-id="990ed-154">uniqueSenders</span></span>|<span data-ttu-id="990ed-155">String コレクション</span><span class="sxs-lookup"><span data-stu-id="990ed-155">String collection</span></span>|<span data-ttu-id="990ed-156">この会話にメッセージを送信したすべてのユーザーです。</span><span class="sxs-lookup"><span data-stu-id="990ed-156">All the users that sent a message to this Conversation.</span></span>|

## <a name="relationships"></a><span data-ttu-id="990ed-157">関係</span><span class="sxs-lookup"><span data-stu-id="990ed-157">Relationships</span></span>
| <span data-ttu-id="990ed-158">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="990ed-158">Relationship</span></span> | <span data-ttu-id="990ed-159">型</span><span class="sxs-lookup"><span data-stu-id="990ed-159">Type</span></span>   |<span data-ttu-id="990ed-160">説明</span><span class="sxs-lookup"><span data-stu-id="990ed-160">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="990ed-161">スレッド</span><span class="sxs-lookup"><span data-stu-id="990ed-161">threads</span></span>|<span data-ttu-id="990ed-162">[conversationThread](conversationthread.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="990ed-162">[conversationThread](conversationthread.md) collection</span></span>|<span data-ttu-id="990ed-p107">会話内のすべての会話スレッドのコレクションです。ナビゲーションのプロパティです。読み取り専用です。Null 許容型。</span><span class="sxs-lookup"><span data-stu-id="990ed-p107">A collection of all the conversation threads in the conversation. A navigation property. Read-only. Nullable.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="990ed-167">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="990ed-167">JSON representation</span></span>

<span data-ttu-id="990ed-168">以下は、リソースの JSON 表記です</span><span class="sxs-lookup"><span data-stu-id="990ed-168">Here is a JSON representation of the resource</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [
    "threads"
  ],
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.conversation"
}-->

```json
{
  "hasAttachments": true,
  "id": "string (identifier)",
  "lastDeliveredDateTime": "String (timestamp)",
  "preview": "string",
  "topic": "string",
  "uniqueSenders": ["string"]
}

```


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "conversation resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
