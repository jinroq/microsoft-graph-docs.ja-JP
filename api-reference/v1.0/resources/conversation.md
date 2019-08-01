---
title: 会話リソースの種類
description: 会話はスレッドのコレクションであり、スレッドにはそのスレッドへの投稿が含まれています。 会話内のすべてのスレッドと投稿は同じ件名を共有します。
localization_priority: Normal
author: dkershaw10
ms.prod: groups
doc_type: resourcePageType
ms.openlocfilehash: 4c34f6f0d55cb27e5ce7f5f2ba6459cfbb4d5291
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "36029597"
---
# <a name="conversation-resource-type"></a><span data-ttu-id="1523d-104">会話リソースの種類</span><span class="sxs-lookup"><span data-stu-id="1523d-104">conversation resource type</span></span>

<span data-ttu-id="1523d-p102">会話は[スレッド](conversationthread.md)のコレクションです。スレッドにはそのスレッドへの投稿が含まれています。会話のすべてのスレッドと投稿は同じ件名を共有します。</span><span class="sxs-lookup"><span data-stu-id="1523d-p102">A conversation is a collection of [threads](conversationthread.md), and a thread contains posts to that thread. All threads and posts in a conversation share the same subject.</span></span>

<span data-ttu-id="1523d-107">このリソースは、[変更通知](/graph/webhooks)のサブスクライブをサポートしています。</span><span class="sxs-lookup"><span data-stu-id="1523d-107">This resource supports subscribing to [change notifications](/graph/webhooks).</span></span>

## <a name="methods"></a><span data-ttu-id="1523d-108">メソッド</span><span class="sxs-lookup"><span data-stu-id="1523d-108">Methods</span></span>

| <span data-ttu-id="1523d-109">メソッド</span><span class="sxs-lookup"><span data-stu-id="1523d-109">Method</span></span>       | <span data-ttu-id="1523d-110">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="1523d-110">Return Type</span></span>  |<span data-ttu-id="1523d-111">説明</span><span class="sxs-lookup"><span data-stu-id="1523d-111">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="1523d-112">会話を一覧表示する</span><span class="sxs-lookup"><span data-stu-id="1523d-112">List conversations</span></span>](../api/group-list-conversations.md) | <span data-ttu-id="1523d-113">[conversation](conversation.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="1523d-113">[conversation](conversation.md) collection</span></span> |<span data-ttu-id="1523d-114">このグループの会話の一覧を取得します。</span><span class="sxs-lookup"><span data-stu-id="1523d-114">Get the list of conversations in this group.</span></span>|
|[<span data-ttu-id="1523d-115">Create</span><span class="sxs-lookup"><span data-stu-id="1523d-115">Create</span></span>](../api/group-post-conversations.md) |[<span data-ttu-id="1523d-116">conversation</span><span class="sxs-lookup"><span data-stu-id="1523d-116">conversation</span></span>](conversation.md)| <span data-ttu-id="1523d-117">スレッドと投稿を含めて、新しい会話を作成します。</span><span class="sxs-lookup"><span data-stu-id="1523d-117">Create a new conversation by including a thread and a post.</span></span>|
|[<span data-ttu-id="1523d-118">会話を取得する</span><span class="sxs-lookup"><span data-stu-id="1523d-118">Get conversation</span></span>](../api/conversation-get.md) | [<span data-ttu-id="1523d-119">conversation</span><span class="sxs-lookup"><span data-stu-id="1523d-119">conversation</span></span>](conversation.md) |<span data-ttu-id="1523d-120">会話オブジェクトのプロパティと関係を読み取ります。</span><span class="sxs-lookup"><span data-stu-id="1523d-120">Read properties and relationships of conversation object.</span></span>|
|[<span data-ttu-id="1523d-121">Delete</span><span class="sxs-lookup"><span data-stu-id="1523d-121">Delete</span></span>](../api/conversation-delete.md) | <span data-ttu-id="1523d-122">なし</span><span class="sxs-lookup"><span data-stu-id="1523d-122">None</span></span> |<span data-ttu-id="1523d-123">conversation オブジェクトを削除します。</span><span class="sxs-lookup"><span data-stu-id="1523d-123">Delete conversation object.</span></span> |
|[<span data-ttu-id="1523d-124">会話スレッドを一覧表示する</span><span class="sxs-lookup"><span data-stu-id="1523d-124">List conversation threads</span></span>](../api/conversation-list-threads.md) |<span data-ttu-id="1523d-125">[conversationThread](conversationthread.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="1523d-125">[conversationThread](conversationthread.md) collection</span></span>| <span data-ttu-id="1523d-126">グループの会話のすべてのスレッドを取得します。</span><span class="sxs-lookup"><span data-stu-id="1523d-126">Get all the threads in a group conversation.</span></span>|
|[<span data-ttu-id="1523d-127">会話スレッドを作成する</span><span class="sxs-lookup"><span data-stu-id="1523d-127">Create conversation thread</span></span>](../api/conversation-post-threads.md) |<span data-ttu-id="1523d-128">[conversationThread](conversationthread.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="1523d-128">[conversationThread](conversationthread.md) collection</span></span>| <span data-ttu-id="1523d-129">指定した会話にスレッドを作成します。</span><span class="sxs-lookup"><span data-stu-id="1523d-129">Create a thread in the specified conversation.</span></span>|

## <a name="properties"></a><span data-ttu-id="1523d-130">プロパティ</span><span class="sxs-lookup"><span data-stu-id="1523d-130">Properties</span></span>
| <span data-ttu-id="1523d-131">プロパティ</span><span class="sxs-lookup"><span data-stu-id="1523d-131">Property</span></span>     | <span data-ttu-id="1523d-132">型</span><span class="sxs-lookup"><span data-stu-id="1523d-132">Type</span></span>   |<span data-ttu-id="1523d-133">説明</span><span class="sxs-lookup"><span data-stu-id="1523d-133">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="1523d-134">hasAttachments</span><span class="sxs-lookup"><span data-stu-id="1523d-134">hasAttachments</span></span>|<span data-ttu-id="1523d-135">Boolean</span><span class="sxs-lookup"><span data-stu-id="1523d-135">Boolean</span></span>|<span data-ttu-id="1523d-136">この会話内のいずれかの投稿に添付ファイルが 1 つ以上あるかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="1523d-136">Indicates whether any of the posts within this Conversation has at least one attachment.</span></span>|
|<span data-ttu-id="1523d-137">id</span><span class="sxs-lookup"><span data-stu-id="1523d-137">id</span></span>|<span data-ttu-id="1523d-138">String</span><span class="sxs-lookup"><span data-stu-id="1523d-138">String</span></span>|<span data-ttu-id="1523d-p103">会話の一意識別子。読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="1523d-p103">The conversations's unique identifier. Read-only.</span></span>|
|<span data-ttu-id="1523d-141">lastDeliveredDateTime</span><span class="sxs-lookup"><span data-stu-id="1523d-141">lastDeliveredDateTime</span></span>|<span data-ttu-id="1523d-142">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="1523d-142">DateTimeOffset</span></span>|<span data-ttu-id="1523d-p104">Timestamp 型は、ISO 8601 形式を使用して日付と時刻の情報を表し、必ず UTC 時間です。たとえば、2014 年 1 月 1 日午前 0 時 (UTC) は、次のようになります。`'2014-01-01T00:00:00Z'`</span><span class="sxs-lookup"><span data-stu-id="1523d-p104">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time. For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|
|<span data-ttu-id="1523d-145">preview</span><span class="sxs-lookup"><span data-stu-id="1523d-145">preview</span></span>|<span data-ttu-id="1523d-146">String</span><span class="sxs-lookup"><span data-stu-id="1523d-146">String</span></span>|<span data-ttu-id="1523d-147">この会話における最新投稿の本文からの短い概要。</span><span class="sxs-lookup"><span data-stu-id="1523d-147">A short summary from the body of the latest post in this converstaion.</span></span>|
|<span data-ttu-id="1523d-148">topic</span><span class="sxs-lookup"><span data-stu-id="1523d-148">topic</span></span>|<span data-ttu-id="1523d-149">String</span><span class="sxs-lookup"><span data-stu-id="1523d-149">String</span></span>|<span data-ttu-id="1523d-p105">会話のトピックです。会話の作成時にこのプロパティを設定できますが、更新することはできません。</span><span class="sxs-lookup"><span data-stu-id="1523d-p105">The topic of the conversation. This property can be set when the conversation is created, but it cannot be updated.</span></span>|
|<span data-ttu-id="1523d-152">uniqueSenders</span><span class="sxs-lookup"><span data-stu-id="1523d-152">uniqueSenders</span></span>|<span data-ttu-id="1523d-153">String collection</span><span class="sxs-lookup"><span data-stu-id="1523d-153">String collection</span></span>|<span data-ttu-id="1523d-154">この会話にメッセージを送信したすべてのユーザーです。</span><span class="sxs-lookup"><span data-stu-id="1523d-154">All the users that sent a message to this Conversation.</span></span>|

## <a name="relationships"></a><span data-ttu-id="1523d-155">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="1523d-155">Relationships</span></span>
| <span data-ttu-id="1523d-156">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="1523d-156">Relationship</span></span> | <span data-ttu-id="1523d-157">型</span><span class="sxs-lookup"><span data-stu-id="1523d-157">Type</span></span>   |<span data-ttu-id="1523d-158">説明</span><span class="sxs-lookup"><span data-stu-id="1523d-158">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="1523d-159">threads</span><span class="sxs-lookup"><span data-stu-id="1523d-159">threads</span></span>|<span data-ttu-id="1523d-160">[conversationThread](conversationthread.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="1523d-160">[conversationThread](conversationthread.md) collection</span></span>|<span data-ttu-id="1523d-p106">会話内のすべての会話スレッドのコレクションです。ナビゲーションのプロパティです。読み取り専用です。Null 許容型。</span><span class="sxs-lookup"><span data-stu-id="1523d-p106">A collection of all the conversation threads in the conversation. A navigation property. Read-only. Nullable.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="1523d-165">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="1523d-165">JSON representation</span></span>

<span data-ttu-id="1523d-166">以下は、リソースの JSON 表記です</span><span class="sxs-lookup"><span data-stu-id="1523d-166">Here is a JSON representation of the resource</span></span>

<!--{
  "blockType": "resource",
  "optionalProperties": [
    "threads"
  ],
  "keyProperty": "id",
  "baseType": "microsoft.graph.entity",
  "@odata.type": "microsoft.graph.conversation",
  "@odata.annotations": [
    {
      "property": "threads",
      "capabilities": {
        "changeTracking": false,
        "searchable": false
      }
    }
  ]
}-->

```json
{
  "hasAttachments": true,
  "id": "string (identifier)",
  "lastDeliveredDateTime": "String (timestamp)",
  "preview": "string",
  "topic": "string",
  "uniqueSenders": ["string"],

  "threads": [{"@odata.type": "microsoft.graph.conversationThread"}]
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
