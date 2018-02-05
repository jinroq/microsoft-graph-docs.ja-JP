# <a name="mailfolder-resource-type"></a><span data-ttu-id="d1346-101">mailFolder リソースの種類</span><span class="sxs-lookup"><span data-stu-id="d1346-101">mailFolder resource type</span></span>

<span data-ttu-id="d1346-102">受信トレイや下書きなどの、ユーザーのメールボックス内のメール フォルダーです。</span><span class="sxs-lookup"><span data-stu-id="d1346-102">A folder in a user's mailbox, such as Inbox, Drafts, and Sent Items.</span></span> <span data-ttu-id="d1346-103">メール フォルダーには、メッセージ、他の Outlook アイテム、子メール フォルダーを含めることができます。</span><span class="sxs-lookup"><span data-stu-id="d1346-103">Mail folders can contain messages, other Outlook items, and child mail folders.</span></span>

<span data-ttu-id="d1346-104">Outlook では、既定でユーザー用の特定のフォルダーを作成します。</span><span class="sxs-lookup"><span data-stu-id="d1346-104">Outlook creates certain folders for users by default.</span></span> <span data-ttu-id="d1346-105">対応するフォルダーの **id** 値の代わりに、便宜のために、既知のフォルダー名 (`ArchiveRoot`、`ConversationHistory`、`DeletedItems`、`Drafts`、`Inbox`、`JunkEmail`、`Outbox`、`SentItems`) を使用して、**mailFolder** コレクションのフォルダーにアクセスすることができます。</span><span class="sxs-lookup"><span data-stu-id="d1346-105">Instead of using the corresponding folder **id** value, for convenience, you can use the following well-known folder names when accessing these folders in a **mailFolder** collection: `ArchiveRoot`, `ConversationHistory`, `DeletedItems`, `Drafts`, `Inbox`, `JunkEmail`, `Outbox`, and `SentItems`.</span></span>

<span data-ttu-id="d1346-106">このリソースでは、[デルタ](../api/mailfolder_delta.md)関数を用意すれば、増分の追加、削除、更新に[デルタ クエリ](../../../concepts/delta_query_overview.md)を使用できます。</span><span class="sxs-lookup"><span data-stu-id="d1346-106">This resource supports using [delta query](../../../concepts/delta_query_overview.md) to track incremental additions, deletions, and updates, by providing a [delta](../api/mailfolder_delta.md) function.</span></span>

## <a name="methods"></a><span data-ttu-id="d1346-107">メソッド</span><span class="sxs-lookup"><span data-stu-id="d1346-107">Methods</span></span>

| <span data-ttu-id="d1346-108">メソッド</span><span class="sxs-lookup"><span data-stu-id="d1346-108">Method</span></span>       | <span data-ttu-id="d1346-109">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="d1346-109">Return Type</span></span>  |<span data-ttu-id="d1346-110">説明</span><span class="sxs-lookup"><span data-stu-id="d1346-110">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="d1346-111">mailFolder の取得</span><span class="sxs-lookup"><span data-stu-id="d1346-111">Get mailFolder</span></span>](../api/mailfolder_get.md) | [<span data-ttu-id="d1346-112">mailFolder</span><span class="sxs-lookup"><span data-stu-id="d1346-112">mailFolder</span></span>](mailfolder.md) |<span data-ttu-id="d1346-113">mailFolder オブジェクトのプロパティとリレーションシップを読み取ります。</span><span class="sxs-lookup"><span data-stu-id="d1346-113">Read properties and relationships of mailFolder object.</span></span>|
|[<span data-ttu-id="d1346-114">MailFolder の作成</span><span class="sxs-lookup"><span data-stu-id="d1346-114">Create MailFolder</span></span>](../api/mailfolder_post_childfolders.md) |[<span data-ttu-id="d1346-115">MailFolder</span><span class="sxs-lookup"><span data-stu-id="d1346-115">MailFolder</span></span>](mailfolder.md)| <span data-ttu-id="d1346-116">childFolders コレクションへの投稿により、現在の mailFolder 下に新しい mailFolder を作成します。</span><span class="sxs-lookup"><span data-stu-id="d1346-116">Create a new mailFolder under the current one by posting to the childFolders collection.</span></span>|
|[<span data-ttu-id="d1346-117">childFolders を一覧表示する</span><span class="sxs-lookup"><span data-stu-id="d1346-117">List childFolders</span></span>](../api/mailfolder_list_childfolders.md) |<span data-ttu-id="d1346-118">[MailFolder](mailfolder.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="d1346-118">[MailFolder](mailfolder.md) collection</span></span>| <span data-ttu-id="d1346-p103">指定したフォルダーの下のフォルダー コレクションを取得します。`.../me/MailFolders` ショートカットを使用すると、最上位フォルダーのコレクションを取得して、別のフォルダーに移動することができます。</span><span class="sxs-lookup"><span data-stu-id="d1346-p103">Get the folder collection under the specified folder. You can use the `.../me/MailFolders` shortcut to get the top-level folder collection and navigate to another folder.</span></span>|
|[<span data-ttu-id="d1346-121">メッセージの作成</span><span class="sxs-lookup"><span data-stu-id="d1346-121">Create Message</span></span>](../api/mailfolder_post_messages.md) |[<span data-ttu-id="d1346-122">Message</span><span class="sxs-lookup"><span data-stu-id="d1346-122">Message</span></span>](message.md)| <span data-ttu-id="d1346-123">メッセージ コレクションへの投稿により、現在の mailFolder に新しいメッセージを作成します。</span><span class="sxs-lookup"><span data-stu-id="d1346-123">Create a new message in the current mailFolder by posting to the messages collection.</span></span>|
|[<span data-ttu-id="d1346-124">List messages</span><span class="sxs-lookup"><span data-stu-id="d1346-124">List messages</span></span>](../api/mailfolder_list_messages.md) |<span data-ttu-id="d1346-125">[Message](message.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="d1346-125">[Message](message.md) collection</span></span>| <span data-ttu-id="d1346-126">サインインしているユーザーのメールボックス内のすべてのメッセージや、メールボックス内の指定したフォルダー内のメッセージを取得します。</span><span class="sxs-lookup"><span data-stu-id="d1346-126">Get all the messages in the signed-in user's mailbox, or those messages in a specified folder in the mailbox.</span></span>|
|[<span data-ttu-id="d1346-127">更新する</span><span class="sxs-lookup"><span data-stu-id="d1346-127">Update</span></span>](../api/mailfolder_update.md) | [<span data-ttu-id="d1346-128">mailFolder</span><span class="sxs-lookup"><span data-stu-id="d1346-128">mailFolder</span></span>](mailfolder.md)|<span data-ttu-id="d1346-129">指定した mailFolder オブジェクトを更新します。</span><span class="sxs-lookup"><span data-stu-id="d1346-129">Update the specified mailFolder object.</span></span> |
|[<span data-ttu-id="d1346-130">削除</span><span class="sxs-lookup"><span data-stu-id="d1346-130">Delete</span></span>](../api/mailfolder_delete.md) | <span data-ttu-id="d1346-131">なし</span><span class="sxs-lookup"><span data-stu-id="d1346-131">None</span></span> |<span data-ttu-id="d1346-132">指定した mailFolder オブジェクトを削除します。</span><span class="sxs-lookup"><span data-stu-id="d1346-132">Delete the specified mailFolder object.</span></span> |
|[<span data-ttu-id="d1346-133">コピー</span><span class="sxs-lookup"><span data-stu-id="d1346-133">copy</span></span>](../api/mailfolder_copy.md)|[<span data-ttu-id="d1346-134">MailFolder</span><span class="sxs-lookup"><span data-stu-id="d1346-134">MailFolder</span></span>](mailfolder.md)|<span data-ttu-id="d1346-135">mailFolder とその内容を別の mailFolder にコピーします。</span><span class="sxs-lookup"><span data-stu-id="d1346-135">Copy a mailFolder and its contents to another mailFolder.</span></span>|
|[<span data-ttu-id="d1346-136">delta</span><span class="sxs-lookup"><span data-stu-id="d1346-136">delta</span></span>](../api/mailfolder_delta.md)|<span data-ttu-id="d1346-137">[mailFolder](mailfolder.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="d1346-137">[mailFolder](mailfolder.md) collection</span></span>|<span data-ttu-id="d1346-138">ユーザーのメールボックスで追加または削除された一連のメール フォルダーを取得します。</span><span class="sxs-lookup"><span data-stu-id="d1346-138">Get a set of mail folders that have been added, deleted, or removed from the user's mailbox.</span></span>|
|[<span data-ttu-id="d1346-139">move</span><span class="sxs-lookup"><span data-stu-id="d1346-139">move</span></span>](../api/mailfolder_move.md)|[<span data-ttu-id="d1346-140">MailFolder</span><span class="sxs-lookup"><span data-stu-id="d1346-140">MailFolder</span></span>](mailfolder.md)|<span data-ttu-id="d1346-141">mailFolder とその内容を別の mailFolder に移動します。</span><span class="sxs-lookup"><span data-stu-id="d1346-141">Move a mailFolder and its contents to another mailFolder.</span></span>|
|[<span data-ttu-id="d1346-142">単一値の拡張プロパティを作成する</span><span class="sxs-lookup"><span data-stu-id="d1346-142">Create single-value extended property</span></span>](../api/singlevaluelegacyextendedproperty_post_singlevalueextendedproperties.md) |[<span data-ttu-id="d1346-143">mailFolder</span><span class="sxs-lookup"><span data-stu-id="d1346-143">mailFolder</span></span>](mailFolder.md)  |<span data-ttu-id="d1346-144">新規または既存の mailFolder に、1 つ以上の単一値の拡張プロパティを作成します。</span><span class="sxs-lookup"><span data-stu-id="d1346-144">Create one or more single-value extended properties in a new or existing mailFolder.</span></span>   |
|[<span data-ttu-id="d1346-145">単一値の拡張プロパティを持つ mailFolder の取得</span><span class="sxs-lookup"><span data-stu-id="d1346-145">Get mailFolder with single-value extended property</span></span>](../api/singlevaluelegacyextendedproperty_get.md)  | [<span data-ttu-id="d1346-146">mailFolder</span><span class="sxs-lookup"><span data-stu-id="d1346-146">mailFolder</span></span>](mailFolder.md) | <span data-ttu-id="d1346-147">`$expand` または `$filter` を使用して、単一値の拡張プロパティを含む mailFolder を取得します。</span><span class="sxs-lookup"><span data-stu-id="d1346-147">Get mailFolders that contain a single-value extended property by using `$expand` or `$filter`.</span></span> |
|[<span data-ttu-id="d1346-148">複数値の拡張プロパティを作成する</span><span class="sxs-lookup"><span data-stu-id="d1346-148">Create multi-value extended property</span></span>](../api/multivaluelegacyextendedproperty_post_multivalueextendedproperties.md) | [<span data-ttu-id="d1346-149">mailFolder</span><span class="sxs-lookup"><span data-stu-id="d1346-149">mailFolder</span></span>](mailFolder.md) | <span data-ttu-id="d1346-150">新規または既存の mailFolder の 1 つ以上の複数値の拡張プロパティを作成します。</span><span class="sxs-lookup"><span data-stu-id="d1346-150">Create one or more multi-value extended properties in a new or existing mailFolder.</span></span>  |
|[<span data-ttu-id="d1346-151">複数値の拡張プロパティを持つ mailFolder の取得</span><span class="sxs-lookup"><span data-stu-id="d1346-151">Get mailFolder with multi-value extended property</span></span>](../api/multivaluelegacyextendedproperty_get.md)  | [<span data-ttu-id="d1346-152">mailFolder</span><span class="sxs-lookup"><span data-stu-id="d1346-152">mailFolder</span></span>](mailFolder.md) | <span data-ttu-id="d1346-153">`$expand` を使用して、複数値の拡張プロパティを含む mailFolder を取得します。</span><span class="sxs-lookup"><span data-stu-id="d1346-153">Get a mailFolder that contains a multi-value extended property by using `$expand`.</span></span> |

## <a name="properties"></a><span data-ttu-id="d1346-154">プロパティ</span><span class="sxs-lookup"><span data-stu-id="d1346-154">Properties</span></span>
| <span data-ttu-id="d1346-155">プロパティ</span><span class="sxs-lookup"><span data-stu-id="d1346-155">Property</span></span>     | <span data-ttu-id="d1346-156">型</span><span class="sxs-lookup"><span data-stu-id="d1346-156">Type</span></span>   |<span data-ttu-id="d1346-157">説明</span><span class="sxs-lookup"><span data-stu-id="d1346-157">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="d1346-158">childFolderCount</span><span class="sxs-lookup"><span data-stu-id="d1346-158">childFolderCount</span></span>|<span data-ttu-id="d1346-159">Int32</span><span class="sxs-lookup"><span data-stu-id="d1346-159">Int32</span></span>|<span data-ttu-id="d1346-160">現在の mailFolder の直下の子 mailFolder の数。</span><span class="sxs-lookup"><span data-stu-id="d1346-160">The number of immediate child mailFolders in the current mailFolder.</span></span>|
|<span data-ttu-id="d1346-161">displayName</span><span class="sxs-lookup"><span data-stu-id="d1346-161">displayName</span></span>|<span data-ttu-id="d1346-162">String</span><span class="sxs-lookup"><span data-stu-id="d1346-162">String</span></span>|<span data-ttu-id="d1346-163">mailFolder の表示名。</span><span class="sxs-lookup"><span data-stu-id="d1346-163">The mailFolder's display name.</span></span>|
|<span data-ttu-id="d1346-164">id</span><span class="sxs-lookup"><span data-stu-id="d1346-164">id</span></span>|<span data-ttu-id="d1346-165">String</span><span class="sxs-lookup"><span data-stu-id="d1346-165">String</span></span>|<span data-ttu-id="d1346-p104">mailFolder の一意識別子。次の既知の名前を使用して対応するフォルダーにアクセスできます。Inbox、Drafts、SentItems、DeletedItems。</span><span class="sxs-lookup"><span data-stu-id="d1346-p104">The mailFolder's unique identifier. You can use the following well-known names to access the corresponding folder: Inbox, Drafts, SentItems, DeletedItems.</span></span>|
|<span data-ttu-id="d1346-168">parentFolderId</span><span class="sxs-lookup"><span data-stu-id="d1346-168">parentFolderId</span></span>|<span data-ttu-id="d1346-169">String</span><span class="sxs-lookup"><span data-stu-id="d1346-169">String</span></span>|<span data-ttu-id="d1346-170">mailFolder の親 mailFolder の一意識別子。</span><span class="sxs-lookup"><span data-stu-id="d1346-170">The unique identifier for the mailFolder's parent mailFolder.</span></span>|
|<span data-ttu-id="d1346-171">totalItemCount</span><span class="sxs-lookup"><span data-stu-id="d1346-171">totalItemCount</span></span>|<span data-ttu-id="d1346-172">Int32</span><span class="sxs-lookup"><span data-stu-id="d1346-172">Int32</span></span>|<span data-ttu-id="d1346-173">mailFolder に含まれるアイテムの数</span><span class="sxs-lookup"><span data-stu-id="d1346-173">The number of items in the mailFolder.</span></span>|
|<span data-ttu-id="d1346-174">unreadItemCount</span><span class="sxs-lookup"><span data-stu-id="d1346-174">unreadItemCount</span></span>|<span data-ttu-id="d1346-175">Int32</span><span class="sxs-lookup"><span data-stu-id="d1346-175">Int32</span></span>|<span data-ttu-id="d1346-176">mailFolder 内で未読としてマークされているアイテムの数。</span><span class="sxs-lookup"><span data-stu-id="d1346-176">The number of items in the mailFolder marked as unread.</span></span>|

<span data-ttu-id="d1346-177">**アイテム数を効率的に取得する**</span><span class="sxs-lookup"><span data-stu-id="d1346-177">**Access item counts efficiently**</span></span>

<span data-ttu-id="d1346-p105">フォルダーの TotalItemCount プロパティと UnreadItemCount プロパティを使用すると、ファイル内の既読アイテム数を簡単に算出できます。これにより、大幅な遅延が発生する可能性がある次のようなクエリを回避できます。</span><span class="sxs-lookup"><span data-stu-id="d1346-p105">The TotalItemCount and UnreadItemCount properties of a folder allow you to conveniently compute the number of read items in the folder. They let you avoid queries like the following that can incur significant latency:</span></span>
```
https://outlook.office.com/api/v1.0/me/folders/inbox/messages?$count=true&$filter=isread%20eq%20false
```
<span data-ttu-id="d1346-p106">Outlook 内の MailFolder には、複数の種類のアイテムを含めることができます。たとえば、受信トレイには、メール アイテムとは異なる会議出席依頼アイテムを入れることができます。TotalItemCount と UnreadItemCount には、アイテムの種類に関係なく、mailFolder 内のアイテムが含まれます。</span><span class="sxs-lookup"><span data-stu-id="d1346-p106">MailFolders in Outlook can contain more than one type of items, for example, the Inbox can contain meeting request items which are distinct from mail items. TotalItemCount and UnreadItemCount include items in a mailFolder irrespective of their item types.</span></span>


## <a name="relationships"></a><span data-ttu-id="d1346-182">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="d1346-182">Relationships</span></span>
| <span data-ttu-id="d1346-183">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="d1346-183">Relationship</span></span> | <span data-ttu-id="d1346-184">型</span><span class="sxs-lookup"><span data-stu-id="d1346-184">Type</span></span>   |<span data-ttu-id="d1346-185">説明</span><span class="sxs-lookup"><span data-stu-id="d1346-185">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="d1346-186">childFolders</span><span class="sxs-lookup"><span data-stu-id="d1346-186">childFolders</span></span>|<span data-ttu-id="d1346-187">[MailFolder](mailfolder.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="d1346-187">[MailFolder](mailfolder.md) collection</span></span>|<span data-ttu-id="d1346-188">mailFolder 内の子フォルダーのコレクション。</span><span class="sxs-lookup"><span data-stu-id="d1346-188">The collection of child folders in the mailFolder.</span></span>|
|<span data-ttu-id="d1346-189">messages</span><span class="sxs-lookup"><span data-stu-id="d1346-189">messages</span></span>|<span data-ttu-id="d1346-190">[Message](message.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="d1346-190">[Message](message.md) collection</span></span>|<span data-ttu-id="d1346-191">mailFolder 内のメッセージのコレクション。</span><span class="sxs-lookup"><span data-stu-id="d1346-191">The collection of messages in the mailFolder.</span></span>|
|<span data-ttu-id="d1346-192">multiValueExtendedProperties</span><span class="sxs-lookup"><span data-stu-id="d1346-192">multiValueExtendedProperties</span></span>|<span data-ttu-id="d1346-193">[multiValueLegacyExtendedProperty](multivaluelegacyextendedproperty.md) collection</span><span class="sxs-lookup"><span data-stu-id="d1346-193">[multiValueLegacyExtendedProperty](multivaluelegacyextendedproperty.md) collection</span></span>| <span data-ttu-id="d1346-p107">mailFolder に対して定義された、複数値の拡張プロパティのコレクション。読み取り専用。Null 許容型。</span><span class="sxs-lookup"><span data-stu-id="d1346-p107">The collection of multi-value extended properties defined for the mailFolder. Read-only. Nullable.</span></span>|
|<span data-ttu-id="d1346-197">singleValueExtendedProperties</span><span class="sxs-lookup"><span data-stu-id="d1346-197">singleValueExtendedProperties</span></span>|<span data-ttu-id="d1346-198">[singleValueLegacyExtendedProperty](singlevaluelegacyextendedproperty.md) collection</span><span class="sxs-lookup"><span data-stu-id="d1346-198">[singleValueLegacyExtendedProperty](singlevaluelegacyextendedproperty.md) collection</span></span>| <span data-ttu-id="d1346-p108">mailFolder に対して定義された、単一値の拡張プロパティのコレクションです。読み取り専用。Null 許容型。</span><span class="sxs-lookup"><span data-stu-id="d1346-p108">The collection of single-value extended properties defined for the mailFolder. Read-only. Nullable.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="d1346-202">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="d1346-202">JSON representation</span></span>

<span data-ttu-id="d1346-203">以下は、リソースの JSON 表記です</span><span class="sxs-lookup"><span data-stu-id="d1346-203">Here is a JSON representation of the resource</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [
    "childFolders",
    "messages",
    "multiValueExtendedProperties",
    "singleValueExtendedProperties"
  ],
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.mailFolder"
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
  "messages": [ { "@odata.type": "microsoft.graph.message" } ],
  "multiValueExtendedProperties": [ { "@odata.type": "microsoft.graph.multiValueLegacyExtendedProperty" }],
  "singleValueExtendedProperties": [ { "@odata.type": "microsoft.graph.singleValueLegacyExtendedProperty" }]
}

```

## <a name="see-also"></a><span data-ttu-id="d1346-204">関連項目</span><span class="sxs-lookup"><span data-stu-id="d1346-204">See also</span></span>

- [<span data-ttu-id="d1346-205">デルタ クエリを使用して、Microsoft Graph データの変更を追跡する</span><span class="sxs-lookup"><span data-stu-id="d1346-205">Use delta query to track changes in Microsoft Graph data</span></span>](../../../concepts/delta_query_overview.md)
- [<span data-ttu-id="d1346-206">フォルダー内のメッセージへの増分の変更を取得する</span><span class="sxs-lookup"><span data-stu-id="d1346-206">Get incremental changes to messages in a folder</span></span>](../../../concepts/delta_query_messages.md)


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "mailFolder resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
