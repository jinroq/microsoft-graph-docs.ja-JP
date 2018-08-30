# <a name="post-resource-type"></a><span data-ttu-id="c09c9-101">post リソース タイプ</span><span class="sxs-lookup"><span data-stu-id="c09c9-101">post resource type</span></span>
<span data-ttu-id="c09c9-102">[conversationThread](conversationthread.md) エンティティ内の個々の投稿アイテムを表します。</span><span class="sxs-lookup"><span data-stu-id="c09c9-102">Represents an individual Post item within a [conversationThread](conversationthread.md) entity.</span></span>

<span data-ttu-id="c09c9-103">投稿を明示的に作成できなくても、次のいずれかの方法で投稿を作成できます。</span><span class="sxs-lookup"><span data-stu-id="c09c9-103">Even though you cannot explicitly create a post, doing any of the following would create a post:</span></span>

- [<span data-ttu-id="c09c9-104">既存の投稿に返信する</span><span class="sxs-lookup"><span data-stu-id="c09c9-104">Reply to an existing post</span></span>](../api/post_reply.md) 
- [<span data-ttu-id="c09c9-105">既存のスレッドに返信する</span><span class="sxs-lookup"><span data-stu-id="c09c9-105">Reply to an existing thread</span></span>](../api/conversationthread_reply.md) 
- [<span data-ttu-id="c09c9-106">新しい会話にスレッドを作成する</span><span class="sxs-lookup"><span data-stu-id="c09c9-106">Create a thread in a new conversation</span></span>](../api/group_post_threads.md)
- [<span data-ttu-id="c09c9-107">新しい会話を作成する</span><span class="sxs-lookup"><span data-stu-id="c09c9-107">Create a new conversation</span></span>](../api/group_post_conversations.md)

<span data-ttu-id="c09c9-108">このリソースでは、[拡張機能](../../../concepts/extensibility_overview.md)を使用してカスタム プロパティに独自のデータを追加することができます。</span><span class="sxs-lookup"><span data-stu-id="c09c9-108">This resource lets you add your own data to custom properties using [extensions](../../../concepts/extensibility_overview.md).</span></span>

## <a name="methods"></a><span data-ttu-id="c09c9-109">メソッド</span><span class="sxs-lookup"><span data-stu-id="c09c9-109">Methods</span></span>

| <span data-ttu-id="c09c9-110">メソッド</span><span class="sxs-lookup"><span data-stu-id="c09c9-110">Method</span></span>       | <span data-ttu-id="c09c9-111">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="c09c9-111">Return Type</span></span>  |<span data-ttu-id="c09c9-112">説明</span><span class="sxs-lookup"><span data-stu-id="c09c9-112">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="c09c9-113">List posts</span><span class="sxs-lookup"><span data-stu-id="c09c9-113">List posts</span></span>](../api/conversationthread_list_posts.md) | [<span data-ttu-id="c09c9-114">post</span><span class="sxs-lookup"><span data-stu-id="c09c9-114">post</span></span>](post.md) |<span data-ttu-id="c09c9-115">指定したスレッドの投稿を取得します。</span><span class="sxs-lookup"><span data-stu-id="c09c9-115">Get the posts of the specified thread.</span></span> |
|[<span data-ttu-id="c09c9-116">Get post</span><span class="sxs-lookup"><span data-stu-id="c09c9-116">Get post</span></span>](../api/post_get.md) | [<span data-ttu-id="c09c9-117">post</span><span class="sxs-lookup"><span data-stu-id="c09c9-117">post</span></span>](post.md) |<span data-ttu-id="c09c9-118">指定したスレッド内の投稿のプロパティと関係を取得します。</span><span class="sxs-lookup"><span data-stu-id="c09c9-118">Get the properties and relationships of a post in a specified thread.</span></span>|
|[<span data-ttu-id="c09c9-119">Reply</span><span class="sxs-lookup"><span data-stu-id="c09c9-119">Reply</span></span>](../api/post_reply.md)|<span data-ttu-id="c09c9-120">なし</span><span class="sxs-lookup"><span data-stu-id="c09c9-120">None</span></span>|<span data-ttu-id="c09c9-121">グループ会話の投稿に返信して、指定されたスレッドに新しい投稿を追加します。</span><span class="sxs-lookup"><span data-stu-id="c09c9-121">Reply to a post and add a new post to the specified thread in a group conversation.</span></span>|
|[<span data-ttu-id="c09c9-122">Forward</span><span class="sxs-lookup"><span data-stu-id="c09c9-122">Forward</span></span>](../api/post_forward.md)|<span data-ttu-id="c09c9-123">なし</span><span class="sxs-lookup"><span data-stu-id="c09c9-123">None</span></span>|<span data-ttu-id="c09c9-124">受信者に投稿を転送します。</span><span class="sxs-lookup"><span data-stu-id="c09c9-124">Forward a post to a recipient.</span></span>|
|<span data-ttu-id="c09c9-125">**添付ファイル**</span><span class="sxs-lookup"><span data-stu-id="c09c9-125">**Attachments**</span></span>| | |
|[<span data-ttu-id="c09c9-126">添付ファイルを一覧表示する</span><span class="sxs-lookup"><span data-stu-id="c09c9-126">List attachments</span></span>](../api/post_list_attachments.md) |<span data-ttu-id="c09c9-127">[attachment](attachment.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="c09c9-127">[attachment](attachment.md) collection</span></span>| <span data-ttu-id="c09c9-128">投稿のすべての添付ファイルを取得します。</span><span class="sxs-lookup"><span data-stu-id="c09c9-128">Get all attachments on a post.</span></span>|
|[<span data-ttu-id="c09c9-129">添付ファイルを追加する</span><span class="sxs-lookup"><span data-stu-id="c09c9-129">Add attachment</span></span>](../api/post_post_attachments.md) |[<span data-ttu-id="c09c9-130">attachment</span><span class="sxs-lookup"><span data-stu-id="c09c9-130">attachment</span></span>](attachment.md)| <span data-ttu-id="c09c9-131">投稿に添付ファイルを追加します。</span><span class="sxs-lookup"><span data-stu-id="c09c9-131">Add an attachment to a post.</span></span> |
|<span data-ttu-id="c09c9-132">**オープン拡張機能**</span><span class="sxs-lookup"><span data-stu-id="c09c9-132">**Open extensions**</span></span>| | |
|[<span data-ttu-id="c09c9-133">オープン拡張機能を作成する</span><span class="sxs-lookup"><span data-stu-id="c09c9-133">Create open extension</span></span>](../api/opentypeextension_post_opentypeextension.md) |[<span data-ttu-id="c09c9-134">openTypeExtension</span><span class="sxs-lookup"><span data-stu-id="c09c9-134">openTypeExtension</span></span>](opentypeextension.md)| <span data-ttu-id="c09c9-135">オープン拡張機能を作成し、リソースの新規または既存のインスタンスのカスタム プロパティを追加します。</span><span class="sxs-lookup"><span data-stu-id="c09c9-135">Create an open extension and add custom properties in a new or existing instance of a resource.</span></span>|
|[<span data-ttu-id="c09c9-136">オープン拡張機能を取得する</span><span class="sxs-lookup"><span data-stu-id="c09c9-136">Get open extension</span></span>](../api/opentypeextension_get.md) |<span data-ttu-id="c09c9-137">[openTypeExtension](opentypeextension.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="c09c9-137">[openTypeExtension](opentypeextension.md) collection</span></span>| <span data-ttu-id="c09c9-138">名前や完全修飾名によって識別されたオープン拡張機能オブジェクトを取得します。</span><span class="sxs-lookup"><span data-stu-id="c09c9-138">Get an open extension object or objects identified by name or fully qualified name.</span></span>|
|<span data-ttu-id="c09c9-139">**スキーマ拡張機能**</span><span class="sxs-lookup"><span data-stu-id="c09c9-139">**Schema extensions**</span></span>| | |
|[<span data-ttu-id="c09c9-140">スキーマ拡張機能の値を追加する</span><span class="sxs-lookup"><span data-stu-id="c09c9-140">Add schema extension values</span></span>](../../../concepts/extensibility_schema_groups.md) || <span data-ttu-id="c09c9-141">スキーマ拡張機能の定義を作成し、それを使用してカスタマイズされた種類のデータをリソースに追加します。</span><span class="sxs-lookup"><span data-stu-id="c09c9-141">Create a schema extension definition and then use it to add custom typed data to a resource.</span></span>|
|<span data-ttu-id="c09c9-142">**拡張プロパティ**</span><span class="sxs-lookup"><span data-stu-id="c09c9-142">**Extended properties**</span></span>| | |
|[<span data-ttu-id="c09c9-143">単一値の拡張プロパティを作成する</span><span class="sxs-lookup"><span data-stu-id="c09c9-143">Create single-value extended property</span></span>](../api/singlevaluelegacyextendedproperty_post_singlevalueextendedproperties.md) |[<span data-ttu-id="c09c9-144">post</span><span class="sxs-lookup"><span data-stu-id="c09c9-144">post</span></span>](post.md)  |<span data-ttu-id="c09c9-145">新規または既存の投稿に、ひとつまたは複数の単一値の拡張プロパティを作成します。</span><span class="sxs-lookup"><span data-stu-id="c09c9-145">Create one or more single-value extended properties in a new or existing post.</span></span>   |
|[<span data-ttu-id="c09c9-146">単一値の拡張プロパティをもつ投稿トを取得する</span><span class="sxs-lookup"><span data-stu-id="c09c9-146">Get post with single-value extended property</span></span>](../api/singlevaluelegacyextendedproperty_get.md)  | [<span data-ttu-id="c09c9-147">post</span><span class="sxs-lookup"><span data-stu-id="c09c9-147">post</span></span>](post.md) | <span data-ttu-id="c09c9-148">または `$filter` を使用して、単一値の拡張プロパティを含む投稿を取得します。`$expand`</span><span class="sxs-lookup"><span data-stu-id="c09c9-148">Get posts that contain a single-value extended property by using `$expand` or `$filter`.</span></span> |
|[<span data-ttu-id="c09c9-149">複数値の拡張プロパティを作成する</span><span class="sxs-lookup"><span data-stu-id="c09c9-149">Create multi-value extended property</span></span>](../api/multivaluelegacyextendedproperty_post_multivalueextendedproperties.md) | [<span data-ttu-id="c09c9-150">post</span><span class="sxs-lookup"><span data-stu-id="c09c9-150">post</span></span>](post.md) | <span data-ttu-id="c09c9-151">新規または既存の投稿に、ひとつまたは複数の複数値の拡張プロパティを作成します。</span><span class="sxs-lookup"><span data-stu-id="c09c9-151">Create one or more multi-value extended properties in a new or existing post.</span></span>  |
|[<span data-ttu-id="c09c9-152">複数値の拡張プロパティをもつ投稿を取得する</span><span class="sxs-lookup"><span data-stu-id="c09c9-152">Get post with multi-value extended property</span></span>](../api/multivaluelegacyextendedproperty_get.md)  | [<span data-ttu-id="c09c9-153">post</span><span class="sxs-lookup"><span data-stu-id="c09c9-153">post</span></span>](post.md) | <span data-ttu-id="c09c9-154">を使用して、複数値の拡張プロパティを含む投稿を取得します。`$expand`</span><span class="sxs-lookup"><span data-stu-id="c09c9-154">Get a post that contains a multi-value extended property by using `$expand`.</span></span> |

## <a name="properties"></a><span data-ttu-id="c09c9-155">プロパティ</span><span class="sxs-lookup"><span data-stu-id="c09c9-155">Properties</span></span>
| <span data-ttu-id="c09c9-156">プロパティ</span><span class="sxs-lookup"><span data-stu-id="c09c9-156">Property</span></span>     | <span data-ttu-id="c09c9-157">タイプ</span><span class="sxs-lookup"><span data-stu-id="c09c9-157">Type</span></span>   |<span data-ttu-id="c09c9-158">説明</span><span class="sxs-lookup"><span data-stu-id="c09c9-158">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="c09c9-159">body</span><span class="sxs-lookup"><span data-stu-id="c09c9-159">body</span></span>|[<span data-ttu-id="c09c9-160">itemBody</span><span class="sxs-lookup"><span data-stu-id="c09c9-160">itemBody</span></span>](itembody.md)|<span data-ttu-id="c09c9-p101">投稿の内容です。これが既定のプロパティです。このプロパティを null にすることができます。</span><span class="sxs-lookup"><span data-stu-id="c09c9-p101">The contents of the post. This is a default property. This property can be null.</span></span>|
|<span data-ttu-id="c09c9-164">categories</span><span class="sxs-lookup"><span data-stu-id="c09c9-164">categories</span></span>|<span data-ttu-id="c09c9-165">String コレクション</span><span class="sxs-lookup"><span data-stu-id="c09c9-165">String collection</span></span>|<span data-ttu-id="c09c9-166">投稿に関連付けられたカテゴリ。</span><span class="sxs-lookup"><span data-stu-id="c09c9-166">The categories associated with the post.</span></span>|
|<span data-ttu-id="c09c9-167">changeKey</span><span class="sxs-lookup"><span data-stu-id="c09c9-167">changeKey</span></span>|<span data-ttu-id="c09c9-168">String</span><span class="sxs-lookup"><span data-stu-id="c09c9-168">String</span></span>|<span data-ttu-id="c09c9-p102">投稿のバージョンを識別します。投稿を変更するたびに ChangeKey も変更されます。これにより、Exchange は正しいバージョンのオブジェクトに変更を適用できます。</span><span class="sxs-lookup"><span data-stu-id="c09c9-p102">Identifies the version of the post. Every time the post is changed, ChangeKey changes as well. This allows Exchange to apply changes to the correct version of the object.</span></span>|
|<span data-ttu-id="c09c9-172">conversationId</span><span class="sxs-lookup"><span data-stu-id="c09c9-172">conversationId</span></span>|<span data-ttu-id="c09c9-173">String</span><span class="sxs-lookup"><span data-stu-id="c09c9-173">String</span></span>|<span data-ttu-id="c09c9-p103">会話の固有 ID です。読み取り専用。</span><span class="sxs-lookup"><span data-stu-id="c09c9-p103">Unique ID of the conversation. Read-only.</span></span>|
|<span data-ttu-id="c09c9-176">conversationThreadId</span><span class="sxs-lookup"><span data-stu-id="c09c9-176">conversationThreadId</span></span>|<span data-ttu-id="c09c9-177">String</span><span class="sxs-lookup"><span data-stu-id="c09c9-177">String</span></span>|<span data-ttu-id="c09c9-p104">会話スレッドの固有 ID です。読み取り専用。</span><span class="sxs-lookup"><span data-stu-id="c09c9-p104">Unique ID of the conversation thread. Read-only.</span></span>|
|<span data-ttu-id="c09c9-180">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="c09c9-180">createdDateTime</span></span>|<span data-ttu-id="c09c9-181">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="c09c9-181">DateTimeOffset</span></span>|<span data-ttu-id="c09c9-p105">投稿の作成時刻を示します。DateTimeOffset 型は、ISO 8601 形式を使用して日付と時刻の情報を表し、常に UTC 時間です。たとえば、2014 年 1 月 1 日午前 0 時 (UTC) は、次のようになります。 `'2014-01-01T00:00:00Z'`</span><span class="sxs-lookup"><span data-stu-id="c09c9-p105">Specifies when the post was created. The DateTimeOffset type represents date and time information using ISO 8601 format and is always in UTC time. For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|
|<span data-ttu-id="c09c9-185">from</span><span class="sxs-lookup"><span data-stu-id="c09c9-185">from</span></span>|[<span data-ttu-id="c09c9-186">recipient</span><span class="sxs-lookup"><span data-stu-id="c09c9-186">recipient</span></span>](recipient.md)|<span data-ttu-id="c09c9-p106">代理人アクセスのシナリオで使用されます。他のユーザーの代わりにメッセージを投稿したユーザーを示します。これが既定のプロパティです。</span><span class="sxs-lookup"><span data-stu-id="c09c9-p106">Used in delegate access scenarios. Indicates who posted the message on behalf of another user. This is a default property.</span></span>|
|<span data-ttu-id="c09c9-190">hasAttachments</span><span class="sxs-lookup"><span data-stu-id="c09c9-190">hasAttachments</span></span>|<span data-ttu-id="c09c9-191">ブール型</span><span class="sxs-lookup"><span data-stu-id="c09c9-191">Boolean</span></span>|<span data-ttu-id="c09c9-p107">投稿の添付ファイルが 1 つ以上あるかどうかを示します。これが既定のプロパティです。</span><span class="sxs-lookup"><span data-stu-id="c09c9-p107">Indicates whether the post has at least one attachment. This is a default property.</span></span>|
|<span data-ttu-id="c09c9-194">id</span><span class="sxs-lookup"><span data-stu-id="c09c9-194">id</span></span>|<span data-ttu-id="c09c9-195">文字列</span><span class="sxs-lookup"><span data-stu-id="c09c9-195">String</span></span>| <span data-ttu-id="c09c9-196">読み取り専用。</span><span class="sxs-lookup"><span data-stu-id="c09c9-196">Read-only.</span></span>|
|<span data-ttu-id="c09c9-197">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="c09c9-197">lastModifiedDateTime</span></span>|<span data-ttu-id="c09c9-198">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="c09c9-198">DateTimeOffset</span></span>|<span data-ttu-id="c09c9-p108">投稿が最後に修正された日時を指定します。DateTimeOffset 型は、ISO 8601 形式を使用して日付と時刻の情報を表し、常に UTC 時間です。たとえば、2014 年 1 月 1 日午前 0 時 (UTC) は、次のようになります。 `'2014-01-01T00:00:00Z'`</span><span class="sxs-lookup"><span data-stu-id="c09c9-p108">Specifies when the post was last modified. The DateTimeOffset type represents date and time information using ISO 8601 format and is always in UTC time. For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|
|<span data-ttu-id="c09c9-202">newParticipants</span><span class="sxs-lookup"><span data-stu-id="c09c9-202">newParticipants</span></span>|<span data-ttu-id="c09c9-203">[recipient](recipient.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="c09c9-203">[recipient](recipient.md) collection</span></span>|<span data-ttu-id="c09c9-204">この投稿の一部としてスレッドに追加された会話の参加者です。</span><span class="sxs-lookup"><span data-stu-id="c09c9-204">Conversation participants that were added to the thread as part of this post.</span></span>|
|<span data-ttu-id="c09c9-205">receivedDateTime</span><span class="sxs-lookup"><span data-stu-id="c09c9-205">receivedDateTime</span></span>|<span data-ttu-id="c09c9-206">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="c09c9-206">DateTimeOffset</span></span>|<span data-ttu-id="c09c9-p109">投稿の受信時刻を示します。DateTimeOffset 型は、ISO 8601 形式を使用して日付と時刻の情報を表し、常に UTC 時間です。たとえば、2014 年 1 月 1 日午前 0 時 (UTC) は、次のようになります。 `'2014-01-01T00:00:00Z'`</span><span class="sxs-lookup"><span data-stu-id="c09c9-p109">Specifies when the post was received. The DateTimeOffset type represents date and time information using ISO 8601 format and is always in UTC time. For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|
|<span data-ttu-id="c09c9-210">sender</span><span class="sxs-lookup"><span data-stu-id="c09c9-210">sender</span></span>|[<span data-ttu-id="c09c9-211">recipient</span><span class="sxs-lookup"><span data-stu-id="c09c9-211">recipient</span></span>](recipient.md)|<span data-ttu-id="c09c9-p110">送信者のアドレスが含まれます。送信者が指定されていない場合、送信者の値は認証済みユーザーのアドレスと見なされます。これが既定のプロパティです。</span><span class="sxs-lookup"><span data-stu-id="c09c9-p110">Contains the address of the sender. The value of Sender is assumed to be the address of the authenticated user in the case when Sender is not specified. This is a default property.</span></span>|

## <a name="relationships"></a><span data-ttu-id="c09c9-215">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="c09c9-215">Relationships</span></span>
| <span data-ttu-id="c09c9-216">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="c09c9-216">Relationship</span></span> | <span data-ttu-id="c09c9-217">型</span><span class="sxs-lookup"><span data-stu-id="c09c9-217">Type</span></span>   |<span data-ttu-id="c09c9-218">説明</span><span class="sxs-lookup"><span data-stu-id="c09c9-218">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="c09c9-219">attachements</span><span class="sxs-lookup"><span data-stu-id="c09c9-219">attachments</span></span>|<span data-ttu-id="c09c9-220">[Attachment](attachment.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="c09c9-220">[Attachment](attachment.md) collection</span></span>| <span data-ttu-id="c09c9-p111">読み取り専用。Null 許容型。</span><span class="sxs-lookup"><span data-stu-id="c09c9-p111">Read-only. Nullable.</span></span>|
|<span data-ttu-id="c09c9-223">extensions</span><span class="sxs-lookup"><span data-stu-id="c09c9-223">extensions</span></span>|<span data-ttu-id="c09c9-224">[Extension](extension.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="c09c9-224">[Extension](extension.md) collection</span></span>|<span data-ttu-id="c09c9-p112">投稿に対して定義されているオープン拡張機能のコレクション。読み取り専用。Null 許容型。</span><span class="sxs-lookup"><span data-stu-id="c09c9-p112">The collection of open extensions defined for the post. Read-only. Nullable.</span></span>|
|<span data-ttu-id="c09c9-228">inReplyTo</span><span class="sxs-lookup"><span data-stu-id="c09c9-228">inReplyTo</span></span>|[<span data-ttu-id="c09c9-229">post</span><span class="sxs-lookup"><span data-stu-id="c09c9-229">post</span></span>](post.md)| <span data-ttu-id="c09c9-230">読み取り専用。</span><span class="sxs-lookup"><span data-stu-id="c09c9-230">Read-only.</span></span>|
|<span data-ttu-id="c09c9-231">multiValueExtendedProperties</span><span class="sxs-lookup"><span data-stu-id="c09c9-231">multiValueExtendedProperties</span></span>|<span data-ttu-id="c09c9-232">[multiValueLegacyExtendedProperty](multivaluelegacyextendedproperty.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="c09c9-232">[multiValueLegacyExtendedProperty](multivaluelegacyextendedproperty.md) collection</span></span>| <span data-ttu-id="c09c9-p113">その投稿用に定義された、複数値拡張プロパティのコレクションです。読み取り専用。Null 許容型。</span><span class="sxs-lookup"><span data-stu-id="c09c9-p113">The collection of multi-value extended properties defined for the post. Read-only. Nullable.</span></span>|
|<span data-ttu-id="c09c9-236">singleValueExtendedProperties</span><span class="sxs-lookup"><span data-stu-id="c09c9-236">singleValueExtendedProperties</span></span>|<span data-ttu-id="c09c9-237">[singleValueLegacyExtendedProperty](singlevaluelegacyextendedproperty.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="c09c9-237">[singleValueLegacyExtendedProperty](singlevaluelegacyextendedproperty.md) collection</span></span>| <span data-ttu-id="c09c9-p114">その投稿用に定義された、単一値拡張プロパティのコレクションです。読み取り専用。Null 許容型。</span><span class="sxs-lookup"><span data-stu-id="c09c9-p114">The collection of single-value extended properties defined for the post. Read-only. Nullable.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="c09c9-241">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="c09c9-241">JSON representation</span></span>

<span data-ttu-id="c09c9-242">以下は、リソースの JSON 表記です</span><span class="sxs-lookup"><span data-stu-id="c09c9-242">Here is a JSON representation of the resource</span></span>

<!--{
  "blockType": "resource",
  "openType": true,
  "optionalProperties": [
    "attachments",
    "inReplyTo",
    "multiValueExtendedProperties",
    "singleValueExtendedProperties"
  ],
  "baseType": "microsoft.graph.outlookItem",
  "@odata.type": "microsoft.graph.post",
  "@odata.annotations": [
    {
      "property": "attachments",
      "capabilities": {
        "changeTracking": false,
        "searchable": false,
        "updatable": false
      }
    },
    {
      "property": "extensions",
      "capabilities": {
        "changeTracking": false,
        "searchable": false
      }
    },
    {
      "property": "inReplyTo",
      "capabilities": {
        "changeTracking": false,
        "deletable": false,
        "insertable": false,
        "navigability": "single",
        "searchable": false,
        "updatable": false
      }
    }
  ]
}-->

```json
{
  "body": {"@odata.type": "microsoft.graph.itemBody"},
  "categories": ["string"],
  "changeKey": "string",
  "conversationId": "string",
  "conversationThreadId": "string",
  "createdDateTime": "String (timestamp)",
  "from": {"@odata.type": "microsoft.graph.recipient"},
  "hasAttachments": true,
  "id": "string (identifier)",
  "lastModifiedDateTime": "String (timestamp)",
  "newParticipants": [{"@odata.type": "microsoft.graph.recipient"}],
  "receivedDateTime": "String (timestamp)",
  "sender": {"@odata.type": "microsoft.graph.recipient"}
}

```

## <a name="see-also"></a><span data-ttu-id="c09c9-243">関連項目</span><span class="sxs-lookup"><span data-stu-id="c09c9-243">See also</span></span>

- [<span data-ttu-id="c09c9-244">拡張機能を使用してカスタム データをリソースに追加する</span><span class="sxs-lookup"><span data-stu-id="c09c9-244">Add custom data to resources using extensions</span></span>](../../../concepts/extensibility_overview.md)
- [<span data-ttu-id="c09c9-245">オープン拡張機能を使用してカスタム データをユーザーに追加する</span><span class="sxs-lookup"><span data-stu-id="c09c9-245">Add custom data to users using open extensions</span></span>](../../../concepts/extensibility_open_users.md)
- [<span data-ttu-id="c09c9-246">スキーマ拡張機能を使用したグループへのカスタム データの追加</span><span class="sxs-lookup"><span data-stu-id="c09c9-246">Add custom data to groups using schema extensions</span></span>](../../../concepts/extensibility_schema_groups.md)


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "post resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
