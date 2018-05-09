# <a name="directory-resource-type-deleted-items"></a><span data-ttu-id="acae2-101">directory リソースの種類 (削除済みアイテム)</span><span class="sxs-lookup"><span data-stu-id="acae2-101">directory resource type (deleted items)</span></span>

<span data-ttu-id="acae2-102">ディレクトリ内の削除済みアイテムを表します。</span><span class="sxs-lookup"><span data-stu-id="acae2-102">Represents a deleted item in the directory.</span></span> <span data-ttu-id="acae2-103">アイテムが削除されると、そのアイテムは削除済みアイテムの「コンテナー」に追加されます。</span><span class="sxs-lookup"><span data-stu-id="acae2-103">When an item is deleted, it is added to the deleted items "container".</span></span> <span data-ttu-id="acae2-104">削除されたアイテムは、最大 30 日間、復元可能な状態に維持されます。</span><span class="sxs-lookup"><span data-stu-id="acae2-104">Deleted items will remain available to restore for up to 30 days.</span></span> <span data-ttu-id="acae2-105">30 日が経過すると、アイテムは完全に削除されます。</span><span class="sxs-lookup"><span data-stu-id="acae2-105">After 30 days, the items are permanently deleted.</span></span>

<span data-ttu-id="acae2-106">現在、[削除済みアイテム] 機能は Office 365 の [group](group.md) および [user](users.md) リソースに対してのみサポートされています。</span><span class="sxs-lookup"><span data-stu-id="acae2-106">Currently, deleted items functionality is only supported for Office 365 [groups](group.md) and [users](users.md).</span></span>

## <a name="methods"></a><span data-ttu-id="acae2-107">メソッド</span><span class="sxs-lookup"><span data-stu-id="acae2-107">Methods</span></span>

| <span data-ttu-id="acae2-108">メソッド</span><span class="sxs-lookup"><span data-stu-id="acae2-108">Method</span></span>         | <span data-ttu-id="acae2-109">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="acae2-109">Return Type</span></span> | <span data-ttu-id="acae2-110">説明</span><span class="sxs-lookup"><span data-stu-id="acae2-110">Description</span></span> |
|:---------------|:------------|:------------|
|[<span data-ttu-id="acae2-111">削除済みアイテムの取得</span><span class="sxs-lookup"><span data-stu-id="acae2-111">Get deleted item</span></span>](../api/directory_deleteditems_get.md) | [<span data-ttu-id="acae2-112">directoryObject</span><span class="sxs-lookup"><span data-stu-id="acae2-112">directoryObject</span></span>](directoryobject.md) | <span data-ttu-id="acae2-113">削除済みアイテムのプロパティを取得します。</span><span class="sxs-lookup"><span data-stu-id="acae2-113">Gets the properties of a deleted item.</span></span> |
|[<span data-ttu-id="acae2-114">削除済みアイテムの復元</span><span class="sxs-lookup"><span data-stu-id="acae2-114">Restore deleted item</span></span>](../api/directory_deleteditems_restore.md) |[<span data-ttu-id="acae2-115">directoryObject</span><span class="sxs-lookup"><span data-stu-id="acae2-115">directoryObject</span></span>](directoryobject.md)| <span data-ttu-id="acae2-116">最近削除されたアイテムを復元します。</span><span class="sxs-lookup"><span data-stu-id="acae2-116">Restores a recently deleted item.</span></span> |
|[<span data-ttu-id="acae2-117">削除済みアイテムの一覧表示</span><span class="sxs-lookup"><span data-stu-id="acae2-117">List deleted items</span></span>](../api/directory_deleteditems_list.md) |<span data-ttu-id="acae2-118">[directoryObject](directoryobject.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="acae2-118">[directoryObject](directoryobject.md) collection</span></span>| <span data-ttu-id="acae2-119">最近削除されたアイテムのリストを取得します。</span><span class="sxs-lookup"><span data-stu-id="acae2-119">Gets a list of recently deleted items.</span></span> |
|[<span data-ttu-id="acae2-120">アイテムの完全削除</span><span class="sxs-lookup"><span data-stu-id="acae2-120">Permanently delete an item</span></span>](../api/directory_deleteditems_delete.md) | <span data-ttu-id="acae2-121">なし</span><span class="sxs-lookup"><span data-stu-id="acae2-121">None</span></span> | <span data-ttu-id="acae2-122">アイテムを完全に削除します。</span><span class="sxs-lookup"><span data-stu-id="acae2-122">Permanently deletes an item.</span></span> |

## <a name="properties"></a><span data-ttu-id="acae2-123">プロパティ</span><span class="sxs-lookup"><span data-stu-id="acae2-123">Properties</span></span>
| <span data-ttu-id="acae2-124">プロパティ</span><span class="sxs-lookup"><span data-stu-id="acae2-124">Property</span></span>   | <span data-ttu-id="acae2-125">型</span><span class="sxs-lookup"><span data-stu-id="acae2-125">Type</span></span> |<span data-ttu-id="acae2-126">説明</span><span class="sxs-lookup"><span data-stu-id="acae2-126">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="acae2-127">id</span><span class="sxs-lookup"><span data-stu-id="acae2-127">id</span></span>|<span data-ttu-id="acae2-128">String</span><span class="sxs-lookup"><span data-stu-id="acae2-128">String</span></span>| <span data-ttu-id="acae2-129">オブジェクトの一意識別子 (例: 12345678-9abc-def0-1234-56789abcde)。</span><span class="sxs-lookup"><span data-stu-id="acae2-129">A Guid that is the unique identifier for the object; for example, 12345678-9abc-def0-1234-56789abcde. Key. Not nullable. Read-only.</span></span> <span data-ttu-id="acae2-130">キー。</span><span class="sxs-lookup"><span data-stu-id="acae2-130">Key</span></span> <span data-ttu-id="acae2-131">null 許容ではありません。</span><span class="sxs-lookup"><span data-stu-id="acae2-131">Not nullable.</span></span> <span data-ttu-id="acae2-132">読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="acae2-132">Read-only.</span></span>|

## <a name="relationships"></a><span data-ttu-id="acae2-133">関係</span><span class="sxs-lookup"><span data-stu-id="acae2-133">Relationships</span></span>
| <span data-ttu-id="acae2-134">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="acae2-134">Relationship</span></span> | <span data-ttu-id="acae2-135">型</span><span class="sxs-lookup"><span data-stu-id="acae2-135">Type</span></span>   |<span data-ttu-id="acae2-136">説明</span><span class="sxs-lookup"><span data-stu-id="acae2-136">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="acae2-137">deleteditems</span><span class="sxs-lookup"><span data-stu-id="acae2-137">deleteditems</span></span>|<span data-ttu-id="acae2-138">[directoryObject](directoryobject.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="acae2-138">[directoryObject](directoryobject.md) collection</span></span>| <span data-ttu-id="acae2-139">最近削除されたアイテム</span><span class="sxs-lookup"><span data-stu-id="acae2-139">Recently deleted items.</span></span> <span data-ttu-id="acae2-140">読み取り専用。</span><span class="sxs-lookup"><span data-stu-id="acae2-140">Read-only.</span></span> <span data-ttu-id="acae2-141">Null 許容型。</span><span class="sxs-lookup"><span data-stu-id="acae2-141">Nullable.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="acae2-142">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="acae2-142">JSON representation</span></span>
<span data-ttu-id="acae2-143">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="acae2-143">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.directory"
}-->

```json
{
  "id": "String (identifier)"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "directory resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->