---
title: directory リソースの種類 (削除済みアイテム)
description: . 削除されたアイテムは、最大 30 日間、復元可能な状態に維持されます。 30 日が経過すると、アイテムは完全に削除されます。
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
ms.openlocfilehash: e9437f2f57c1ac53dc8f227149e679edd32d1ff1
ms.sourcegitcommit: 33f1cf5b3b79bfba6a06b52d34e558a6ba327d21
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/31/2019
ms.locfileid: "34657687"
---
# <a name="directory-resource-type-deleted-items"></a><span data-ttu-id="aa205-105">directory リソースの種類 (削除済みアイテム)</span><span class="sxs-lookup"><span data-stu-id="aa205-105">directory resource type (deleted items)</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="aa205-106">ディレクトリ内の削除済みアイテムを表します。</span><span class="sxs-lookup"><span data-stu-id="aa205-106">Represents a deleted item in the directory.</span></span> <span data-ttu-id="aa205-107">アイテムが削除されると、そのアイテムは削除済みアイテムの「コンテナー」に追加されます。</span><span class="sxs-lookup"><span data-stu-id="aa205-107">When an item is deleted, it is added to the deleted items "container".</span></span> <span data-ttu-id="aa205-108">削除されたアイテムは、最大 30 日間、復元可能な状態に維持されます。</span><span class="sxs-lookup"><span data-stu-id="aa205-108">Deleted items will remain available to restore for up to 30 days.</span></span> <span data-ttu-id="aa205-109">30 日が経過すると、アイテムは完全に削除されます。</span><span class="sxs-lookup"><span data-stu-id="aa205-109">After 30 days, the items are permanently deleted.</span></span>

<span data-ttu-id="aa205-110">現在、[削除済みアイテム] 機能は Office 365 の [group](group.md) および [user](users.md) リソースに対してのみサポートされています。</span><span class="sxs-lookup"><span data-stu-id="aa205-110">Currently, deleted items functionality is only supported for Office 365 [groups](group.md) and [users](users.md).</span></span>

## <a name="methods"></a><span data-ttu-id="aa205-111">メソッド</span><span class="sxs-lookup"><span data-stu-id="aa205-111">Methods</span></span>

| <span data-ttu-id="aa205-112">メソッド</span><span class="sxs-lookup"><span data-stu-id="aa205-112">Method</span></span>         | <span data-ttu-id="aa205-113">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="aa205-113">Return Type</span></span> | <span data-ttu-id="aa205-114">説明</span><span class="sxs-lookup"><span data-stu-id="aa205-114">Description</span></span> |
|:---------------|:------------|:------------|
|[<span data-ttu-id="aa205-115">削除済みアイテムの取得</span><span class="sxs-lookup"><span data-stu-id="aa205-115">Get deleted item</span></span>](../api/directory-deleteditems-get.md) | [<span data-ttu-id="aa205-116">directoryObject</span><span class="sxs-lookup"><span data-stu-id="aa205-116">directoryObject</span></span>](directoryobject.md) | <span data-ttu-id="aa205-117">削除済みアイテムのプロパティを取得します。</span><span class="sxs-lookup"><span data-stu-id="aa205-117">Gets the properties of a deleted item.</span></span> |
|[<span data-ttu-id="aa205-118">削除済みアイテムの復元</span><span class="sxs-lookup"><span data-stu-id="aa205-118">Restore deleted item</span></span>](../api/directory-deleteditems-restore.md) |[<span data-ttu-id="aa205-119">directoryObject</span><span class="sxs-lookup"><span data-stu-id="aa205-119">directoryObject</span></span>](directoryobject.md)| <span data-ttu-id="aa205-120">最近削除されたアイテムを復元します。</span><span class="sxs-lookup"><span data-stu-id="aa205-120">Restores a recently deleted item.</span></span> |
|[<span data-ttu-id="aa205-121">削除済みアイテムの一覧表示</span><span class="sxs-lookup"><span data-stu-id="aa205-121">List deleted items</span></span>](../api/directory-deleteditems-list.md) |<span data-ttu-id="aa205-122">[directoryObject](directoryobject.md) collection</span><span class="sxs-lookup"><span data-stu-id="aa205-122">[directoryObject](directoryobject.md) collection</span></span>| <span data-ttu-id="aa205-123">最近削除されたアイテムのリストを取得します。</span><span class="sxs-lookup"><span data-stu-id="aa205-123">Gets a list of recently deleted items.</span></span> |
|[<span data-ttu-id="aa205-124">アイテムの完全削除</span><span class="sxs-lookup"><span data-stu-id="aa205-124">Permanently delete an item</span></span>](../api/directory-deleteditems-delete.md) | <span data-ttu-id="aa205-125">なし</span><span class="sxs-lookup"><span data-stu-id="aa205-125">None</span></span> | <span data-ttu-id="aa205-126">アイテムを完全に削除します。</span><span class="sxs-lookup"><span data-stu-id="aa205-126">Permanently deletes an item.</span></span> |
|[<span data-ttu-id="aa205-127">ユーザーが所有する削除済みアイテムを一覧表示する</span><span class="sxs-lookup"><span data-stu-id="aa205-127">List deleted items owned by a user</span></span>](../api/directory-deleteditems-user-owned.md) | <span data-ttu-id="aa205-128">[directoryObject](directoryobject.md) collection</span><span class="sxs-lookup"><span data-stu-id="aa205-128">[directoryObject](directoryobject.md) collection</span></span> | <span data-ttu-id="aa205-129">ユーザーが所有しているディレクトリアイテムを一覧表示します。</span><span class="sxs-lookup"><span data-stu-id="aa205-129">Lists directory items owned by a user.</span></span> |

## <a name="properties"></a><span data-ttu-id="aa205-130">プロパティ</span><span class="sxs-lookup"><span data-stu-id="aa205-130">Properties</span></span>
| <span data-ttu-id="aa205-131">プロパティ</span><span class="sxs-lookup"><span data-stu-id="aa205-131">Property</span></span>   | <span data-ttu-id="aa205-132">型</span><span class="sxs-lookup"><span data-stu-id="aa205-132">Type</span></span> |<span data-ttu-id="aa205-133">説明</span><span class="sxs-lookup"><span data-stu-id="aa205-133">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="aa205-134">id</span><span class="sxs-lookup"><span data-stu-id="aa205-134">id</span></span>|<span data-ttu-id="aa205-135">String</span><span class="sxs-lookup"><span data-stu-id="aa205-135">String</span></span>| <span data-ttu-id="aa205-136">オブジェクトの一意識別子 (例: 12345678-9abc-def0-1234-56789abcde)。</span><span class="sxs-lookup"><span data-stu-id="aa205-136">A unique identifier for the object; for example, 12345678-9abc-def0-1234-56789abcde.</span></span> <span data-ttu-id="aa205-137">キー。</span><span class="sxs-lookup"><span data-stu-id="aa205-137">Key.</span></span> <span data-ttu-id="aa205-138">null 許容ではありません。</span><span class="sxs-lookup"><span data-stu-id="aa205-138">Not nullable.</span></span> <span data-ttu-id="aa205-139">読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="aa205-139">Read-only.</span></span>|

## <a name="relationships"></a><span data-ttu-id="aa205-140">関係</span><span class="sxs-lookup"><span data-stu-id="aa205-140">Relationships</span></span>
| <span data-ttu-id="aa205-141">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="aa205-141">Relationship</span></span> | <span data-ttu-id="aa205-142">型</span><span class="sxs-lookup"><span data-stu-id="aa205-142">Type</span></span>   |<span data-ttu-id="aa205-143">説明</span><span class="sxs-lookup"><span data-stu-id="aa205-143">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="aa205-144">deleteditems</span><span class="sxs-lookup"><span data-stu-id="aa205-144">deleteditems</span></span>|<span data-ttu-id="aa205-145">[directoryObject](directoryobject.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="aa205-145">[directoryObject](directoryobject.md) collection</span></span>| <span data-ttu-id="aa205-146">最近削除されたアイテム</span><span class="sxs-lookup"><span data-stu-id="aa205-146">Recently deleted items.</span></span> <span data-ttu-id="aa205-147">読み取り専用。</span><span class="sxs-lookup"><span data-stu-id="aa205-147">Read-only.</span></span> <span data-ttu-id="aa205-148">Null 許容型。</span><span class="sxs-lookup"><span data-stu-id="aa205-148">Nullable.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="aa205-149">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="aa205-149">JSON representation</span></span>
<span data-ttu-id="aa205-150">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="aa205-150">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "keyProperty":"id",
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
<!--
{
  "type": "#page.annotation",
  "description": "directory resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
