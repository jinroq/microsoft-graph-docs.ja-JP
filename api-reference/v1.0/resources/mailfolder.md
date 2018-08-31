# <a name="mailfolder-resource-type"></a><span data-ttu-id="26b25-101">mailFolder リソースの種類</span><span class="sxs-lookup"><span data-stu-id="26b25-101">mailFolder resource type</span></span>

<span data-ttu-id="26b25-102">受信トレイや下書きなどの、ユーザーのメールボックス内のメール フォルダーです。</span><span class="sxs-lookup"><span data-stu-id="26b25-102">A mail folder in a user's mailbox, such as Inbox and Drafts.</span></span> <span data-ttu-id="26b25-103">メール フォルダーには、メッセージ、他の Outlook アイテム、子メール フォルダーを含めることができます。</span><span class="sxs-lookup"><span data-stu-id="26b25-103">Mail folders can contain messages, other Outlook items, and child mail folders.</span></span>

<span data-ttu-id="26b25-104">このリソースでは、[デルタ](../api/mailfolder_delta.md)関数を用意すれば、増分の追加、削除、更新を追跡するために[デルタ クエリ](../../../concepts/delta_query_overview.md)を使用できます。</span><span class="sxs-lookup"><span data-stu-id="26b25-104">This resource supports using [delta query](../../../concepts/delta_query_overview.md) to track incremental additions, deletions, and updates, by providing a [delta](../api/mailfolder_delta.md) function.</span></span>

<span data-ttu-id="26b25-105">**既知のフォルダー名**</span><span class="sxs-lookup"><span data-stu-id="26b25-105">**Well-known folder names**</span></span>

<span data-ttu-id="26b25-106">Outlook では、既定でユーザー用の特定のフォルダーを作成します。</span><span class="sxs-lookup"><span data-stu-id="26b25-106">Outlook creates certain folders for users by default.</span></span> <span data-ttu-id="26b25-107">対応するフォルダーの **id** 値を使用する代わりに、便利なことに、これらのフォルダーにアクセスするときに、次の表から既知のフォルダー名を使用できます。</span><span class="sxs-lookup"><span data-stu-id="26b25-107">Instead of using the corresponding folder id value, for convenience, you can use the following well-known folder names when accessing these folders in a mailFolder collection: , , , , , , , and .</span></span> <span data-ttu-id="26b25-108">たとえば、次のクエリで、既知の名前を使用して、[下書き] フォルダーを取得できます。</span><span class="sxs-lookup"><span data-stu-id="26b25-108">For example, you can get the Drafts folder using its well-known name with the following query.</span></span>

<!-- { "blockType": "ignored" } -->
```http
GET /me/mailFolders/drafts
```

<span data-ttu-id="26b25-109">既知の名前は、ユーザーのメールボックスのロケールに関係なく機能します。そのため、上記のクエリは、命名方法に関わらず、常にユーザーの [下書き] フォルダーを返します。</span><span class="sxs-lookup"><span data-stu-id="26b25-109">Well-known names work regardless of the locale of the user's mailbox, so the above query will always return the user's Drafts folder regardless of how it is named.</span></span>

| <span data-ttu-id="26b25-110">既知のフォルダー名</span><span class="sxs-lookup"><span data-stu-id="26b25-110">Well-known folder name</span></span> | <span data-ttu-id="26b25-111">説明</span><span class="sxs-lookup"><span data-stu-id="26b25-111">Description</span></span> |
|:-----------------------|:------------|
| <span data-ttu-id="26b25-112">archive</span><span class="sxs-lookup"><span data-stu-id="26b25-112">Archive</span></span> | <span data-ttu-id="26b25-113">archive フォルダーのメッセージは、"ワンクリックでアーカイブ" (クイックアーカイブ) 機能をサポートしている Outlook クライアントでこの機能を使用すると送信されます。</span><span class="sxs-lookup"><span data-stu-id="26b25-113">The archive folder messages are sent to when using the One_Click Archive feature in Outlook clients that support it.</span></span> <span data-ttu-id="26b25-114">**注:** これは Exchange Online のアーカイブ メールボックス機能とは異なります。</span><span class="sxs-lookup"><span data-stu-id="26b25-114">**Note:** this is not the same as the Archive Mailbox feature of Exchange online.</span></span> |
| <span data-ttu-id="26b25-115">clutter</span><span class="sxs-lookup"><span data-stu-id="26b25-115">Clutter</span></span> | <span data-ttu-id="26b25-116">[低優先メール] フォルダーの優先順位の低いメッセージは、低優先メール機能を使用すると移動されます。</span><span class="sxs-lookup"><span data-stu-id="26b25-116">The clutter folder low-priority messages are moved to when using the Clutter feature.</span></span> |
| <span data-ttu-id="26b25-117">conflicts</span><span class="sxs-lookup"><span data-stu-id="26b25-117">Conflicts</span></span> | <span data-ttu-id="26b25-118">メールボックスにある競合アイテムを含むフォルダーです。</span><span class="sxs-lookup"><span data-stu-id="26b25-118">The folder that contains conflicting items in the mailbox.</span></span> |
| <span data-ttu-id="26b25-119">conversationhistory</span><span class="sxs-lookup"><span data-stu-id="26b25-119">conversationhistory</span></span> | <span data-ttu-id="26b25-120"> (Skype がこの動作を実行するように構成されている場合) Skype が IM での会話を保存するフォルダーです。</span><span class="sxs-lookup"><span data-stu-id="26b25-120">The folder where Skype saves IM conversations (if Skype is configured to do so).</span></span> |
| <span data-ttu-id="26b25-121">deleteditems</span><span class="sxs-lookup"><span data-stu-id="26b25-121">deleteditems</span></span> | <span data-ttu-id="26b25-122">フォルダーのアイテムは削除時に移動されます。</span><span class="sxs-lookup"><span data-stu-id="26b25-122">The folder items are moved to when they are deleted.</span></span> |
| <span data-ttu-id="26b25-123">drafts</span><span class="sxs-lookup"><span data-stu-id="26b25-123">drafts</span></span> | <span data-ttu-id="26b25-124">未送信のメッセージを含むフォルダーです。</span><span class="sxs-lookup"><span data-stu-id="26b25-124">The folder that contains unsent messages.</span></span> |
| <span data-ttu-id="26b25-125">inbox</span><span class="sxs-lookup"><span data-stu-id="26b25-125">Inbox</span></span> | <span data-ttu-id="26b25-126">受信トレイのフォルダーです。</span><span class="sxs-lookup"><span data-stu-id="26b25-126">The Inbox folder.</span></span> |
| <span data-ttu-id="26b25-127">junkemail</span><span class="sxs-lookup"><span data-stu-id="26b25-127">junkemail</span></span> | <span data-ttu-id="26b25-128">迷惑メールのフォルダーです。</span><span class="sxs-lookup"><span data-stu-id="26b25-128">The Junk E-Mail folder.</span></span> |
| <span data-ttu-id="26b25-129">localfailures</span><span class="sxs-lookup"><span data-stu-id="26b25-129">localfailures</span></span> | <span data-ttu-id="26b25-130">ローカル クライアント上に存在するが、サーバーにアップロードできなかったアイテムを含むフォルダーです。</span><span class="sxs-lookup"><span data-stu-id="26b25-130">The folder that contains items that exist on the local client but could not be uploaded to the server.</span></span> |
| <span data-ttu-id="26b25-131">msgfolderroot</span><span class="sxs-lookup"><span data-stu-id="26b25-131">msgfolderroot</span></span> | <span data-ttu-id="26b25-132">"インフォメーション ストアの最上位" のフォルダーです。</span><span class="sxs-lookup"><span data-stu-id="26b25-132">The "Top of Information Store" folder.</span></span> <span data-ttu-id="26b25-133">このフォルダーは、受信トレイなど、通常のメール クライアントで表示されているフォルダーの親フォルダーです。</span><span class="sxs-lookup"><span data-stu-id="26b25-133">This folder is the parent folder for folders that are displayed in normal mail clients, such as the inbox.</span></span> |
| <span data-ttu-id="26b25-134">outbox</span><span class="sxs-lookup"><span data-stu-id="26b25-134">Outbox</span></span> | <span data-ttu-id="26b25-135">送信トレイのフォルダーです。</span><span class="sxs-lookup"><span data-stu-id="26b25-135">The Outbox folder.</span></span> |
| <span data-ttu-id="26b25-136">recoverableitemsdeletions</span><span class="sxs-lookup"><span data-stu-id="26b25-136">recoverableitemsdeletions</span></span> | <span data-ttu-id="26b25-137">論理的に削除されたアイテムを含むフォルダーです。つまり、[削除済みアイテム]フォルダーから、または  Outlook で Shift キーを押しながら Delete キーを押して削除されたアイテムです。</span><span class="sxs-lookup"><span data-stu-id="26b25-137">The folder that contains soft-deleted items: deleted either from the Deleted Items folder, or by pressing shift+delete in Outlook.</span></span> <span data-ttu-id="26b25-138">このフォルダーは Outlook のメール クライアントには表示されませんが、エンドユーザーは、Outlook または Outlook on the web の **[サーバーから削除済みアイテムを復元] ** 機能を使用して、このフォルダーにアクセスできます。</span><span class="sxs-lookup"><span data-stu-id="26b25-138">This folder is not visible in any Outlook email client, but end users can interact with it through the **Recover Deleted Items from Server** feature in Outlook or Outlook on the web.</span></span> |
| <span data-ttu-id="26b25-139">scheduled</span><span class="sxs-lookup"><span data-stu-id="26b25-139">scheduled</span></span> | <span data-ttu-id="26b25-140">iOS 版 Outlook のスケジュール機能を使用して受信トレイに再表示されるようにスケジュールされているメッセージを含むフォルダーです。</span><span class="sxs-lookup"><span data-stu-id="26b25-140">The folder that contains messages that are scheduled to reappear in the inbox using the Schedule feature in Outlook for iOS.</span></span> |
| <span data-ttu-id="26b25-141">searchfolders</span><span class="sxs-lookup"><span data-stu-id="26b25-141">searchfolders</span></span> | <span data-ttu-id="26b25-142">ユーザーのメールボックスで定義されているすべての検索フォルダーの親フォルダーです。</span><span class="sxs-lookup"><span data-stu-id="26b25-142">The parent folder for all search folders defined in the user's mailbox.</span></span> |
| <span data-ttu-id="26b25-143">sentitems</span><span class="sxs-lookup"><span data-stu-id="26b25-143">sentitems</span></span> | <span data-ttu-id="26b25-144">送信済みアイテムのフォルダーです。</span><span class="sxs-lookup"><span data-stu-id="26b25-144">sent items folder</span></span> |
| <span data-ttu-id="26b25-145">serverfailures</span><span class="sxs-lookup"><span data-stu-id="26b25-145">serverfailures</span></span> | <span data-ttu-id="26b25-146">サーバー上に存在するが、ローカル クライアントに同期できなかったアイテムを含むフォルダーです。</span><span class="sxs-lookup"><span data-stu-id="26b25-146">The folder that contains items that exist on the server but could not be synchronized to the local client.</span></span> |
| <span data-ttu-id="26b25-147">syncissues</span><span class="sxs-lookup"><span data-stu-id="26b25-147">syncissues</span></span> | <span data-ttu-id="26b25-148">Outlook で作成された同期ログを含むフォルダーです。</span><span class="sxs-lookup"><span data-stu-id="26b25-148">The folder that contains synchronization logs created by Outlook.</span></span> |

## <a name="methods"></a><span data-ttu-id="26b25-149">メソッド</span><span class="sxs-lookup"><span data-stu-id="26b25-149">Methods</span></span>

| <span data-ttu-id="26b25-150">メソッド</span><span class="sxs-lookup"><span data-stu-id="26b25-150">Method</span></span> | <span data-ttu-id="26b25-151">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="26b25-151">Return Type</span></span> | <span data-ttu-id="26b25-152">説明</span><span class="sxs-lookup"><span data-stu-id="26b25-152">Description</span></span> |
|:-------|:------------|:------------|
|[<span data-ttu-id="26b25-153">mailFolder の取得</span><span class="sxs-lookup"><span data-stu-id="26b25-153">Get mailFolder</span></span>](../api/mailfolder_get.md) | [<span data-ttu-id="26b25-154">mailFolder</span><span class="sxs-lookup"><span data-stu-id="26b25-154">mailFolder</span></span>](mailfolder.md) |<span data-ttu-id="26b25-155">mailFolder オブジェクトのプロパティとリレーションシップを読み取ります。</span><span class="sxs-lookup"><span data-stu-id="26b25-155">Read properties and relationships of mailFolder object.</span></span>|
|[<span data-ttu-id="26b25-156">MailFolder の作成</span><span class="sxs-lookup"><span data-stu-id="26b25-156">Create MailFolder</span></span>](../api/mailfolder_post_childfolders.md) |[<span data-ttu-id="26b25-157">MailFolder</span><span class="sxs-lookup"><span data-stu-id="26b25-157">MailFolder</span></span>](mailfolder.md)| <span data-ttu-id="26b25-158">childFolders コレクションへの投稿により、現在の mailFolder 下に新しい mailFolder を作成します。</span><span class="sxs-lookup"><span data-stu-id="26b25-158">Create a new mailFolder under the current one by posting to the childFolders collection.</span></span>|
|[<span data-ttu-id="26b25-159">childFolders を一覧表示する</span><span class="sxs-lookup"><span data-stu-id="26b25-159">List childFolders</span></span>](../api/mailfolder_list_childfolders.md) |<span data-ttu-id="26b25-160">[MailFolder](mailfolder.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="26b25-160">[MailFolder](mailfolder.md) collection</span></span>| <span data-ttu-id="26b25-p106">指定したフォルダーの下のフォルダー コレクションを取得します。`.../me/MailFolders` ショートカットを使用すると、最上位フォルダーのコレクションを取得して、別のフォルダーに移動することができます。</span><span class="sxs-lookup"><span data-stu-id="26b25-p106">Get the folder collection under the specified folder. You can use the `.../me/MailFolders` shortcut to get the top-level folder collection and navigate to another folder.</span></span>|
|[<span data-ttu-id="26b25-163">メッセージの作成</span><span class="sxs-lookup"><span data-stu-id="26b25-163">Create Message</span></span>](../api/mailfolder_post_messages.md) |[<span data-ttu-id="26b25-164">メッセージ</span><span class="sxs-lookup"><span data-stu-id="26b25-164">Message</span></span>](message.md)| <span data-ttu-id="26b25-165">メッセージ コレクションへの投稿により、現在の mailFolder に新しいメッセージを作成します。</span><span class="sxs-lookup"><span data-stu-id="26b25-165">Create a new message in the current mailFolder by posting to the messages collection.</span></span>|
|[<span data-ttu-id="26b25-166">メッセージのリスト</span><span class="sxs-lookup"><span data-stu-id="26b25-166">List messages</span></span>](../api/mailfolder_list_messages.md) |<span data-ttu-id="26b25-167">[Message](message.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="26b25-167">[Message](message.md) collection</span></span>| <span data-ttu-id="26b25-168">サインインしているユーザーのメールボックス内のすべてのメッセージや、メールボックス内の指定したフォルダー内のメッセージを取得します。</span><span class="sxs-lookup"><span data-stu-id="26b25-168">Get all the messages in the signed-in user's mailbox, or those messages in a specified folder in the mailbox.</span></span>|
|[<span data-ttu-id="26b25-169">更新する</span><span class="sxs-lookup"><span data-stu-id="26b25-169">Update</span></span>](../api/mailfolder_update.md) | [<span data-ttu-id="26b25-170">mailFolder</span><span class="sxs-lookup"><span data-stu-id="26b25-170">mailFolder</span></span>](mailfolder.md)|<span data-ttu-id="26b25-171">指定した mailFolder オブジェクトを更新します。</span><span class="sxs-lookup"><span data-stu-id="26b25-171">Update the specified mailFolder object.</span></span> |
|[<span data-ttu-id="26b25-172">削除</span><span class="sxs-lookup"><span data-stu-id="26b25-172">Delete</span></span>](../api/mailfolder_delete.md) | <span data-ttu-id="26b25-173">なし</span><span class="sxs-lookup"><span data-stu-id="26b25-173">None</span></span> |<span data-ttu-id="26b25-174">指定した mailFolder オブジェクトを削除します。</span><span class="sxs-lookup"><span data-stu-id="26b25-174">Delete the specified mailFolder object.</span></span> |
|[<span data-ttu-id="26b25-175">コピー</span><span class="sxs-lookup"><span data-stu-id="26b25-175">copy</span></span>](../api/mailfolder_copy.md)|[<span data-ttu-id="26b25-176">MailFolder</span><span class="sxs-lookup"><span data-stu-id="26b25-176">MailFolder</span></span>](mailfolder.md)|<span data-ttu-id="26b25-177">mailFolder とその内容を別の mailFolder にコピーします。</span><span class="sxs-lookup"><span data-stu-id="26b25-177">Copy a mailFolder and its contents to another mailFolder.</span></span>|
|[<span data-ttu-id="26b25-178">デルタ</span><span class="sxs-lookup"><span data-stu-id="26b25-178">delta</span></span>](../api/mailfolder_delta.md)|<span data-ttu-id="26b25-179">[mailFolder](mailfolder.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="26b25-179">[mailFolder](mailfolder.md) collection</span></span>|<span data-ttu-id="26b25-180">ユーザーのメールボックスで追加または削除された一連のメール フォルダーを取得します。</span><span class="sxs-lookup"><span data-stu-id="26b25-180">Get a set of mail folders that have been added, deleted, or removed from the user's mailbox.</span></span>|
|[<span data-ttu-id="26b25-181">移動</span><span class="sxs-lookup"><span data-stu-id="26b25-181">move</span></span>](../api/mailfolder_move.md)|[<span data-ttu-id="26b25-182">MailFolder</span><span class="sxs-lookup"><span data-stu-id="26b25-182">MailFolder</span></span>](mailfolder.md)|<span data-ttu-id="26b25-183">mailFolder とその内容を別の mailFolder に移動します。</span><span class="sxs-lookup"><span data-stu-id="26b25-183">Move a mailFolder and its contents to another mailFolder.</span></span>|
|<span data-ttu-id="26b25-184">**拡張プロパティ**</span><span class="sxs-lookup"><span data-stu-id="26b25-184">**Extended properties**</span></span>| | |
|[<span data-ttu-id="26b25-185">単一値の拡張プロパティを作成する</span><span class="sxs-lookup"><span data-stu-id="26b25-185">Create single-value extended property</span></span>](../api/singlevaluelegacyextendedproperty_post_singlevalueextendedproperties.md) |[<span data-ttu-id="26b25-186">mailFolder</span><span class="sxs-lookup"><span data-stu-id="26b25-186">mailFolder</span></span>](mailFolder.md)  |<span data-ttu-id="26b25-187">新規または既存の mailFolder に、1 つ以上の単一値の拡張プロパティを作成します。</span><span class="sxs-lookup"><span data-stu-id="26b25-187">Create one or more single-value extended properties in a new or existing mailFolder.</span></span>   |
|[<span data-ttu-id="26b25-188">単一値の拡張プロパティを持つ mailFolder の取得</span><span class="sxs-lookup"><span data-stu-id="26b25-188">Get mailFolder with single-value extended property</span></span>](../api/singlevaluelegacyextendedproperty_get.md)  | [<span data-ttu-id="26b25-189">mailFolder</span><span class="sxs-lookup"><span data-stu-id="26b25-189">mailFolder</span></span>](mailFolder.md) | <span data-ttu-id="26b25-190">または `$filter` を使用して、単一値の拡張プロパティを含む mailFolder を取得します。`$expand`</span><span class="sxs-lookup"><span data-stu-id="26b25-190">Get mailFolders that contain a single-value extended property by using `$expand` or `$filter`.</span></span> |
|[<span data-ttu-id="26b25-191">複数値の拡張プロパティを作成する</span><span class="sxs-lookup"><span data-stu-id="26b25-191">Create multi-value extended property</span></span>](../api/multivaluelegacyextendedproperty_post_multivalueextendedproperties.md) | [<span data-ttu-id="26b25-192">mailFolder</span><span class="sxs-lookup"><span data-stu-id="26b25-192">mailFolder</span></span>](mailFolder.md) | <span data-ttu-id="26b25-193">新規または既存の mailFolder の 1 つ以上の複数値の拡張プロパティを作成します。</span><span class="sxs-lookup"><span data-stu-id="26b25-193">Create one or more multi-value extended properties in a new or existing mailFolder.</span></span>  |
|[<span data-ttu-id="26b25-194">複数値の拡張プロパティを持つ mailFolder の取得</span><span class="sxs-lookup"><span data-stu-id="26b25-194">Get mailFolder with multi-value extended property</span></span>](../api/multivaluelegacyextendedproperty_get.md)  | [<span data-ttu-id="26b25-195">mailFolder</span><span class="sxs-lookup"><span data-stu-id="26b25-195">mailFolder</span></span>](mailFolder.md) | <span data-ttu-id="26b25-196">を使用して、複数値の拡張プロパティを含む mailFolder を取得します。`$expand`</span><span class="sxs-lookup"><span data-stu-id="26b25-196">Get a mailFolder that contains a multi-value extended property by using `$expand`.</span></span> |

## <a name="properties"></a><span data-ttu-id="26b25-197">プロパティ</span><span class="sxs-lookup"><span data-stu-id="26b25-197">Properties</span></span>

| <span data-ttu-id="26b25-198">プロパティ</span><span class="sxs-lookup"><span data-stu-id="26b25-198">Property</span></span> | <span data-ttu-id="26b25-199">タイプ</span><span class="sxs-lookup"><span data-stu-id="26b25-199">Type</span></span> | <span data-ttu-id="26b25-200">説明</span><span class="sxs-lookup"><span data-stu-id="26b25-200">Description</span></span> |
|:---------|:-----|:------------|
|<span data-ttu-id="26b25-201">childFolderCount</span><span class="sxs-lookup"><span data-stu-id="26b25-201">childFolderCount</span></span>|<span data-ttu-id="26b25-202">Int32</span><span class="sxs-lookup"><span data-stu-id="26b25-202">Int32</span></span>|<span data-ttu-id="26b25-203">現在の mailFolder の直下の子 mailFolder の数。</span><span class="sxs-lookup"><span data-stu-id="26b25-203">The number of immediate child mailFolders in the current mailFolder.</span></span>|
|<span data-ttu-id="26b25-204">displayName</span><span class="sxs-lookup"><span data-stu-id="26b25-204">displayName</span></span>|<span data-ttu-id="26b25-205">文字列</span><span class="sxs-lookup"><span data-stu-id="26b25-205">String</span></span>|<span data-ttu-id="26b25-206">mailFolder の表示名。</span><span class="sxs-lookup"><span data-stu-id="26b25-206">The mailFolder's display name.</span></span>|
|<span data-ttu-id="26b25-207">id</span><span class="sxs-lookup"><span data-stu-id="26b25-207">id</span></span>|<span data-ttu-id="26b25-208">文字列</span><span class="sxs-lookup"><span data-stu-id="26b25-208">String</span></span>|<span data-ttu-id="26b25-209">MailFolder の一意の識別子です。</span><span class="sxs-lookup"><span data-stu-id="26b25-209">The unique identifier.</span></span>|
|<span data-ttu-id="26b25-210">parentFolderId</span><span class="sxs-lookup"><span data-stu-id="26b25-210">parentFolderId</span></span>|<span data-ttu-id="26b25-211">文字列</span><span class="sxs-lookup"><span data-stu-id="26b25-211">String</span></span>|<span data-ttu-id="26b25-212">mailFolder の親 mailFolder の一意識別子。</span><span class="sxs-lookup"><span data-stu-id="26b25-212">The unique identifier for the mailFolder's parent mailFolder.</span></span>|
|<span data-ttu-id="26b25-213">totalItemCount</span><span class="sxs-lookup"><span data-stu-id="26b25-213">totalItemCount</span></span>|<span data-ttu-id="26b25-214">Int32</span><span class="sxs-lookup"><span data-stu-id="26b25-214">Int32</span></span>|<span data-ttu-id="26b25-215">mailFolder に含まれるアイテムの数</span><span class="sxs-lookup"><span data-stu-id="26b25-215">The number of items in the mailFolder.</span></span>|
|<span data-ttu-id="26b25-216">unreadItemCount</span><span class="sxs-lookup"><span data-stu-id="26b25-216">unreadItemCount</span></span>|<span data-ttu-id="26b25-217">Int32</span><span class="sxs-lookup"><span data-stu-id="26b25-217">Int32</span></span>|<span data-ttu-id="26b25-218">mailFolder 内で未読としてマークされているアイテムの数。</span><span class="sxs-lookup"><span data-stu-id="26b25-218">The number of items in the mailFolder marked as unread.</span></span>|

<span data-ttu-id="26b25-219">**アイテム数を効率的に取得する**</span><span class="sxs-lookup"><span data-stu-id="26b25-219">**Access item counts efficiently**</span></span>

<span data-ttu-id="26b25-220">フォルダーの `TotalItemCount` プロパティと `UnreadItemCount` プロパティを使用すると、ファイル内の既読アイテム数を簡単に算出できます。</span><span class="sxs-lookup"><span data-stu-id="26b25-220">The `TotalItemCount` and `UnreadItemCount` properties of a folder allow you to conveniently compute the number of read items in the folder.</span></span>
<span data-ttu-id="26b25-221">これにより、大幅な遅延が発生する可能性がある次のようなクエリを回避できます。</span><span class="sxs-lookup"><span data-stu-id="26b25-221">They let you avoid queries like the following that can incur significant latency:</span></span>

```http
https://outlook.office.com/api/v1.0/me/folders/inbox/messages?$count=true&$filter=isread%20eq%20false
```

<span data-ttu-id="26b25-222">Outlook のメール フォルダーには複数の種類のアイテムを含めることができます。たとえば、受信トレイには、メール アイテムとは異なる会議出席依頼アイテムを入れることができます。</span><span class="sxs-lookup"><span data-stu-id="26b25-222">Folders in Outlook can contain more than one type of items, for example, the Inbox can contain meeting request items which are distinct from mail items. TotalItemCount and UnreadItemCount include items in a folder irrespective of their item types.</span></span> <span data-ttu-id="26b25-223">`TotalItemCount`  `UnreadItemCount` には、アイテムの種類に関係なく、[メール] フォルダー内のアイテムが含まれます。</span><span class="sxs-lookup"><span data-stu-id="26b25-223">`TotalItemCount` and `UnreadItemCount` include items in a mail folder irrespective of their item types.</span></span>

## <a name="relationships"></a><span data-ttu-id="26b25-224">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="26b25-224">Relationships</span></span>

| <span data-ttu-id="26b25-225">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="26b25-225">Relationship</span></span> | <span data-ttu-id="26b25-226">型</span><span class="sxs-lookup"><span data-stu-id="26b25-226">Type</span></span> | <span data-ttu-id="26b25-227">説明</span><span class="sxs-lookup"><span data-stu-id="26b25-227">Description</span></span> |
|:-------------|:-----|:------------|
|<span data-ttu-id="26b25-228">childFolders</span><span class="sxs-lookup"><span data-stu-id="26b25-228">childFolders</span></span>|<span data-ttu-id="26b25-229">[MailFolder](mailfolder.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="26b25-229">[MailFolder](mailfolder.md) collection</span></span>|<span data-ttu-id="26b25-230">mailFolder 内の子フォルダーのコレクション。</span><span class="sxs-lookup"><span data-stu-id="26b25-230">The collection of child folders in the mailFolder.</span></span>|
|<span data-ttu-id="26b25-231">messageRules</span><span class="sxs-lookup"><span data-stu-id="26b25-231">messageRules</span></span> | <span data-ttu-id="26b25-232">[messageRule](messagerule.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="26b25-232">[messageRule](messagerule.md) collection</span></span> | <span data-ttu-id="26b25-233">ユーザーの受信トレイ フォルダーに適用されるルールのコレクション。</span><span class="sxs-lookup"><span data-stu-id="26b25-233">The collection of rules that apply to the user's Inbox folder.</span></span> |
|<span data-ttu-id="26b25-234">messages</span><span class="sxs-lookup"><span data-stu-id="26b25-234">messages</span></span>|<span data-ttu-id="26b25-235">[Message](message.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="26b25-235">[Message](message.md) collection</span></span>|<span data-ttu-id="26b25-236">mailFolder 内のメッセージのコレクション。</span><span class="sxs-lookup"><span data-stu-id="26b25-236">The collection of messages in the mailFolder.</span></span>|
|<span data-ttu-id="26b25-237">multiValueExtendedProperties</span><span class="sxs-lookup"><span data-stu-id="26b25-237">multiValueExtendedProperties</span></span>|<span data-ttu-id="26b25-238">[multiValueLegacyExtendedProperty](multivaluelegacyextendedproperty.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="26b25-238">[multiValueLegacyExtendedProperty](multivaluelegacyextendedproperty.md) collection</span></span>| <span data-ttu-id="26b25-p109">mailFolder に対して定義された、複数値の拡張プロパティのコレクション。読み取り専用。Null 許容型。</span><span class="sxs-lookup"><span data-stu-id="26b25-p109">The collection of multi-value extended properties defined for the mailFolder. Read-only. Nullable.</span></span>|
|<span data-ttu-id="26b25-242">singleValueExtendedProperties</span><span class="sxs-lookup"><span data-stu-id="26b25-242">singleValueExtendedProperties</span></span>|<span data-ttu-id="26b25-243">[singleValueLegacyExtendedProperty](singlevaluelegacyextendedproperty.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="26b25-243">[singleValueLegacyExtendedProperty](singlevaluelegacyextendedproperty.md) collection</span></span>| <span data-ttu-id="26b25-p110">mailFolder に対して定義された、単一値の拡張プロパティのコレクションです。読み取り専用。Null 許容型。</span><span class="sxs-lookup"><span data-stu-id="26b25-p110">The collection of single-value extended properties defined for the mailFolder. Read-only. Nullable.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="26b25-247">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="26b25-247">JSON representation</span></span>

<span data-ttu-id="26b25-248">以下は、リソースの JSON 表記です</span><span class="sxs-lookup"><span data-stu-id="26b25-248">Here is a JSON representation of the resource</span></span>

<!--{
  "blockType": "resource",
  "optionalProperties": [
    "childFolders",
    "messageRules",
    "messages",
    "multiValueExtendedProperties",
    "singleValueExtendedProperties"
  ],
  "keyProperty": "id",
  "baseType": "microsoft.graph.entity",
  "@odata.type": "microsoft.graph.mailFolder",
  "@odata.annotations": [
    {
      "property": "childFolders",
      "capabilities": {
        "changeTracking": false,
        "navigability": "single",
        "searchable": false
      }
    },
    {
      "property": "messageRules",
      "capabilities": {
        "changeTracking": false,
        "expandable": false,
        "searchable": false
      }
    },
    {
      "property": "messages",
      "capabilities": {
        "changeTracking": true,
        "navigability": "single"
      }
    }
  ]
}-->

```json
{
  "childFolderCount": 1024,
  "displayName": "string",
  "id": "string (identifier)",
  "parentFolderId": "string",
  "totalItemCount": 1024,
  "unreadItemCount": 1024,
  "childFolders": [ { "@odata.type": "microsoft.graph.mailFolder" } ],
  "messageRules": [ { "@odata.type": "microsoft.graph.messageRule" } ],
  "messages": [ { "@odata.type": "microsoft.graph.message" } ],
  "multiValueExtendedProperties": [ { "@odata.type": "microsoft.graph.multiValueLegacyExtendedProperty" }],
  "singleValueExtendedProperties": [ { "@odata.type": "microsoft.graph.singleValueLegacyExtendedProperty" }]
}
```

## <a name="see-also"></a><span data-ttu-id="26b25-249">関連項目</span><span class="sxs-lookup"><span data-stu-id="26b25-249">See also</span></span>

- [<span data-ttu-id="26b25-250">デルタ クエリを使用して、Microsoft Graph データの変更を追跡する</span><span class="sxs-lookup"><span data-stu-id="26b25-250">Use delta query to track changes in Microsoft Graph data</span></span>](../../../concepts/delta_query_overview.md)
- [<span data-ttu-id="26b25-251">フォルダー内のメッセージへの増分の変更を取得する</span><span class="sxs-lookup"><span data-stu-id="26b25-251">Get incremental changes to messages in a folder</span></span>](../../../concepts/delta_query_messages.md)

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "mailFolder resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
