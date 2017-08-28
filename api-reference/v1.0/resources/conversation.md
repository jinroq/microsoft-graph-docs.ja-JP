# <a name="conversation-resource-type"></a><span data-ttu-id="512f7-101">会話リソースの種類</span><span class="sxs-lookup"><span data-stu-id="512f7-101">conversation resource type</span></span>

<span data-ttu-id="512f7-p101">会話は[スレッド](conversationthread.md)のコレクションです。スレッドにはそのスレッドへの投稿が含まれています。会話のすべてのスレッドと投稿は同じ件名を共有します。</span><span class="sxs-lookup"><span data-stu-id="512f7-p101">A conversation is a collection of [threads](conversationthread.md), and a thread contains posts to that thread. All threads and posts in a conversation share the same subject.</span></span>

## <a name="methods"></a><span data-ttu-id="512f7-104">メソッド</span><span class="sxs-lookup"><span data-stu-id="512f7-104">Methods</span></span>

| <span data-ttu-id="512f7-105">メソッド</span><span class="sxs-lookup"><span data-stu-id="512f7-105">Method</span></span>       | <span data-ttu-id="512f7-106">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="512f7-106">Return Type</span></span>  |<span data-ttu-id="512f7-107">説明</span><span class="sxs-lookup"><span data-stu-id="512f7-107">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="512f7-108">会話を一覧表示する</span><span class="sxs-lookup"><span data-stu-id="512f7-108">List conversations</span></span>](../api/group_list_conversations.md) | <span data-ttu-id="512f7-109">[conversation](conversation.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="512f7-109">[conversation](conversation.md) collection</span></span> |<span data-ttu-id="512f7-110">このグループの会話の一覧を取得します。</span><span class="sxs-lookup"><span data-stu-id="512f7-110">Get the list of conversations in this group.</span></span>|
|[<span data-ttu-id="512f7-111">Create</span><span class="sxs-lookup"><span data-stu-id="512f7-111">Create</span></span>](../api/group_post_conversations.md) |[<span data-ttu-id="512f7-112">conversation</span><span class="sxs-lookup"><span data-stu-id="512f7-112">conversation</span></span>](conversation.md)| <span data-ttu-id="512f7-113">スレッドと投稿を含めて、新しい会話を作成します。</span><span class="sxs-lookup"><span data-stu-id="512f7-113">Create a new conversation by including a thread and a post.</span></span>|
|[<span data-ttu-id="512f7-114">会話を取得する</span><span class="sxs-lookup"><span data-stu-id="512f7-114">Get conversation</span></span>](../api/conversation_get.md) | [<span data-ttu-id="512f7-115">conversation</span><span class="sxs-lookup"><span data-stu-id="512f7-115">conversation</span></span>](conversation.md) |<span data-ttu-id="512f7-116">会話オブジェクトのプロパティと関係を読み取ります。</span><span class="sxs-lookup"><span data-stu-id="512f7-116">Read properties and relationships of conversation object.</span></span>|
|[<span data-ttu-id="512f7-117">Delete</span><span class="sxs-lookup"><span data-stu-id="512f7-117">Delete</span></span>](../api/conversation_delete.md) | <span data-ttu-id="512f7-118">なし</span><span class="sxs-lookup"><span data-stu-id="512f7-118">None</span></span> |<span data-ttu-id="512f7-119">会話オブジェクトを削除します。</span><span class="sxs-lookup"><span data-stu-id="512f7-119">Delete conversation object.</span></span> |
|[<span data-ttu-id="512f7-120">会話スレッドを一覧表示する</span><span class="sxs-lookup"><span data-stu-id="512f7-120">List conversation threads</span></span>](../api/conversation_list_threads.md) |<span data-ttu-id="512f7-121">[conversationThread](conversationthread.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="512f7-121">[conversationThread](conversationthread.md) collection</span></span>| <span data-ttu-id="512f7-122">グループの会話のすべてのスレッドを取得します。</span><span class="sxs-lookup"><span data-stu-id="512f7-122">Get all the threads in a group conversation.</span></span>|
|[<span data-ttu-id="512f7-123">会話スレッドを作成する</span><span class="sxs-lookup"><span data-stu-id="512f7-123">Create conversation thread</span></span>](../api/conversation_post_threads.md) |<span data-ttu-id="512f7-124">[conversationThread](conversationthread.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="512f7-124">[conversationThread](conversationthread.md) collection</span></span>| <span data-ttu-id="512f7-125">指定した会話にスレッドを作成します。</span><span class="sxs-lookup"><span data-stu-id="512f7-125">Create a thread in the specified conversation.</span></span>|

## <a name="properties"></a><span data-ttu-id="512f7-126">プロパティ</span><span class="sxs-lookup"><span data-stu-id="512f7-126">Properties</span></span>
| <span data-ttu-id="512f7-127">プロパティ</span><span class="sxs-lookup"><span data-stu-id="512f7-127">Property</span></span>     | <span data-ttu-id="512f7-128">型</span><span class="sxs-lookup"><span data-stu-id="512f7-128">Type</span></span>   |<span data-ttu-id="512f7-129">説明</span><span class="sxs-lookup"><span data-stu-id="512f7-129">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="512f7-130">hasAttachments</span><span class="sxs-lookup"><span data-stu-id="512f7-130">hasAttachments</span></span>|<span data-ttu-id="512f7-131">Boolean</span><span class="sxs-lookup"><span data-stu-id="512f7-131">Boolean</span></span>|<span data-ttu-id="512f7-132">この会話内のいずれかの投稿に添付ファイルが 1 つ以上あるかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="512f7-132">Indicates whether any of the posts within this Conversation has at least one attachment.</span></span>|
|<span data-ttu-id="512f7-133">id</span><span class="sxs-lookup"><span data-stu-id="512f7-133">id</span></span>|<span data-ttu-id="512f7-134">String</span><span class="sxs-lookup"><span data-stu-id="512f7-134">String</span></span>|<span data-ttu-id="512f7-p102">会話の一意識別子。読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="512f7-p102">The conversations's unique identifier. Read-only.</span></span>|
|<span data-ttu-id="512f7-137">lastDeliveredDateTime</span><span class="sxs-lookup"><span data-stu-id="512f7-137">lastDeliveredDateTime</span></span>|<span data-ttu-id="512f7-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="512f7-138">DateTimeOffset</span></span>|<span data-ttu-id="512f7-p103">Timestamp 型は、ISO 8601 形式を使用して日付と時刻の情報を表し、必ず UTC 時間です。たとえば、2014 年 1 月 1 日午前 0 時 (UTC) は、次のようになります。`'2014-01-01T00:00:00Z'`</span><span class="sxs-lookup"><span data-stu-id="512f7-p103">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time. For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|
|<span data-ttu-id="512f7-141">preview</span><span class="sxs-lookup"><span data-stu-id="512f7-141">preview</span></span>|<span data-ttu-id="512f7-142">String</span><span class="sxs-lookup"><span data-stu-id="512f7-142">String</span></span>|<span data-ttu-id="512f7-143">この会話における最新投稿の本文からの短い概要。</span><span class="sxs-lookup"><span data-stu-id="512f7-143">A short summary from the body of the latest post in this converstaion.</span></span>|
|<span data-ttu-id="512f7-144">topic</span><span class="sxs-lookup"><span data-stu-id="512f7-144">topic</span></span>|<span data-ttu-id="512f7-145">String</span><span class="sxs-lookup"><span data-stu-id="512f7-145">String</span></span>|<span data-ttu-id="512f7-p104">会話のトピックです。会話の作成時にこのプロパティを設定できますが、更新することはできません。</span><span class="sxs-lookup"><span data-stu-id="512f7-p104">The topic of the conversation. This property can be set when the conversation is created, but it cannot be updated.</span></span>|
|<span data-ttu-id="512f7-148">uniqueSenders</span><span class="sxs-lookup"><span data-stu-id="512f7-148">uniqueSenders</span></span>|<span data-ttu-id="512f7-149">String collection</span><span class="sxs-lookup"><span data-stu-id="512f7-149">String collection</span></span>|<span data-ttu-id="512f7-150">この会話にメッセージを送信したすべてのユーザーです。</span><span class="sxs-lookup"><span data-stu-id="512f7-150">All the users that sent a message to this Conversation.</span></span>|

## <a name="relationships"></a><span data-ttu-id="512f7-151">関係</span><span class="sxs-lookup"><span data-stu-id="512f7-151">Relationships</span></span>
| <span data-ttu-id="512f7-152">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="512f7-152">Relationship</span></span> | <span data-ttu-id="512f7-153">型</span><span class="sxs-lookup"><span data-stu-id="512f7-153">Type</span></span>   |<span data-ttu-id="512f7-154">説明</span><span class="sxs-lookup"><span data-stu-id="512f7-154">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="512f7-155">スレッド</span><span class="sxs-lookup"><span data-stu-id="512f7-155">threads</span></span>|<span data-ttu-id="512f7-156">[conversationThread](conversationthread.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="512f7-156">[conversationThread](conversationthread.md) collection</span></span>|<span data-ttu-id="512f7-p105">会話内のすべての会話スレッドのコレクションです。ナビゲーションのプロパティです。読み取り専用です。Null 許容型。</span><span class="sxs-lookup"><span data-stu-id="512f7-p105">A collection of all the conversation threads in the conversation. A navigation property. Read-only. Nullable.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="512f7-161">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="512f7-161">JSON representation</span></span>

<span data-ttu-id="512f7-162">以下は、リソースの JSON 表記です</span><span class="sxs-lookup"><span data-stu-id="512f7-162">Here is a JSON representation of the resource</span></span>

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
