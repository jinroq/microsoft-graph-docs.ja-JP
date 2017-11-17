# <a name="mailfolder-resource-type"></a><span data-ttu-id="281aa-101">mailFolder リソースの種類</span><span class="sxs-lookup"><span data-stu-id="281aa-101">mailFolder resource type</span></span>

<span data-ttu-id="281aa-p101">受信トレイ、下書き、送信済みアイテムなどのユーザーのメールボックス内の mailFolder です。MailFolders にはメッセージと子 mailFolders を含めることができます。</span><span class="sxs-lookup"><span data-stu-id="281aa-p101">A mailFolder in a user's mailbox, such as Inbox, Drafts, and Sent Items. MailFolders can contain messages and child mailFolders.</span></span>

<span data-ttu-id="281aa-104">このリソースでは、[デルタ](../api/mailfolder_delta.md)関数を用意すれば、増分の追加、削除、更新に[デルタ クエリ](../../../concepts/delta_query_overview.md)を使用できます。</span><span class="sxs-lookup"><span data-stu-id="281aa-104">This resource supports using [delta query](../../../concepts/delta_query_overview.md) to track incremental additions, deletions, and updates, by providing a [delta](../api/mailfolder_delta.md) function.</span></span>

## <a name="methods"></a><span data-ttu-id="281aa-105">メソッド</span><span class="sxs-lookup"><span data-stu-id="281aa-105">Methods</span></span>

| <span data-ttu-id="281aa-106">メソッド</span><span class="sxs-lookup"><span data-stu-id="281aa-106">Method</span></span>       | <span data-ttu-id="281aa-107">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="281aa-107">Return Type</span></span>  |<span data-ttu-id="281aa-108">説明</span><span class="sxs-lookup"><span data-stu-id="281aa-108">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="281aa-109">mailFolder の取得</span><span class="sxs-lookup"><span data-stu-id="281aa-109">Get mailFolder</span></span>](../api/mailfolder_get.md) | [<span data-ttu-id="281aa-110">mailFolder</span><span class="sxs-lookup"><span data-stu-id="281aa-110">mailFolder</span></span>](mailfolder.md) |<span data-ttu-id="281aa-111">mailFolder オブジェクトのプロパティとリレーションシップを読み取ります。</span><span class="sxs-lookup"><span data-stu-id="281aa-111">Read properties and relationships of mailFolder object.</span></span>|
|[<span data-ttu-id="281aa-112">MailFolder の作成</span><span class="sxs-lookup"><span data-stu-id="281aa-112">Create MailFolder</span></span>](../api/mailfolder_post_childfolders.md) |[<span data-ttu-id="281aa-113">MailFolder</span><span class="sxs-lookup"><span data-stu-id="281aa-113">MailFolder</span></span>](mailfolder.md)| <span data-ttu-id="281aa-114">childFolders コレクションへの投稿により、現在の mailFolder 下に新しい mailFolder を作成します。</span><span class="sxs-lookup"><span data-stu-id="281aa-114">Create a new mailFolder under the current one by posting to the childFolders collection.</span></span>|
|[<span data-ttu-id="281aa-115">childFolders を一覧表示する</span><span class="sxs-lookup"><span data-stu-id="281aa-115">List childFolders</span></span>](../api/mailfolder_list_childfolders.md) |<span data-ttu-id="281aa-116">[MailFolder](mailfolder.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="281aa-116">[MailFolder](mailfolder.md) collection</span></span>| <span data-ttu-id="281aa-p102">指定したフォルダーの下のフォルダー コレクションを取得します。`.../me/MailFolders` ショートカットを使用すると、最上位フォルダーのコレクションを取得して、別のフォルダーに移動することができます。</span><span class="sxs-lookup"><span data-stu-id="281aa-p102">Get the folder collection under the specified folder. You can use the `.../me/MailFolders` shortcut to get the top-level folder collection and navigate to another folder.</span></span>|
|[<span data-ttu-id="281aa-119">メッセージの作成</span><span class="sxs-lookup"><span data-stu-id="281aa-119">Create Message</span></span>](../api/mailfolder_post_messages.md) |[<span data-ttu-id="281aa-120">Message</span><span class="sxs-lookup"><span data-stu-id="281aa-120">Message</span></span>](message.md)| <span data-ttu-id="281aa-121">メッセージ コレクションへの投稿により、現在の mailFolder に新しいメッセージを作成します。</span><span class="sxs-lookup"><span data-stu-id="281aa-121">Create a new message in the current mailFolder by posting to the messages collection.</span></span>|
|[<span data-ttu-id="281aa-122">List messages</span><span class="sxs-lookup"><span data-stu-id="281aa-122">List messages</span></span>](../api/mailfolder_list_messages.md) |<span data-ttu-id="281aa-123">[Message](message.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="281aa-123">[Message](message.md) collection</span></span>| <span data-ttu-id="281aa-124">サインインしているユーザーのメールボックス内のすべてのメッセージや、メールボックス内の指定したフォルダー内のメッセージを取得します。</span><span class="sxs-lookup"><span data-stu-id="281aa-124">Get all the messages in the signed-in user's mailbox, or those messages in a specified folder in the mailbox.</span></span>|
|[<span data-ttu-id="281aa-125">更新する</span><span class="sxs-lookup"><span data-stu-id="281aa-125">Update</span></span>](../api/mailfolder_update.md) | [<span data-ttu-id="281aa-126">mailFolder</span><span class="sxs-lookup"><span data-stu-id="281aa-126">mailFolder</span></span>](mailfolder.md)|<span data-ttu-id="281aa-127">指定した mailFolder オブジェクトを更新します。</span><span class="sxs-lookup"><span data-stu-id="281aa-127">Update the specified mailFolder object.</span></span> |
|[<span data-ttu-id="281aa-128">削除</span><span class="sxs-lookup"><span data-stu-id="281aa-128">Delete</span></span>](../api/mailfolder_delete.md) | <span data-ttu-id="281aa-129">なし</span><span class="sxs-lookup"><span data-stu-id="281aa-129">None</span></span> |<span data-ttu-id="281aa-130">指定した mailFolder オブジェクトを削除します。</span><span class="sxs-lookup"><span data-stu-id="281aa-130">Delete the specified mailFolder object.</span></span> |
|[<span data-ttu-id="281aa-131">コピー</span><span class="sxs-lookup"><span data-stu-id="281aa-131">copy</span></span>](../api/mailfolder_copy.md)|[<span data-ttu-id="281aa-132">MailFolder</span><span class="sxs-lookup"><span data-stu-id="281aa-132">MailFolder</span></span>](mailfolder.md)|<span data-ttu-id="281aa-133">mailFolder とその内容を別の mailFolder にコピーします。</span><span class="sxs-lookup"><span data-stu-id="281aa-133">Copy a mailFolder and its contents to another mailFolder.</span></span>|
|[<span data-ttu-id="281aa-134">delta</span><span class="sxs-lookup"><span data-stu-id="281aa-134">delta</span></span>](../api/mailfolder_delta.md)|<span data-ttu-id="281aa-135">[mailFolder](mailfolder.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="281aa-135">[mailFolder](mailfolder.md) collection</span></span>|<span data-ttu-id="281aa-136">ユーザーのメールボックスで追加または削除された一連のメール フォルダーを取得します。</span><span class="sxs-lookup"><span data-stu-id="281aa-136">Get a set of mail folders that have been added, deleted, or removed from the user's mailbox.</span></span>|
|[<span data-ttu-id="281aa-137">move</span><span class="sxs-lookup"><span data-stu-id="281aa-137">move</span></span>](../api/mailfolder_move.md)|[<span data-ttu-id="281aa-138">MailFolder</span><span class="sxs-lookup"><span data-stu-id="281aa-138">MailFolder</span></span>](mailfolder.md)|<span data-ttu-id="281aa-139">mailFolder とその内容を別の mailFolder に移動します。</span><span class="sxs-lookup"><span data-stu-id="281aa-139">Move a mailFolder and its contents to another mailFolder.</span></span>|
|[<span data-ttu-id="281aa-140">単一値の拡張プロパティを作成する</span><span class="sxs-lookup"><span data-stu-id="281aa-140">Create single-value extended property</span></span>](../api/singlevaluelegacyextendedproperty_post_singlevalueextendedproperties.md) |[<span data-ttu-id="281aa-141">mailFolder</span><span class="sxs-lookup"><span data-stu-id="281aa-141">mailFolder</span></span>](mailFolder.md)  |<span data-ttu-id="281aa-142">新規または既存の mailFolder に、1 つ以上の単一値の拡張プロパティを作成します。</span><span class="sxs-lookup"><span data-stu-id="281aa-142">Create one or more single-value extended properties in a new or existing mailFolder.</span></span>   |
|[<span data-ttu-id="281aa-143">単一値の拡張プロパティを持つ mailFolder の取得</span><span class="sxs-lookup"><span data-stu-id="281aa-143">Get mailFolder with single-value extended property</span></span>](../api/singlevaluelegacyextendedproperty_get.md)  | [<span data-ttu-id="281aa-144">mailFolder</span><span class="sxs-lookup"><span data-stu-id="281aa-144">mailFolder</span></span>](mailFolder.md) | <span data-ttu-id="281aa-145">`$expand` または `$filter` を使用して、単一値の拡張プロパティを含む mailFolder を取得します。</span><span class="sxs-lookup"><span data-stu-id="281aa-145">Get mailFolders that contain a single-value extended property by using `$expand` or `$filter`.</span></span> |
|[<span data-ttu-id="281aa-146">複数値の拡張プロパティを作成する</span><span class="sxs-lookup"><span data-stu-id="281aa-146">Create multi-value extended property</span></span>](../api/multivaluelegacyextendedproperty_post_multivalueextendedproperties.md) | [<span data-ttu-id="281aa-147">mailFolder</span><span class="sxs-lookup"><span data-stu-id="281aa-147">mailFolder</span></span>](mailFolder.md) | <span data-ttu-id="281aa-148">新規または既存の mailFolder の 1 つ以上の複数値の拡張プロパティを作成します。</span><span class="sxs-lookup"><span data-stu-id="281aa-148">Create one or more multi-value extended properties in a new or existing mailFolder.</span></span>  |
|[<span data-ttu-id="281aa-149">複数値の拡張プロパティを持つ mailFolder の取得</span><span class="sxs-lookup"><span data-stu-id="281aa-149">Get mailFolder with multi-value extended property</span></span>](../api/multivaluelegacyextendedproperty_get.md)  | [<span data-ttu-id="281aa-150">mailFolder</span><span class="sxs-lookup"><span data-stu-id="281aa-150">mailFolder</span></span>](mailFolder.md) | <span data-ttu-id="281aa-151">`$expand` を使用して、複数値の拡張プロパティを含む mailFolder を取得します。</span><span class="sxs-lookup"><span data-stu-id="281aa-151">Get a mailFolder that contains a multi-value extended property by using `$expand`.</span></span> |

## <a name="properties"></a><span data-ttu-id="281aa-152">プロパティ</span><span class="sxs-lookup"><span data-stu-id="281aa-152">Properties</span></span>
| <span data-ttu-id="281aa-153">プロパティ</span><span class="sxs-lookup"><span data-stu-id="281aa-153">Property</span></span>     | <span data-ttu-id="281aa-154">型</span><span class="sxs-lookup"><span data-stu-id="281aa-154">Type</span></span>   |<span data-ttu-id="281aa-155">説明</span><span class="sxs-lookup"><span data-stu-id="281aa-155">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="281aa-156">childFolderCount</span><span class="sxs-lookup"><span data-stu-id="281aa-156">childFolderCount</span></span>|<span data-ttu-id="281aa-157">Int32</span><span class="sxs-lookup"><span data-stu-id="281aa-157">Int32</span></span>|<span data-ttu-id="281aa-158">現在の mailFolder の直下の子 mailFolder の数。</span><span class="sxs-lookup"><span data-stu-id="281aa-158">The number of immediate child mailFolders in the current mailFolder.</span></span>|
|<span data-ttu-id="281aa-159">displayName</span><span class="sxs-lookup"><span data-stu-id="281aa-159">displayName</span></span>|<span data-ttu-id="281aa-160">String</span><span class="sxs-lookup"><span data-stu-id="281aa-160">String</span></span>|<span data-ttu-id="281aa-161">mailFolder の表示名。</span><span class="sxs-lookup"><span data-stu-id="281aa-161">The mailFolder's display name.</span></span>|
|<span data-ttu-id="281aa-162">id</span><span class="sxs-lookup"><span data-stu-id="281aa-162">id</span></span>|<span data-ttu-id="281aa-163">String</span><span class="sxs-lookup"><span data-stu-id="281aa-163">String</span></span>|<span data-ttu-id="281aa-p103">mailFolder の一意識別子。次の既知の名前を使用して対応するフォルダーにアクセスできます。Inbox、Drafts、SentItems、DeletedItems。</span><span class="sxs-lookup"><span data-stu-id="281aa-p103">The mailFolder's unique identifier. You can use the following well-known names to access the corresponding folder: Inbox, Drafts, SentItems, DeletedItems.</span></span>|
|<span data-ttu-id="281aa-166">parentFolderId</span><span class="sxs-lookup"><span data-stu-id="281aa-166">parentFolderId</span></span>|<span data-ttu-id="281aa-167">String</span><span class="sxs-lookup"><span data-stu-id="281aa-167">String</span></span>|<span data-ttu-id="281aa-168">mailFolder の親 mailFolder の一意識別子。</span><span class="sxs-lookup"><span data-stu-id="281aa-168">The unique identifier for the mailFolder's parent mailFolder.</span></span>|
|<span data-ttu-id="281aa-169">totalItemCount</span><span class="sxs-lookup"><span data-stu-id="281aa-169">totalItemCount</span></span>|<span data-ttu-id="281aa-170">Int32</span><span class="sxs-lookup"><span data-stu-id="281aa-170">Int32</span></span>|<span data-ttu-id="281aa-171">mailFolder に含まれるアイテムの数</span><span class="sxs-lookup"><span data-stu-id="281aa-171">The number of items in the mailFolder.</span></span>|
|<span data-ttu-id="281aa-172">unreadItemCount</span><span class="sxs-lookup"><span data-stu-id="281aa-172">unreadItemCount</span></span>|<span data-ttu-id="281aa-173">Int32</span><span class="sxs-lookup"><span data-stu-id="281aa-173">Int32</span></span>|<span data-ttu-id="281aa-174">mailFolder 内で未読としてマークされているアイテムの数。</span><span class="sxs-lookup"><span data-stu-id="281aa-174">The number of items in the mailFolder marked as unread.</span></span>|

<span data-ttu-id="281aa-175">**アイテム数を効率的に取得する**</span><span class="sxs-lookup"><span data-stu-id="281aa-175">**Access item counts efficiently**</span></span>

<span data-ttu-id="281aa-p104">フォルダーの TotalItemCount プロパティと UnreadItemCount プロパティを使用すると、ファイル内の既読アイテム数を簡単に算出できます。これにより、大幅な遅延が発生する可能性がある次のようなクエリを回避できます。</span><span class="sxs-lookup"><span data-stu-id="281aa-p104">The TotalItemCount and UnreadItemCount properties of a folder allow you to conveniently compute the number of read items in the folder. They let you avoid queries like the following that can incur significant latency:</span></span>
```
https://outlook.office.com/api/v1.0/me/folders/inbox/messages?$count=true&$filter=isread%20eq%20false
```
<span data-ttu-id="281aa-p105">Outlook 内の MailFolder には、複数の種類のアイテムを含めることができます。たとえば、受信トレイには、メール アイテムとは異なる会議出席依頼アイテムを入れることができます。TotalItemCount と UnreadItemCount には、アイテムの種類に関係なく、mailFolder 内のアイテムが含まれます。</span><span class="sxs-lookup"><span data-stu-id="281aa-p105">MailFolders in Outlook can contain more than one type of items, for example, the Inbox can contain meeting request items which are distinct from mail items. TotalItemCount and UnreadItemCount include items in a mailFolder irrespective of their item types.</span></span>


## <a name="relationships"></a><span data-ttu-id="281aa-180">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="281aa-180">Relationships</span></span>
| <span data-ttu-id="281aa-181">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="281aa-181">Relationship</span></span> | <span data-ttu-id="281aa-182">型</span><span class="sxs-lookup"><span data-stu-id="281aa-182">Type</span></span>   |<span data-ttu-id="281aa-183">説明</span><span class="sxs-lookup"><span data-stu-id="281aa-183">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="281aa-184">childFolders</span><span class="sxs-lookup"><span data-stu-id="281aa-184">childFolders</span></span>|<span data-ttu-id="281aa-185">[MailFolder](mailfolder.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="281aa-185">[MailFolder](mailfolder.md) collection</span></span>|<span data-ttu-id="281aa-186">mailFolder 内の子フォルダーのコレクション。</span><span class="sxs-lookup"><span data-stu-id="281aa-186">The collection of child folders in the mailFolder.</span></span>|
|<span data-ttu-id="281aa-187">messages</span><span class="sxs-lookup"><span data-stu-id="281aa-187">messages</span></span>|<span data-ttu-id="281aa-188">[Message](message.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="281aa-188">[Message](message.md) collection</span></span>|<span data-ttu-id="281aa-189">mailFolder 内のメッセージのコレクション。</span><span class="sxs-lookup"><span data-stu-id="281aa-189">The collection of messages in the mailFolder.</span></span>|
|<span data-ttu-id="281aa-190">multiValueExtendedProperties</span><span class="sxs-lookup"><span data-stu-id="281aa-190">multiValueExtendedProperties</span></span>|<span data-ttu-id="281aa-191">[multiValueLegacyExtendedProperty](multivaluelegacyextendedproperty.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="281aa-191">[multiValueLegacyExtendedProperty](multivaluelegacyextendedproperty.md) collection</span></span>| <span data-ttu-id="281aa-p106">mailFolder に対して定義された、複数値の拡張プロパティのコレクション。読み取り専用。Null 許容型。</span><span class="sxs-lookup"><span data-stu-id="281aa-p106">The collection of multi-value extended properties defined for the mailFolder. Read-only. Nullable.</span></span>|
|<span data-ttu-id="281aa-195">singleValueExtendedProperties</span><span class="sxs-lookup"><span data-stu-id="281aa-195">singleValueExtendedProperties</span></span>|<span data-ttu-id="281aa-196">[singleValueLegacyExtendedProperty](singlevaluelegacyextendedproperty.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="281aa-196">[singleValueLegacyExtendedProperty](singlevaluelegacyextendedproperty.md) collection</span></span>| <span data-ttu-id="281aa-p107">mailFolder に対して定義された、単一値の拡張プロパティのコレクションです。読み取り専用。Null 許容型。</span><span class="sxs-lookup"><span data-stu-id="281aa-p107">The collection of single-value extended properties defined for the mailFolder. Read-only. Nullable.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="281aa-200">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="281aa-200">JSON representation</span></span>

<span data-ttu-id="281aa-201">以下は、リソースの JSON 表記です</span><span class="sxs-lookup"><span data-stu-id="281aa-201">Here is a JSON representation of the resource</span></span>

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

## <a name="see-also"></a><span data-ttu-id="281aa-202">関連項目</span><span class="sxs-lookup"><span data-stu-id="281aa-202">See also</span></span>

- [<span data-ttu-id="281aa-203">デルタ クエリを使用して、Microsoft Graph データの変更を追跡する</span><span class="sxs-lookup"><span data-stu-id="281aa-203">Use delta query to track changes in Microsoft Graph data</span></span>](../../../concepts/delta_query_overview.md)
- [<span data-ttu-id="281aa-204">フォルダー内のメッセージへの増分の変更を取得する</span><span class="sxs-lookup"><span data-stu-id="281aa-204">Get incremental changes to messages in a folder</span></span>](../../../concepts/delta_query_messages.md)


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "mailFolder resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
