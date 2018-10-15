# <a name="contactfolder-resource-type"></a><span data-ttu-id="d7fab-101">contactFolder リソース型</span><span class="sxs-lookup"><span data-stu-id="d7fab-101">contactFolder resource type</span></span>

<span data-ttu-id="d7fab-102">連絡先が格納されたフォルダーです。</span><span class="sxs-lookup"><span data-stu-id="d7fab-102">A folder that contains contacts.</span></span>

<span data-ttu-id="d7fab-103">このリソースでは、[デルタ](../api/contactfolder_delta.md)関数を用意すれば、増分の追加、削除、更新に[デルタ クエリ](../../../concepts/delta_query_overview.md)を使用できます。</span><span class="sxs-lookup"><span data-stu-id="d7fab-103">This resource supports using [delta query](../../../concepts/delta_query_overview.md) to track incremental additions, deletions, and updates, by providing a [delta](../api/contactfolder_delta.md) function.</span></span>


## <a name="methods"></a><span data-ttu-id="d7fab-104">メソッド</span><span class="sxs-lookup"><span data-stu-id="d7fab-104">Methods</span></span>

| <span data-ttu-id="d7fab-105">メソッド</span><span class="sxs-lookup"><span data-stu-id="d7fab-105">Method</span></span>       | <span data-ttu-id="d7fab-106">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="d7fab-106">Return Type</span></span>  |<span data-ttu-id="d7fab-107">説明</span><span class="sxs-lookup"><span data-stu-id="d7fab-107">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="d7fab-108">contactFolder を取得する</span><span class="sxs-lookup"><span data-stu-id="d7fab-108">Get contactFolder</span></span>](../api/contactfolder_get.md) | [<span data-ttu-id="d7fab-109">contactFolder</span><span class="sxs-lookup"><span data-stu-id="d7fab-109">contactFolder</span></span>](contactfolder.md) |<span data-ttu-id="d7fab-110">連絡先フォルダー ID を使用して連絡先フォルダーを取得します。</span><span class="sxs-lookup"><span data-stu-id="d7fab-110">Get a contact folder by using the contact folder ID.</span></span>|
|[<span data-ttu-id="d7fab-111">更新する</span><span class="sxs-lookup"><span data-stu-id="d7fab-111">Update</span></span>](../api/contactfolder_update.md) | [<span data-ttu-id="d7fab-112">contactFolder</span><span class="sxs-lookup"><span data-stu-id="d7fab-112">contactFolder</span></span>](contactfolder.md) |<span data-ttu-id="d7fab-113">contactFolder オブジェクトを更新します。</span><span class="sxs-lookup"><span data-stu-id="d7fab-113">Update contactFolder object.</span></span> |
|[<span data-ttu-id="d7fab-114">削除</span><span class="sxs-lookup"><span data-stu-id="d7fab-114">Delete</span></span>](../api/contactfolder_delete.md) | <span data-ttu-id="d7fab-115">なし</span><span class="sxs-lookup"><span data-stu-id="d7fab-115">None</span></span> |<span data-ttu-id="d7fab-116">contactFolder オブジェクトを削除します。</span><span class="sxs-lookup"><span data-stu-id="d7fab-116">Delete contactFolder object.</span></span> |
|[<span data-ttu-id="d7fab-117">childFolders を一覧表示する</span><span class="sxs-lookup"><span data-stu-id="d7fab-117">List childFolders</span></span>](../api/contactfolder_list_childfolders.md) |<span data-ttu-id="d7fab-118">[ContactFolder](contactfolder.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="d7fab-118">[ContactFolder](contactfolder.md) collection</span></span>| <span data-ttu-id="d7fab-119">指定した連絡先フォルダーの下の子フォルダーのコレクションを取得します。</span><span class="sxs-lookup"><span data-stu-id="d7fab-119">Get a collection of child folders under the specified contact folder.</span></span>|
|[<span data-ttu-id="d7fab-120">子 contactFolder を作成する</span><span class="sxs-lookup"><span data-stu-id="d7fab-120">Create child contactFolder</span></span>](../api/contactfolder_post_childfolders.md) |[<span data-ttu-id="d7fab-121">ContactFolder</span><span class="sxs-lookup"><span data-stu-id="d7fab-121">ContactFolder</span></span>](contactfolder.md)| <span data-ttu-id="d7fab-122">指定したフォルダーの子として新しい contactFolder を作成します。</span><span class="sxs-lookup"><span data-stu-id="d7fab-122">Create a new contactFolder as a child of a specified folder.</span></span>|
|[<span data-ttu-id="d7fab-123">delta</span><span class="sxs-lookup"><span data-stu-id="d7fab-123">delta</span></span>](../api/contact_delta.md)|<span data-ttu-id="d7fab-124">[contact](contact.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="d7fab-124">[contact](contact.md) collection</span></span>| <span data-ttu-id="d7fab-125">ユーザーのメールボックスで追加または削除された一連の連絡先フォルダーを取得します。</span><span class="sxs-lookup"><span data-stu-id="d7fab-125">Get a set of contact folders that have been added, deleted, or removed from the user's mailbox.</span></span>|
|[<span data-ttu-id="d7fab-126">フォルダー内の連絡先を一覧表示する</span><span class="sxs-lookup"><span data-stu-id="d7fab-126">List contacts in folder</span></span>](../api/contactfolder_list_contacts.md) |<span data-ttu-id="d7fab-127">[Contact](contact.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="d7fab-127">[Contact](contact.md) collection</span></span>| <span data-ttu-id="d7fab-128">サインイン中のユーザーの既定の連絡先フォルダーから連絡先のコレクションを取得する (`.../me/contacts`) か、指定した連絡先フォルダーから取得します。</span><span class="sxs-lookup"><span data-stu-id="d7fab-128">Get a contact collection from the default Contacts folder of the signed-in user (`.../me/contacts`), or from the specified contact folder.</span></span>|
|[<span data-ttu-id="d7fab-129">フォルダー内に連絡先を作成する</span><span class="sxs-lookup"><span data-stu-id="d7fab-129">Create contact in folder</span></span>](../api/contactfolder_post_contacts.md) |[<span data-ttu-id="d7fab-130">連絡先</span><span class="sxs-lookup"><span data-stu-id="d7fab-130">Contact</span></span>](contact.md)| <span data-ttu-id="d7fab-131">連絡先をルート連絡先フォルダーまたは別の連絡先フォルダーの `contacts` エンドポイントに追加します。</span><span class="sxs-lookup"><span data-stu-id="d7fab-131">Add a contact to the root Contacts folder or to the `contacts` endpoint of another contact folder.</span></span>|
|[<span data-ttu-id="d7fab-132">単一値の拡張プロパティを作成する</span><span class="sxs-lookup"><span data-stu-id="d7fab-132">Create single-value extended property</span></span>](../api/singlevaluelegacyextendedproperty_post_singlevalueextendedproperties.md) |[<span data-ttu-id="d7fab-133">contactFolder</span><span class="sxs-lookup"><span data-stu-id="d7fab-133">contactFolder</span></span>](contactFolder.md)  |<span data-ttu-id="d7fab-134">新規または既存の contactFolder に、1 つ以上の単一値の拡張プロパティを作成します。</span><span class="sxs-lookup"><span data-stu-id="d7fab-134">Create one or more single-value extended properties in a new or existing contactFolder.</span></span>   |
|[<span data-ttu-id="d7fab-135">単一値の拡張プロパティを持つ contactFolder を取得する</span><span class="sxs-lookup"><span data-stu-id="d7fab-135">Get contactFolder with single-value extended property</span></span>](../api/singlevaluelegacyextendedproperty_get.md)  | [<span data-ttu-id="d7fab-136">contactFolder</span><span class="sxs-lookup"><span data-stu-id="d7fab-136">contactFolder</span></span>](contactFolder.md) | <span data-ttu-id="d7fab-137">または `$filter` を使用して、単一値の拡張プロパティを含む contactFolder を取得します。`$expand`</span><span class="sxs-lookup"><span data-stu-id="d7fab-137">Get contactFolders that contain a single-value extended property by using `$expand` or `$filter`.</span></span> |
|[<span data-ttu-id="d7fab-138">複数値の拡張プロパティを作成する</span><span class="sxs-lookup"><span data-stu-id="d7fab-138">Create multi-value extended property</span></span>](../api/multivaluelegacyextendedproperty_post_multivalueextendedproperties.md) | [<span data-ttu-id="d7fab-139">contactFolder</span><span class="sxs-lookup"><span data-stu-id="d7fab-139">contactFolder</span></span>](contactFolder.md) | <span data-ttu-id="d7fab-140">新規または既存の contactFolder に、1 つ以上の複数値の拡張プロパティを作成します。</span><span class="sxs-lookup"><span data-stu-id="d7fab-140">Create one or more multi-value extended properties in a new or existing contactFolder.</span></span>  |
|[<span data-ttu-id="d7fab-141">複数値の拡張プロパティを持つ contactFolder を取得する</span><span class="sxs-lookup"><span data-stu-id="d7fab-141">Get contactFolder with multi-value extended property</span></span>](../api/multivaluelegacyextendedproperty_get.md)  | [<span data-ttu-id="d7fab-142">contactFolder</span><span class="sxs-lookup"><span data-stu-id="d7fab-142">contactFolder</span></span>](contactFolder.md) | <span data-ttu-id="d7fab-143">を使用して、複数値の拡張プロパティを含む contactFolder を取得します。`$expand`</span><span class="sxs-lookup"><span data-stu-id="d7fab-143">Get a contactFolder that contains a multi-value extended property by using `$expand`.</span></span> |

## <a name="properties"></a><span data-ttu-id="d7fab-144">プロパティ</span><span class="sxs-lookup"><span data-stu-id="d7fab-144">Properties</span></span>
| <span data-ttu-id="d7fab-145">プロパティ</span><span class="sxs-lookup"><span data-stu-id="d7fab-145">Property</span></span>     | <span data-ttu-id="d7fab-146">タイプ</span><span class="sxs-lookup"><span data-stu-id="d7fab-146">Type</span></span>   |<span data-ttu-id="d7fab-147">説明</span><span class="sxs-lookup"><span data-stu-id="d7fab-147">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="d7fab-148">displayName</span><span class="sxs-lookup"><span data-stu-id="d7fab-148">displayName</span></span>|<span data-ttu-id="d7fab-149">文字列</span><span class="sxs-lookup"><span data-stu-id="d7fab-149">String</span></span>|<span data-ttu-id="d7fab-150">フォルダーの表示名。</span><span class="sxs-lookup"><span data-stu-id="d7fab-150">The folder's display name.</span></span>|
|<span data-ttu-id="d7fab-151">id</span><span class="sxs-lookup"><span data-stu-id="d7fab-151">id</span></span>|<span data-ttu-id="d7fab-152">文字列</span><span class="sxs-lookup"><span data-stu-id="d7fab-152">String</span></span>|<span data-ttu-id="d7fab-p101">連絡先フォルダーの一意識別子。読み取り専用。</span><span class="sxs-lookup"><span data-stu-id="d7fab-p101">Unique identifier of the contact folder. Read-only.</span></span>|
|<span data-ttu-id="d7fab-155">parentFolderId</span><span class="sxs-lookup"><span data-stu-id="d7fab-155">parentFolderId</span></span>|<span data-ttu-id="d7fab-156">文字列</span><span class="sxs-lookup"><span data-stu-id="d7fab-156">String</span></span>|<span data-ttu-id="d7fab-157">フォルダーの親フォルダーの ID。</span><span class="sxs-lookup"><span data-stu-id="d7fab-157">The ID of the folder's parent folder.</span></span>|

## <a name="relationships"></a><span data-ttu-id="d7fab-158">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="d7fab-158">Relationships</span></span>
| <span data-ttu-id="d7fab-159">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="d7fab-159">Relationship</span></span> | <span data-ttu-id="d7fab-160">型</span><span class="sxs-lookup"><span data-stu-id="d7fab-160">Type</span></span>   |<span data-ttu-id="d7fab-161">説明</span><span class="sxs-lookup"><span data-stu-id="d7fab-161">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="d7fab-162">childFolders</span><span class="sxs-lookup"><span data-stu-id="d7fab-162">childFolders</span></span>|<span data-ttu-id="d7fab-163">[ContactFolder](contactfolder.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="d7fab-163">[ContactFolder](contactfolder.md) collection</span></span>|<span data-ttu-id="d7fab-p102">フォルダー内の子フォルダーのコレクション。ナビゲーション プロパティ。読み取り専用。Null 許容型。</span><span class="sxs-lookup"><span data-stu-id="d7fab-p102">The collection of child folders in the folder. Navigation property. Read-only. Nullable.</span></span>|
|<span data-ttu-id="d7fab-168">contacts</span><span class="sxs-lookup"><span data-stu-id="d7fab-168">contacts</span></span>|<span data-ttu-id="d7fab-169">[Contact](contact.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="d7fab-169">[Contact](contact.md) collection</span></span>|<span data-ttu-id="d7fab-p103">フォルダー内の連絡先。ナビゲーション プロパティ。読み取り専用。Null 許容型。</span><span class="sxs-lookup"><span data-stu-id="d7fab-p103">The contacts in the folder. Navigation property. Read-only. Nullable.</span></span>|
|<span data-ttu-id="d7fab-174">multiValueExtendedProperties</span><span class="sxs-lookup"><span data-stu-id="d7fab-174">multiValueExtendedProperties</span></span>|<span data-ttu-id="d7fab-175">[multiValueLegacyExtendedProperty](multivaluelegacyextendedproperty.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="d7fab-175">[multiValueLegacyExtendedProperty](multivaluelegacyextendedproperty.md) collection</span></span>| <span data-ttu-id="d7fab-p104">contactFolder に定義された、複数値の拡張プロパティのコレクションです。読み取り専用。Null 許容型。</span><span class="sxs-lookup"><span data-stu-id="d7fab-p104">The collection of multi-value extended properties defined for the contactFolder. Read-only. Nullable.</span></span>|
|<span data-ttu-id="d7fab-179">singleValueExtendedProperties</span><span class="sxs-lookup"><span data-stu-id="d7fab-179">singleValueExtendedProperties</span></span>|<span data-ttu-id="d7fab-180">[singleValueLegacyExtendedProperty](singlevaluelegacyextendedproperty.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="d7fab-180">[singleValueLegacyExtendedProperty](singlevaluelegacyextendedproperty.md) collection</span></span>| <span data-ttu-id="d7fab-p105">contactFolder に定義された、単一値の拡張プロパティのコレクションです。読み取り専用。Null 許容型。</span><span class="sxs-lookup"><span data-stu-id="d7fab-p105">The collection of single-value extended properties defined for the contactFolder. Read-only. Nullable.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="d7fab-184">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="d7fab-184">JSON representation</span></span>

<span data-ttu-id="d7fab-185">以下は、リソースの JSON 表記です</span><span class="sxs-lookup"><span data-stu-id="d7fab-185">Here is a JSON representation of the resource</span></span>

<!--{
  "blockType": "resource",
  "optionalProperties": [
    "childFolders",
    "contacts",
    "multiValueExtendedProperties",
    "singleValueExtendedProperties"
  ],
  "keyProperty": "id",
  "baseType": "microsoft.graph.entity",
  "@odata.type": "microsoft.graph.contactFolder",
  "@odata.annotations": [
    {
      "property": "childFolders",
      "capabilities": {
        "navigability": "single",
        "changeTracking": false,
        "searchable": false
      }
    },
    {
      "property": "contacts",
      "capabilities": {
        "changeTracking": true,
        "navigability": "single",
        "searchable": false
      }
    }
  ]
}-->

```json
{
  "displayName": "string",
  "id": "string (identifier)",
  "parentFolderId": "string"
}

```

## <a name="see-also"></a><span data-ttu-id="d7fab-186">関連項目</span><span class="sxs-lookup"><span data-stu-id="d7fab-186">See also</span></span>

- [<span data-ttu-id="d7fab-187">デルタ クエリを使用して、Microsoft Graph データの変更を追跡する</span><span class="sxs-lookup"><span data-stu-id="d7fab-187">Use delta query to track changes in Microsoft Graph data</span></span>](../../../concepts/delta_query_overview.md)
- [<span data-ttu-id="d7fab-188">フォルダー内のメッセージへの増分の変更を取得する</span><span class="sxs-lookup"><span data-stu-id="d7fab-188">Get incremental changes to messages in a folder</span></span>](../../../concepts/delta_query_messages.md)


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "contactFolder resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
