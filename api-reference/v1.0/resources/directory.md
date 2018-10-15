# <a name="directory-resource-type-deleted-items"></a><span data-ttu-id="7bd6d-101">directory リソースの種類 (削除済みアイテム)</span><span class="sxs-lookup"><span data-stu-id="7bd6d-101">directory resource type (deleted items)</span></span>

<span data-ttu-id="7bd6d-102">ディレクトリ内の削除済みアイテムを表します。</span><span class="sxs-lookup"><span data-stu-id="7bd6d-102">Represents a deleted item in the directory.</span></span> <span data-ttu-id="7bd6d-103">アイテムが削除されると、そのアイテムは削除済みアイテムの「コンテナー」に追加されます。</span><span class="sxs-lookup"><span data-stu-id="7bd6d-103">When an item is deleted, it is added to the deleted items "container".</span></span> <span data-ttu-id="7bd6d-104">削除されたアイテムは、最大 30 日間、復元可能な状態に維持されます。</span><span class="sxs-lookup"><span data-stu-id="7bd6d-104">Deleted items will remain available to restore for up to 30 days.</span></span> <span data-ttu-id="7bd6d-105">30 日が経過すると、アイテムは完全に削除されます。</span><span class="sxs-lookup"><span data-stu-id="7bd6d-105">After 30 days, the items are permanently deleted.</span></span>

<span data-ttu-id="7bd6d-106">現在、[削除済みアイテム] 機能は Office 365 の [group](group.md) および [user](users.md) リソースに対してのみサポートされています。</span><span class="sxs-lookup"><span data-stu-id="7bd6d-106">Currently, deleted items functionality is only supported for Office 365 [groups](group.md) and [users](users.md).</span></span>

## <a name="methods"></a><span data-ttu-id="7bd6d-107">メソッド</span><span class="sxs-lookup"><span data-stu-id="7bd6d-107">Methods</span></span>

| <span data-ttu-id="7bd6d-108">メソッド</span><span class="sxs-lookup"><span data-stu-id="7bd6d-108">Method</span></span>         | <span data-ttu-id="7bd6d-109">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="7bd6d-109">Return Type</span></span> | <span data-ttu-id="7bd6d-110">説明</span><span class="sxs-lookup"><span data-stu-id="7bd6d-110">Description</span></span> |
|:---------------|:------------|:------------|
|[<span data-ttu-id="7bd6d-111">削除済みアイテムの取得</span><span class="sxs-lookup"><span data-stu-id="7bd6d-111">Get deleted item</span></span>](../api/directory_deleteditems_get.md) | [<span data-ttu-id="7bd6d-112">directoryObject</span><span class="sxs-lookup"><span data-stu-id="7bd6d-112">directoryObject</span></span>](directoryobject.md) | <span data-ttu-id="7bd6d-113">削除済みアイテムのプロパティを取得します。</span><span class="sxs-lookup"><span data-stu-id="7bd6d-113">Gets the properties of a deleted item.</span></span> |
|[<span data-ttu-id="7bd6d-114">削除済みアイテムの復元</span><span class="sxs-lookup"><span data-stu-id="7bd6d-114">Restore deleted item</span></span>](../api/directory_deleteditems_restore.md) |[<span data-ttu-id="7bd6d-115">directoryObject</span><span class="sxs-lookup"><span data-stu-id="7bd6d-115">directoryObject</span></span>](directoryobject.md)| <span data-ttu-id="7bd6d-116">最近削除されたアイテムを復元します。</span><span class="sxs-lookup"><span data-stu-id="7bd6d-116">Restores a recently deleted item.</span></span> |
|[<span data-ttu-id="7bd6d-117">削除済みアイテムの一覧表示</span><span class="sxs-lookup"><span data-stu-id="7bd6d-117">List deleted items</span></span>](../api/directory_deleteditems_list.md) |<span data-ttu-id="7bd6d-118">[directoryObject](directoryobject.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="7bd6d-118">[directoryObject](directoryobject.md) collection</span></span>| <span data-ttu-id="7bd6d-119">最近削除されたアイテムのリストを取得します。</span><span class="sxs-lookup"><span data-stu-id="7bd6d-119">Gets a list of recently deleted items.</span></span> |
|[<span data-ttu-id="7bd6d-120">アイテムの完全削除</span><span class="sxs-lookup"><span data-stu-id="7bd6d-120">Permanently delete an item</span></span>](../api/directory_deleteditems_delete.md) | <span data-ttu-id="7bd6d-121">なし</span><span class="sxs-lookup"><span data-stu-id="7bd6d-121">None</span></span> | <span data-ttu-id="7bd6d-122">アイテムを完全に削除します。</span><span class="sxs-lookup"><span data-stu-id="7bd6d-122">Permanently deletes an item.</span></span> |
|<span data-ttu-id="7bd6d-123">[ユーザーによって所有されている削除済みのアイテムを一覧表示します。](../api/directory_deleteditems_user_owned.md)</span><span class="sxs-lookup"><span data-stu-id="7bd6d-123">Added [List deleted items owned by a user](../api/directory_deleteditems_user_owned.md) action to directory (deleted items) resource</span></span> | <span data-ttu-id="7bd6d-124">[directoryObject](directoryobject.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="7bd6d-124">[directoryObject](directoryobject.md) collection</span></span> | <span data-ttu-id="7bd6d-125">ユーザーによって所有されているディレクトリの項目を一覧表示します。</span><span class="sxs-lookup"><span data-stu-id="7bd6d-125">Lists directory items owned by a user.</span></span> |

## <a name="relationships"></a><span data-ttu-id="7bd6d-126">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="7bd6d-126">Relationships</span></span>
| <span data-ttu-id="7bd6d-127">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="7bd6d-127">Relationship</span></span> | <span data-ttu-id="7bd6d-128">型</span><span class="sxs-lookup"><span data-stu-id="7bd6d-128">Type</span></span>   |<span data-ttu-id="7bd6d-129">説明</span><span class="sxs-lookup"><span data-stu-id="7bd6d-129">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="7bd6d-130">deleteditems</span><span class="sxs-lookup"><span data-stu-id="7bd6d-130">deleteditems</span></span>|<span data-ttu-id="7bd6d-131">[directoryObject](directoryobject.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="7bd6d-131">[directoryObject](directoryobject.md) collection</span></span>| <span data-ttu-id="7bd6d-132">最近削除されたアイテム</span><span class="sxs-lookup"><span data-stu-id="7bd6d-132">Recently deleted items.</span></span> <span data-ttu-id="7bd6d-133">読み取り専用。</span><span class="sxs-lookup"><span data-stu-id="7bd6d-133">Read-only.</span></span> <span data-ttu-id="7bd6d-134">Null 許容型。</span><span class="sxs-lookup"><span data-stu-id="7bd6d-134">Nullable.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="7bd6d-135">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="7bd6d-135">JSON representation</span></span>
<span data-ttu-id="7bd6d-136">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="7bd6d-136">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "baseType": "microsoft.graph.entity",
  "@odata.type": "microsoft.graph.directory"
}-->

```json
{
}
```

## <a name="example"></a><span data-ttu-id="7bd6d-137">例</span><span class="sxs-lookup"><span data-stu-id="7bd6d-137">Example</span></span>

<!--{"blockType": "request"}-->
```http
GET https://graph.microsoft.com/v1.0/directory
```

<!--{"blockType": "response", "truncated": true, "@odata.type": "microsoft.graph.directory"}-->
```json
HTTP/1.1 200 OK
Content-Type: application/json

{
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