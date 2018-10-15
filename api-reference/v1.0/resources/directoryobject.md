# <a name="directoryobject-resource-type"></a><span data-ttu-id="75143-101">directoryObject リソースの種類</span><span class="sxs-lookup"><span data-stu-id="75143-101">directoryObject resource type</span></span>

<span data-ttu-id="75143-p101">Azure Active Directory オブジェクトを表します。**directoryObject** 型は、他の多くのディレクトリ エンティティ型の基本型です。</span><span class="sxs-lookup"><span data-stu-id="75143-p101">Represents an Azure Active Directory object. The **directoryObject** type is the base type for many other directory entity types.</span></span>

## <a name="methods"></a><span data-ttu-id="75143-104">メソッド</span><span class="sxs-lookup"><span data-stu-id="75143-104">Methods</span></span>

| <span data-ttu-id="75143-105">メソッド</span><span class="sxs-lookup"><span data-stu-id="75143-105">Method</span></span>       | <span data-ttu-id="75143-106">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="75143-106">Return Type</span></span>  |<span data-ttu-id="75143-107">説明</span><span class="sxs-lookup"><span data-stu-id="75143-107">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="75143-108">Get directoryObject</span><span class="sxs-lookup"><span data-stu-id="75143-108">Get directoryObject</span></span>](../api/directoryobject_get.md) | [<span data-ttu-id="75143-109">directoryObject</span><span class="sxs-lookup"><span data-stu-id="75143-109">directoryObject</span></span>](directoryobject.md) |<span data-ttu-id="75143-110">ディレクトリ オブジェクトのプロパティを読み取ります。</span><span class="sxs-lookup"><span data-stu-id="75143-110">Read the properties  of a directory object.</span></span>|
|[<span data-ttu-id="75143-111">Delete directoryObject</span><span class="sxs-lookup"><span data-stu-id="75143-111">Delete directoryObject</span></span>](../api/directoryobject_delete.md) | <span data-ttu-id="75143-112">なし</span><span class="sxs-lookup"><span data-stu-id="75143-112">None</span></span> |<span data-ttu-id="75143-113">ディレクトリ オブジェクトを削除します。</span><span class="sxs-lookup"><span data-stu-id="75143-113">Delete a directory object.</span></span> |
|[<span data-ttu-id="75143-114">checkMemberGroups</span><span class="sxs-lookup"><span data-stu-id="75143-114">checkMemberGroups</span></span>](../api/directoryobject_checkmembergroups.md)|<span data-ttu-id="75143-115">String コレクション</span><span class="sxs-lookup"><span data-stu-id="75143-115">String collection</span></span>|<span data-ttu-id="75143-p102">グループの一覧内のメンバーシップを確認します。チェックは推移的です。</span><span class="sxs-lookup"><span data-stu-id="75143-p102">Check for membership in a list of groups. The check is transitive.</span></span>|
|[<span data-ttu-id="75143-118">getMemberGroups</span><span class="sxs-lookup"><span data-stu-id="75143-118">getMemberGroups</span></span>](../api/directoryobject_getmembergroups.md)|<span data-ttu-id="75143-119">String コレクション</span><span class="sxs-lookup"><span data-stu-id="75143-119">String collection</span></span>|<span data-ttu-id="75143-p103">ユーザー オブジェクト、グループ オブジェクト、またはディレクトリ オブジェクトがメンバーであるすべてのグループを返します。チェックは推移的です。</span><span class="sxs-lookup"><span data-stu-id="75143-p103">Return all the groups that the user, group, or directory object is a member of. The check is transitive.</span></span>|
|[<span data-ttu-id="75143-122">getMemberObjects</span><span class="sxs-lookup"><span data-stu-id="75143-122">getMemberObjects</span></span>](../api/directoryobject_getmemberobjects.md)|<span data-ttu-id="75143-123">String コレクション</span><span class="sxs-lookup"><span data-stu-id="75143-123">String collection</span></span>| <span data-ttu-id="75143-p104">ユーザー オブジェクト、グループ オブジェクト、またはディレクトリ オブジェクトがメンバーであるすべてのグループとディレクトリ ロールを返します。チェックは推移的です。</span><span class="sxs-lookup"><span data-stu-id="75143-p104">Return all of the groups and directory roles that the user, group, or directory object is a member of. The check is transitive.</span></span> |
|[<span data-ttu-id="75143-126">getByIds</span><span class="sxs-lookup"><span data-stu-id="75143-126">getByIds</span></span>](../api/directoryobject_getbyids.md) | <span data-ttu-id="75143-127">[directoryObject](directoryobject.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="75143-127">[directoryObject](directoryobject.md) collection</span></span> | <span data-ttu-id="75143-128">指定された一連の ID に基づいて、一連のディレクトリ オブジェクトを取得します。</span><span class="sxs-lookup"><span data-stu-id="75143-128">Get a set of directory objects based on a set of supplied ids.</span></span> |

## <a name="properties"></a><span data-ttu-id="75143-129">プロパティ</span><span class="sxs-lookup"><span data-stu-id="75143-129">Properties</span></span>

| <span data-ttu-id="75143-130">プロパティ</span><span class="sxs-lookup"><span data-stu-id="75143-130">Property</span></span>   | <span data-ttu-id="75143-131">タイプ</span><span class="sxs-lookup"><span data-stu-id="75143-131">Type</span></span> |<span data-ttu-id="75143-132">説明</span><span class="sxs-lookup"><span data-stu-id="75143-132">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="75143-133">id</span><span class="sxs-lookup"><span data-stu-id="75143-133">id</span></span>|<span data-ttu-id="75143-134">文字列</span><span class="sxs-lookup"><span data-stu-id="75143-134">String</span></span>|<span data-ttu-id="75143-p105">オブジェクトの一意識別子である Guid。例: 12345678-9abc-def0-1234-56789abcde。キー。null 許容ではありません。読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="75143-p105">A Guid that is the unique identifier for the object; for example, 12345678-9abc-def0-1234-56789abcde. Key. Not nullable. Read-only.</span></span>|

## <a name="relationships"></a><span data-ttu-id="75143-139">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="75143-139">Relationships</span></span>

<span data-ttu-id="75143-140">なし</span><span class="sxs-lookup"><span data-stu-id="75143-140">None</span></span>


## <a name="json-representation"></a><span data-ttu-id="75143-141">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="75143-141">JSON representation</span></span>

<span data-ttu-id="75143-142">以下は、リソースの JSON 表記です</span><span class="sxs-lookup"><span data-stu-id="75143-142">Here is a JSON representation of the resource</span></span>

<!--{
  "blockType": "resource",
  "openType": true,
  "optionalProperties": [],
  "keyProperty": "id",
  "baseType": "microsoft.graph.entity",
  "@odata.type": "microsoft.graph.directoryObject",
  "@odata.annotations": [
    {
      "capabilities": {
        "skippable": false,
        "countable": false,
        "expandable": false,
        "filterable": false,
        "referenceable": false,
        "selectable": false
      }
    }
  ]
}-->

```json
{
  "id": "string (identifier)"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "directoryObject resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
