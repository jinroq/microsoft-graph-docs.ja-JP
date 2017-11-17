# <a name="contactfolder-resource-type"></a><span data-ttu-id="41e1d-101">contactFolder リソース型</span><span class="sxs-lookup"><span data-stu-id="41e1d-101">contactFolder resource type</span></span>

<span data-ttu-id="41e1d-102">連絡先が格納されたフォルダーです。</span><span class="sxs-lookup"><span data-stu-id="41e1d-102">A folder that contains contacts.</span></span>

<span data-ttu-id="41e1d-103">このリソースでは、[デルタ](../api/contactfolder_delta.md)関数を用意すれば、増分の追加、削除、更新に[デルタ クエリ](../../../concepts/delta_query_overview.md)を使用できます。</span><span class="sxs-lookup"><span data-stu-id="41e1d-103">This resource supports using [delta query](../../../concepts/delta_query_overview.md) to track incremental additions, deletions, and updates, by providing a [delta](../api/contactfolder_delta.md) function.</span></span>


## <a name="methods"></a><span data-ttu-id="41e1d-104">メソッド</span><span class="sxs-lookup"><span data-stu-id="41e1d-104">Methods</span></span>

| <span data-ttu-id="41e1d-105">メソッド</span><span class="sxs-lookup"><span data-stu-id="41e1d-105">Method</span></span>       | <span data-ttu-id="41e1d-106">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="41e1d-106">Return Type</span></span>  |<span data-ttu-id="41e1d-107">説明</span><span class="sxs-lookup"><span data-stu-id="41e1d-107">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="41e1d-108">contactFolder を取得する</span><span class="sxs-lookup"><span data-stu-id="41e1d-108">Get contactFolder</span></span>](../api/contactfolder_get.md) | [<span data-ttu-id="41e1d-109">contactFolder</span><span class="sxs-lookup"><span data-stu-id="41e1d-109">contactFolder</span></span>](contactfolder.md) |<span data-ttu-id="41e1d-110">連絡先フォルダー ID を使用して連絡先フォルダーを取得します。</span><span class="sxs-lookup"><span data-stu-id="41e1d-110">Get a contact folder by using the contact folder ID.</span></span>|
|[<span data-ttu-id="41e1d-111">更新する</span><span class="sxs-lookup"><span data-stu-id="41e1d-111">Update</span></span>](../api/contactfolder_update.md) | [<span data-ttu-id="41e1d-112">contactFolder</span><span class="sxs-lookup"><span data-stu-id="41e1d-112">contactFolder</span></span>](contactfolder.md) |<span data-ttu-id="41e1d-113">contactFolder オブジェクトを更新します。</span><span class="sxs-lookup"><span data-stu-id="41e1d-113">Update contactFolder object.</span></span> |
|[<span data-ttu-id="41e1d-114">削除</span><span class="sxs-lookup"><span data-stu-id="41e1d-114">Delete</span></span>](../api/contactfolder_delete.md) | <span data-ttu-id="41e1d-115">なし</span><span class="sxs-lookup"><span data-stu-id="41e1d-115">None</span></span> |<span data-ttu-id="41e1d-116">contactFolder オブジェクトを削除します。</span><span class="sxs-lookup"><span data-stu-id="41e1d-116">Delete contactFolder object.</span></span> |
|[<span data-ttu-id="41e1d-117">childFolders を一覧表示する</span><span class="sxs-lookup"><span data-stu-id="41e1d-117">List childFolders</span></span>](../api/contactfolder_list_childfolders.md) |<span data-ttu-id="41e1d-118">[ContactFolder](contactfolder.md) collection</span><span class="sxs-lookup"><span data-stu-id="41e1d-118">[ContactFolder](contactfolder.md) collection</span></span>| <span data-ttu-id="41e1d-119">指定した連絡先フォルダーの下の子フォルダーのコレクションを取得します。</span><span class="sxs-lookup"><span data-stu-id="41e1d-119">Get a collection of child folders under the specified contact folder.</span></span>|
|[<span data-ttu-id="41e1d-120">子 contactFolder を作成する</span><span class="sxs-lookup"><span data-stu-id="41e1d-120">Create child contactFolder</span></span>](../api/contactfolder_post_childfolders.md) |[<span data-ttu-id="41e1d-121">ContactFolder</span><span class="sxs-lookup"><span data-stu-id="41e1d-121">ContactFolder</span></span>](contactfolder.md)| <span data-ttu-id="41e1d-122">指定したフォルダーの子として新しい contactFolder を作成します。</span><span class="sxs-lookup"><span data-stu-id="41e1d-122">Create a new contactFolder as a child of a specified folder.</span></span>|
|[<span data-ttu-id="41e1d-123">delta</span><span class="sxs-lookup"><span data-stu-id="41e1d-123">delta</span></span>](../api/contact_delta.md)|<span data-ttu-id="41e1d-124">[contact](contact.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="41e1d-124">[contact](contact.md) collection</span></span>| <span data-ttu-id="41e1d-125">ユーザーのメールボックスで追加または削除された一連の連絡先フォルダーを取得します。</span><span class="sxs-lookup"><span data-stu-id="41e1d-125">Get a set of contact folders that have been added, deleted, or removed from the user's mailbox.</span></span>|
|[<span data-ttu-id="41e1d-126">フォルダー内の連絡先を一覧表示する</span><span class="sxs-lookup"><span data-stu-id="41e1d-126">List contacts in folder</span></span>](../api/contactfolder_list_contacts.md) |<span data-ttu-id="41e1d-127">[Contact](contact.md) collection</span><span class="sxs-lookup"><span data-stu-id="41e1d-127">[Contact](contact.md) collection</span></span>| <span data-ttu-id="41e1d-128">サインイン中のユーザーの既定の連絡先フォルダーから連絡先のコレクションを取得する (`.../me/contacts`) か、指定した連絡先フォルダーから取得します。</span><span class="sxs-lookup"><span data-stu-id="41e1d-128">Get a contact collection from the default Contacts folder of the signed-in user (`.../me/contacts`), or from the specified contact folder.</span></span>|
|[<span data-ttu-id="41e1d-129">フォルダー内に連絡先を作成する</span><span class="sxs-lookup"><span data-stu-id="41e1d-129">Create contact in folder</span></span>](../api/contactfolder_post_contacts.md) |[<span data-ttu-id="41e1d-130">Contact</span><span class="sxs-lookup"><span data-stu-id="41e1d-130">Contact</span></span>](contact.md)| <span data-ttu-id="41e1d-131">連絡先をルート連絡先フォルダーまたは別の連絡先フォルダーの `contacts` エンドポイントに追加します。</span><span class="sxs-lookup"><span data-stu-id="41e1d-131">Add a contact to the root Contacts folder or to the `contacts` endpoint of another contact folder.</span></span>|
|[<span data-ttu-id="41e1d-132">単一値の拡張プロパティを作成する</span><span class="sxs-lookup"><span data-stu-id="41e1d-132">Create single-value extended property</span></span>](../api/singlevaluelegacyextendedproperty_post_singlevalueextendedproperties.md) |[<span data-ttu-id="41e1d-133">contactFolder</span><span class="sxs-lookup"><span data-stu-id="41e1d-133">contactFolder</span></span>](contactFolder.md)  |<span data-ttu-id="41e1d-134">新規または既存の contactFolder に、1 つ以上の単一値の拡張プロパティを作成します。</span><span class="sxs-lookup"><span data-stu-id="41e1d-134">Create one or more single-value extended properties in a new or existing contactFolder.</span></span>   |
|[<span data-ttu-id="41e1d-135">単一値の拡張プロパティを持つ contactFolder を取得する</span><span class="sxs-lookup"><span data-stu-id="41e1d-135">Get contactFolder with single-value extended property</span></span>](../api/singlevaluelegacyextendedproperty_get.md)  | [<span data-ttu-id="41e1d-136">contactFolder</span><span class="sxs-lookup"><span data-stu-id="41e1d-136">contactFolder</span></span>](contactFolder.md) | <span data-ttu-id="41e1d-137">`$expand` または `$filter` を使用して、単一値の拡張プロパティを含む contactFolder を取得します。</span><span class="sxs-lookup"><span data-stu-id="41e1d-137">Get contactFolders that contain a single-value extended property by using `$expand` or `$filter`.</span></span> |
|[<span data-ttu-id="41e1d-138">複数値の拡張プロパティを作成する</span><span class="sxs-lookup"><span data-stu-id="41e1d-138">Create multi-value extended property</span></span>](../api/multivaluelegacyextendedproperty_post_multivalueextendedproperties.md) | [<span data-ttu-id="41e1d-139">contactFolder</span><span class="sxs-lookup"><span data-stu-id="41e1d-139">contactFolder</span></span>](contactFolder.md) | <span data-ttu-id="41e1d-140">新規または既存の contactFolder に、1 つ以上の複数値の拡張プロパティを作成します。</span><span class="sxs-lookup"><span data-stu-id="41e1d-140">Create one or more multi-value extended properties in a new or existing contactFolder.</span></span>  |
|[<span data-ttu-id="41e1d-141">複数値の拡張プロパティを持つ contactFolder を取得する</span><span class="sxs-lookup"><span data-stu-id="41e1d-141">Get contactFolder with multi-value extended property</span></span>](../api/multivaluelegacyextendedproperty_get.md)  | [<span data-ttu-id="41e1d-142">contactFolder</span><span class="sxs-lookup"><span data-stu-id="41e1d-142">contactFolder</span></span>](contactFolder.md) | <span data-ttu-id="41e1d-143">`$expand` を使用して、複数値の拡張プロパティを含む contactFolder を取得します。</span><span class="sxs-lookup"><span data-stu-id="41e1d-143">Get a contactFolder that contains a multi-value extended property by using `$expand`.</span></span> |

## <a name="properties"></a><span data-ttu-id="41e1d-144">プロパティ</span><span class="sxs-lookup"><span data-stu-id="41e1d-144">Properties</span></span>
| <span data-ttu-id="41e1d-145">プロパティ</span><span class="sxs-lookup"><span data-stu-id="41e1d-145">Property</span></span>     | <span data-ttu-id="41e1d-146">型</span><span class="sxs-lookup"><span data-stu-id="41e1d-146">Type</span></span>   |<span data-ttu-id="41e1d-147">説明</span><span class="sxs-lookup"><span data-stu-id="41e1d-147">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="41e1d-148">displayName</span><span class="sxs-lookup"><span data-stu-id="41e1d-148">displayName</span></span>|<span data-ttu-id="41e1d-149">String</span><span class="sxs-lookup"><span data-stu-id="41e1d-149">String</span></span>|<span data-ttu-id="41e1d-150">フォルダーの表示名。</span><span class="sxs-lookup"><span data-stu-id="41e1d-150">The folder's display name.</span></span>|
|<span data-ttu-id="41e1d-151">id</span><span class="sxs-lookup"><span data-stu-id="41e1d-151">id</span></span>|<span data-ttu-id="41e1d-152">String</span><span class="sxs-lookup"><span data-stu-id="41e1d-152">String</span></span>|<span data-ttu-id="41e1d-p101">連絡先フォルダーの一意識別子。読み取り専用。</span><span class="sxs-lookup"><span data-stu-id="41e1d-p101">Unique identifier of the contact folder. Read-only.</span></span>|
|<span data-ttu-id="41e1d-155">parentFolderId</span><span class="sxs-lookup"><span data-stu-id="41e1d-155">parentFolderId</span></span>|<span data-ttu-id="41e1d-156">String</span><span class="sxs-lookup"><span data-stu-id="41e1d-156">String</span></span>|<span data-ttu-id="41e1d-157">フォルダーの親フォルダーの ID。</span><span class="sxs-lookup"><span data-stu-id="41e1d-157">The ID of the folder's parent folder.</span></span>|

## <a name="relationships"></a><span data-ttu-id="41e1d-158">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="41e1d-158">Relationships</span></span>
| <span data-ttu-id="41e1d-159">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="41e1d-159">Relationship</span></span> | <span data-ttu-id="41e1d-160">型</span><span class="sxs-lookup"><span data-stu-id="41e1d-160">Type</span></span>   |<span data-ttu-id="41e1d-161">説明</span><span class="sxs-lookup"><span data-stu-id="41e1d-161">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="41e1d-162">childFolders</span><span class="sxs-lookup"><span data-stu-id="41e1d-162">childFolders</span></span>|<span data-ttu-id="41e1d-163">[ContactFolder](contactfolder.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="41e1d-163">[ContactFolder](contactfolder.md) collection</span></span>|<span data-ttu-id="41e1d-p102">フォルダー内の子フォルダーのコレクション。ナビゲーション プロパティ。読み取り専用。Null 許容型。</span><span class="sxs-lookup"><span data-stu-id="41e1d-p102">The collection of child folders in the folder. Navigation property. Read-only. Nullable.</span></span>|
|<span data-ttu-id="41e1d-168">contacts</span><span class="sxs-lookup"><span data-stu-id="41e1d-168">contacts</span></span>|<span data-ttu-id="41e1d-169">[Contact](contact.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="41e1d-169">[Contact](contact.md) collection</span></span>|<span data-ttu-id="41e1d-p103">フォルダー内の連絡先。ナビゲーション プロパティ。読み取り専用。Null 許容型。</span><span class="sxs-lookup"><span data-stu-id="41e1d-p103">The contacts in the folder. Navigation property. Read-only. Nullable.</span></span>|
|<span data-ttu-id="41e1d-174">multiValueExtendedProperties</span><span class="sxs-lookup"><span data-stu-id="41e1d-174">multiValueExtendedProperties</span></span>|<span data-ttu-id="41e1d-175">[multiValueLegacyExtendedProperty](multivaluelegacyextendedproperty.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="41e1d-175">[multiValueLegacyExtendedProperty](multivaluelegacyextendedproperty.md) collection</span></span>| <span data-ttu-id="41e1d-p104">contactFolder に定義された、複数値の拡張プロパティのコレクションです。読み取り専用。Null 許容型。</span><span class="sxs-lookup"><span data-stu-id="41e1d-p104">The collection of multi-value extended properties defined for the contactFolder. Read-only. Nullable.</span></span>|
|<span data-ttu-id="41e1d-179">singleValueExtendedProperties</span><span class="sxs-lookup"><span data-stu-id="41e1d-179">singleValueExtendedProperties</span></span>|<span data-ttu-id="41e1d-180">[singleValueLegacyExtendedProperty](singlevaluelegacyextendedproperty.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="41e1d-180">[singleValueLegacyExtendedProperty](singlevaluelegacyextendedproperty.md) collection</span></span>| <span data-ttu-id="41e1d-p105">contactFolder に定義された、単一値の拡張プロパティのコレクションです。読み取り専用。Null 許容型。</span><span class="sxs-lookup"><span data-stu-id="41e1d-p105">The collection of single-value extended properties defined for the contactFolder. Read-only. Nullable.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="41e1d-184">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="41e1d-184">JSON representation</span></span>

<span data-ttu-id="41e1d-185">以下は、リソースの JSON 表記です</span><span class="sxs-lookup"><span data-stu-id="41e1d-185">Here is a JSON representation of the resource</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [
    "childFolders",
    "contacts",
    "multiValueExtendedProperties",
    "singleValueExtendedProperties"
  ],
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.contactFolder"
}-->

```json
{
  "displayName": "string",
  "id": "string (identifier)",
  "parentFolderId": "string"
}

```

## <a name="see-also"></a><span data-ttu-id="41e1d-186">関連項目</span><span class="sxs-lookup"><span data-stu-id="41e1d-186">See also</span></span>

- [<span data-ttu-id="41e1d-187">デルタ クエリを使用して、Microsoft Graph データの変更を追跡する</span><span class="sxs-lookup"><span data-stu-id="41e1d-187">Use delta query to track changes in Microsoft Graph data</span></span>](../../../concepts/delta_query_overview.md)
- [<span data-ttu-id="41e1d-188">フォルダー内のメッセージへの増分の変更を取得する</span><span class="sxs-lookup"><span data-stu-id="41e1d-188">Get incremental changes to messages in a folder</span></span>](../../../concepts/delta_query_messages.md)


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "contactFolder resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
