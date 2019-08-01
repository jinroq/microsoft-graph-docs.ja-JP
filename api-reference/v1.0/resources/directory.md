---
title: directory リソースの種類 (削除済みアイテム)
description: . 削除されたアイテムは、最大 30 日間、復元可能な状態に維持されます。 30 日が経過すると、アイテムは完全に削除されます。
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 627ced59fa87a8e950af96173a807da4d500f428
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "36032747"
---
# <a name="directory-resource-type-deleted-items"></a><span data-ttu-id="92aa9-105">directory リソースの種類 (削除済みアイテム)</span><span class="sxs-lookup"><span data-stu-id="92aa9-105">directory resource type (deleted items)</span></span>

<span data-ttu-id="92aa9-106">ディレクトリ内の削除済みアイテムを表します。</span><span class="sxs-lookup"><span data-stu-id="92aa9-106">Represents a deleted item in the directory.</span></span> <span data-ttu-id="92aa9-107">アイテムが削除されると、そのアイテムは削除済みアイテムの「コンテナー」に追加されます。</span><span class="sxs-lookup"><span data-stu-id="92aa9-107">When an item is deleted, it is added to the deleted items "container".</span></span> <span data-ttu-id="92aa9-108">削除されたアイテムは、最大 30 日間、復元可能な状態に維持されます。</span><span class="sxs-lookup"><span data-stu-id="92aa9-108">Deleted items will remain available to restore for up to 30 days.</span></span> <span data-ttu-id="92aa9-109">30 日が経過すると、アイテムは完全に削除されます。</span><span class="sxs-lookup"><span data-stu-id="92aa9-109">After 30 days, the items are permanently deleted.</span></span>

<span data-ttu-id="92aa9-110">現在、[削除済みアイテム] 機能は Office 365 の [group](group.md) および [user](users.md) リソースに対してのみサポートされています。</span><span class="sxs-lookup"><span data-stu-id="92aa9-110">Currently, deleted items functionality is only supported for Office 365 [groups](group.md) and [users](users.md).</span></span>

## <a name="methods"></a><span data-ttu-id="92aa9-111">メソッド</span><span class="sxs-lookup"><span data-stu-id="92aa9-111">Methods</span></span>

| <span data-ttu-id="92aa9-112">メソッド</span><span class="sxs-lookup"><span data-stu-id="92aa9-112">Method</span></span>         | <span data-ttu-id="92aa9-113">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="92aa9-113">Return Type</span></span> | <span data-ttu-id="92aa9-114">説明</span><span class="sxs-lookup"><span data-stu-id="92aa9-114">Description</span></span> |
|:---------------|:------------|:------------|
|[<span data-ttu-id="92aa9-115">削除済みアイテムの取得</span><span class="sxs-lookup"><span data-stu-id="92aa9-115">Get deleted item</span></span>](../api/directory-deleteditems-get.md) | [<span data-ttu-id="92aa9-116">directoryObject</span><span class="sxs-lookup"><span data-stu-id="92aa9-116">directoryObject</span></span>](directoryobject.md) | <span data-ttu-id="92aa9-117">削除済みアイテムのプロパティを取得します。</span><span class="sxs-lookup"><span data-stu-id="92aa9-117">Gets the properties of a deleted item.</span></span> |
|[<span data-ttu-id="92aa9-118">削除済みアイテムの復元</span><span class="sxs-lookup"><span data-stu-id="92aa9-118">Restore deleted item</span></span>](../api/directory-deleteditems-restore.md) |[<span data-ttu-id="92aa9-119">directoryObject</span><span class="sxs-lookup"><span data-stu-id="92aa9-119">directoryObject</span></span>](directoryobject.md)| <span data-ttu-id="92aa9-120">最近削除されたアイテムを復元します。</span><span class="sxs-lookup"><span data-stu-id="92aa9-120">Restores a recently deleted item.</span></span> |
|[<span data-ttu-id="92aa9-121">削除済みアイテムの一覧表示</span><span class="sxs-lookup"><span data-stu-id="92aa9-121">List deleted items</span></span>](../api/directory-deleteditems-list.md) |<span data-ttu-id="92aa9-122">[directoryObject](directoryobject.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="92aa9-122">[directoryObject](directoryobject.md) collection</span></span>| <span data-ttu-id="92aa9-123">最近削除されたアイテムのリストを取得します。</span><span class="sxs-lookup"><span data-stu-id="92aa9-123">Gets a list of recently deleted items.</span></span> |
|[<span data-ttu-id="92aa9-124">アイテムの完全削除</span><span class="sxs-lookup"><span data-stu-id="92aa9-124">Permanently delete an item</span></span>](../api/directory-deleteditems-delete.md) | <span data-ttu-id="92aa9-125">なし</span><span class="sxs-lookup"><span data-stu-id="92aa9-125">None</span></span> | <span data-ttu-id="92aa9-126">アイテムを完全に削除します。</span><span class="sxs-lookup"><span data-stu-id="92aa9-126">Permanently deletes an item.</span></span> |
|[<span data-ttu-id="92aa9-127">ユーザーが所有する削除済みアイテムを一覧表示する</span><span class="sxs-lookup"><span data-stu-id="92aa9-127">List deleted items owned by a user</span></span>](../api/directory-deleteditems-user-owned.md) | <span data-ttu-id="92aa9-128">[directoryObject](directoryobject.md) collection</span><span class="sxs-lookup"><span data-stu-id="92aa9-128">[directoryObject](directoryobject.md) collection</span></span> | <span data-ttu-id="92aa9-129">ユーザーが所有しているディレクトリアイテムを一覧表示します。</span><span class="sxs-lookup"><span data-stu-id="92aa9-129">Lists directory items owned by a user.</span></span> |

## <a name="relationships"></a><span data-ttu-id="92aa9-130">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="92aa9-130">Relationships</span></span>
| <span data-ttu-id="92aa9-131">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="92aa9-131">Relationship</span></span> | <span data-ttu-id="92aa9-132">型</span><span class="sxs-lookup"><span data-stu-id="92aa9-132">Type</span></span>   |<span data-ttu-id="92aa9-133">説明</span><span class="sxs-lookup"><span data-stu-id="92aa9-133">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="92aa9-134">deletedItems</span><span class="sxs-lookup"><span data-stu-id="92aa9-134">deletedItems</span></span>|<span data-ttu-id="92aa9-135">[directoryObject](directoryobject.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="92aa9-135">[directoryObject](directoryobject.md) collection</span></span>| <span data-ttu-id="92aa9-136">最近削除されたアイテム</span><span class="sxs-lookup"><span data-stu-id="92aa9-136">Recently deleted items.</span></span> <span data-ttu-id="92aa9-137">読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="92aa9-137">Read-only.</span></span> <span data-ttu-id="92aa9-138">Null 許容型。</span><span class="sxs-lookup"><span data-stu-id="92aa9-138">Nullable.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="92aa9-139">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="92aa9-139">JSON representation</span></span>
<span data-ttu-id="92aa9-140">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="92aa9-140">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "baseType": "microsoft.graph.entity",
  "@odata.type": "microsoft.graph.directory"
}-->

```json
{
}
```

## <a name="example"></a><span data-ttu-id="92aa9-141">例</span><span class="sxs-lookup"><span data-stu-id="92aa9-141">Example</span></span>

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
