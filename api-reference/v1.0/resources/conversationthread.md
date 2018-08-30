# <a name="conversationthread-resource-type"></a><span data-ttu-id="4065d-101">conversationThread リソースの種類</span><span class="sxs-lookup"><span data-stu-id="4065d-101">conversationThread resource type</span></span>
<span data-ttu-id="4065d-102">onversationThread は、[投稿](post.md)のコレクションです。</span><span class="sxs-lookup"><span data-stu-id="4065d-102">A conversationThread is a collection of [posts](post.md).</span></span>

<span data-ttu-id="4065d-p101">最後の投稿の受信者コレクションはスレッド全体の集計された受信者です。スレッドの受信者コレクションは増大する可能性があります。スレッドから受信者が削除されると、新しいスレッドが作成されます。</span><span class="sxs-lookup"><span data-stu-id="4065d-p101">The last post's recipients collection is the aggregated recipients of the entire thread. A thread can have a growing collection of recipients. A new thread is created when a recipient is removed from the thread.</span></span>

## <a name="methods"></a><span data-ttu-id="4065d-106">メソッド</span><span class="sxs-lookup"><span data-stu-id="4065d-106">Methods</span></span>

| <span data-ttu-id="4065d-107">メソッド</span><span class="sxs-lookup"><span data-stu-id="4065d-107">Method</span></span>       | <span data-ttu-id="4065d-108">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="4065d-108">Return Type</span></span>  |<span data-ttu-id="4065d-109">説明</span><span class="sxs-lookup"><span data-stu-id="4065d-109">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="4065d-110">スレッドを一覧表示する</span><span class="sxs-lookup"><span data-stu-id="4065d-110">List threads</span></span>](../api/group_list_threads.md) | <span data-ttu-id="4065d-111">[conversationThread](conversationthread.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="4065d-111">[conversationThread](conversationthread.md) collection</span></span> |<span data-ttu-id="4065d-112">グループのすべてのスレッドを取得します。</span><span class="sxs-lookup"><span data-stu-id="4065d-112">Get all the threads of a group.</span></span>|
|[<span data-ttu-id="4065d-113">スレッドを作成する</span><span class="sxs-lookup"><span data-stu-id="4065d-113">Create thread</span></span>](../api/group_post_threads.md) | [<span data-ttu-id="4065d-114">conversationThread</span><span class="sxs-lookup"><span data-stu-id="4065d-114">conversationThread</span></span>](conversationthread.md) |<span data-ttu-id="4065d-p102">最初にスレッドを作成して、新しい会話を開始します。グループには、新しい会話、会話スレッド、および投稿が作成されます。</span><span class="sxs-lookup"><span data-stu-id="4065d-p102">Start a new conversation by first creating a thread. A new conversation, conversation thread, and post are created in the group.</span></span>|
|[<span data-ttu-id="4065d-117">conversationThread を取得する</span><span class="sxs-lookup"><span data-stu-id="4065d-117">Get conversationThread</span></span>](../api/conversationthread_get.md) | [<span data-ttu-id="4065d-118">conversationThread</span><span class="sxs-lookup"><span data-stu-id="4065d-118">conversationThread</span></span>](conversationthread.md) |<span data-ttu-id="4065d-119">グループに属している特定のスレッドを取得します。</span><span class="sxs-lookup"><span data-stu-id="4065d-119">Get a specific thread that belongs to a group.</span></span> |
|[<span data-ttu-id="4065d-120">更新</span><span class="sxs-lookup"><span data-stu-id="4065d-120">Update</span></span>](../api/conversationthread_update.md) | [<span data-ttu-id="4065d-121">conversationThread</span><span class="sxs-lookup"><span data-stu-id="4065d-121">conversationThread</span></span>](conversationthread.md)  |<span data-ttu-id="4065d-122">conversationThread オブジェクトを更新します。</span><span class="sxs-lookup"><span data-stu-id="4065d-122">Update conversationThread object.</span></span> |
|[<span data-ttu-id="4065d-123">削除</span><span class="sxs-lookup"><span data-stu-id="4065d-123">Delete</span></span>](../api/conversationthread_delete.md) | <span data-ttu-id="4065d-124">なし</span><span class="sxs-lookup"><span data-stu-id="4065d-124">None</span></span> |<span data-ttu-id="4065d-125">conversationThread オブジェクトを削除します。</span><span class="sxs-lookup"><span data-stu-id="4065d-125">Delete conversationThread object.</span></span> |
|[<span data-ttu-id="4065d-126">返信</span><span class="sxs-lookup"><span data-stu-id="4065d-126">Reply</span></span>](../api/conversationthread_reply.md)|<span data-ttu-id="4065d-127">なし</span><span class="sxs-lookup"><span data-stu-id="4065d-127">None</span></span>|<span data-ttu-id="4065d-128">新しい投稿のエンティティを作成して、このスレッドに返信します。</span><span class="sxs-lookup"><span data-stu-id="4065d-128">Reply to this thread by creating a new Post entity.</span></span>|
|[<span data-ttu-id="4065d-129">投稿を一覧表示する</span><span class="sxs-lookup"><span data-stu-id="4065d-129">List Posts</span></span>](../api/conversationthread_list_posts.md) |<span data-ttu-id="4065d-130">[post](post.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="4065d-130">[post](post.md) collection</span></span>| <span data-ttu-id="4065d-131">指定したスレッドの投稿を取得します。</span><span class="sxs-lookup"><span data-stu-id="4065d-131">Get the posts of the specified thread.</span></span> |

## <a name="properties"></a><span data-ttu-id="4065d-132">プロパティ</span><span class="sxs-lookup"><span data-stu-id="4065d-132">Properties</span></span>
| <span data-ttu-id="4065d-133">プロパティ</span><span class="sxs-lookup"><span data-stu-id="4065d-133">Property</span></span>     | <span data-ttu-id="4065d-134">タイプ</span><span class="sxs-lookup"><span data-stu-id="4065d-134">Type</span></span>   |<span data-ttu-id="4065d-135">説明</span><span class="sxs-lookup"><span data-stu-id="4065d-135">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="4065d-136">ID</span><span class="sxs-lookup"><span data-stu-id="4065d-136">id</span></span>|<span data-ttu-id="4065d-137">文字列</span><span class="sxs-lookup"><span data-stu-id="4065d-137">String</span></span>| <span data-ttu-id="4065d-138">読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="4065d-138">Read-only.</span></span>|
|<span data-ttu-id="4065d-139">toRecipients</span><span class="sxs-lookup"><span data-stu-id="4065d-139">toRecipients</span></span>|<span data-ttu-id="4065d-140">[recipient](recipient.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="4065d-140">[recipient](recipient.md) collection</span></span>|<span data-ttu-id="4065d-141">スレッドの宛先の受信者。</span><span class="sxs-lookup"><span data-stu-id="4065d-141">The To: recipients for the thread.</span></span>|
|<span data-ttu-id="4065d-142">ccRecipients</span><span class="sxs-lookup"><span data-stu-id="4065d-142">ccRecipients</span></span>|<span data-ttu-id="4065d-143">[recipient](recipient.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="4065d-143">[recipient](recipient.md) collection</span></span>|<span data-ttu-id="4065d-144">スレッドの CC の受信者。</span><span class="sxs-lookup"><span data-stu-id="4065d-144">The Cc: recipients for the thread.</span></span>|
|<span data-ttu-id="4065d-145">トピック</span><span class="sxs-lookup"><span data-stu-id="4065d-145">topic</span></span>|<span data-ttu-id="4065d-146">文字列</span><span class="sxs-lookup"><span data-stu-id="4065d-146">String</span></span>|<span data-ttu-id="4065d-p103">会話のトピックです。会話の作成時にこのプロパティを設定できますが、更新することはできません。</span><span class="sxs-lookup"><span data-stu-id="4065d-p103">The topic of the conversation. This property can be set when the conversation is created, but it cannot be updated.</span></span>||
|<span data-ttu-id="4065d-149">hasAttachments</span><span class="sxs-lookup"><span data-stu-id="4065d-149">hasAttachments</span></span>|<span data-ttu-id="4065d-150">ブール値</span><span class="sxs-lookup"><span data-stu-id="4065d-150">Boolean</span></span>|<span data-ttu-id="4065d-151">このスレッド内のいずれかの投稿に添付ファイルが 1 つ以上あるかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="4065d-151">Indicates whether any of the posts within this thread has at least one attachment.</span></span>|
|<span data-ttu-id="4065d-152">lastDeliveredDateTime</span><span class="sxs-lookup"><span data-stu-id="4065d-152">lastDeliveredDateTime</span></span>|<span data-ttu-id="4065d-153">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="4065d-153">DateTimeOffset</span></span>|<span data-ttu-id="4065d-p104">Timestamp 型は、ISO 8601 形式を使用して日付と時刻の情報を表し、必ず UTC 時間です。たとえば、2014 年 1 月 1 日午前 0 時 (UTC) は、次のようになります。 `'2014-01-01T00:00:00Z'`</span><span class="sxs-lookup"><span data-stu-id="4065d-p104">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time. For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|
|<span data-ttu-id="4065d-156">uniqueSenders</span><span class="sxs-lookup"><span data-stu-id="4065d-156">uniqueSenders</span></span>|<span data-ttu-id="4065d-157">String コレクション</span><span class="sxs-lookup"><span data-stu-id="4065d-157">String collection</span></span>|<span data-ttu-id="4065d-158">このスレッドにメッセージを送信したすべてのユーザー。</span><span class="sxs-lookup"><span data-stu-id="4065d-158">All the users that sent a message to this thread.</span></span>|
|<span data-ttu-id="4065d-159">プレビュー</span><span class="sxs-lookup"><span data-stu-id="4065d-159">preview</span></span>|<span data-ttu-id="4065d-160">文字列</span><span class="sxs-lookup"><span data-stu-id="4065d-160">String</span></span>|<span data-ttu-id="4065d-161">この会話における最新投稿の本文からの短い概要。</span><span class="sxs-lookup"><span data-stu-id="4065d-161">A short summary from the body of the latest post in this converstaion.</span></span>|
|<span data-ttu-id="4065d-162">isLocked</span><span class="sxs-lookup"><span data-stu-id="4065d-162">isLocked</span></span>|<span data-ttu-id="4065d-163">ブール値</span><span class="sxs-lookup"><span data-stu-id="4065d-163">Boolean</span></span>|<span data-ttu-id="4065d-164">スレッドがロックされているかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="4065d-164">Indicates if the thread is locked.</span></span>|

## <a name="relationships"></a><span data-ttu-id="4065d-165">関係</span><span class="sxs-lookup"><span data-stu-id="4065d-165">Relationships</span></span>
| <span data-ttu-id="4065d-166">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="4065d-166">Relationship</span></span> | <span data-ttu-id="4065d-167">型</span><span class="sxs-lookup"><span data-stu-id="4065d-167">Type</span></span>   |<span data-ttu-id="4065d-168">説明</span><span class="sxs-lookup"><span data-stu-id="4065d-168">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="4065d-169">投稿</span><span class="sxs-lookup"><span data-stu-id="4065d-169">posts</span></span>|<span data-ttu-id="4065d-170">[post](post.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="4065d-170">[post](post.md) collection</span></span>| <span data-ttu-id="4065d-p105">読み取り専用です。Null 許容型。</span><span class="sxs-lookup"><span data-stu-id="4065d-p105">Read-only. Nullable.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="4065d-173">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="4065d-173">JSON representation</span></span>

<span data-ttu-id="4065d-174">以下は、リソースの JSON 表記です</span><span class="sxs-lookup"><span data-stu-id="4065d-174">Here is a JSON representation of the resource</span></span>

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
