---
title: directory リソースの種類 (削除済みアイテム)
description: . 削除されたアイテムは、最大 30 日間、復元可能な状態に維持されます。 30 日が経過すると、アイテムは完全に削除されます。
ms.openlocfilehash: 74b4d1ff94b567557fd90701b1c4bae479a8317e
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27073673"
---
# <a name="directory-resource-type-deleted-items"></a><span data-ttu-id="d522c-105">directory リソースの種類 (削除済みアイテム)</span><span class="sxs-lookup"><span data-stu-id="d522c-105">directory resource type (deleted items)</span></span>

> <span data-ttu-id="d522c-106">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="d522c-106">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="d522c-107">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="d522c-107">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="d522c-108">ディレクトリ内の削除済みアイテムを表します。</span><span class="sxs-lookup"><span data-stu-id="d522c-108">Represents a deleted item in the directory.</span></span> <span data-ttu-id="d522c-109">アイテムが削除されると、そのアイテムは削除済みアイテムの「コンテナー」に追加されます。</span><span class="sxs-lookup"><span data-stu-id="d522c-109">When an item is deleted, it is added to the deleted items "container".</span></span> <span data-ttu-id="d522c-110">削除されたアイテムは、最大 30 日間、復元可能な状態に維持されます。</span><span class="sxs-lookup"><span data-stu-id="d522c-110">Deleted items will remain available to restore for up to 30 days.</span></span> <span data-ttu-id="d522c-111">30 日が経過すると、アイテムは完全に削除されます。</span><span class="sxs-lookup"><span data-stu-id="d522c-111">After 30 days, the items are permanently deleted.</span></span>

<span data-ttu-id="d522c-112">現在、[削除済みアイテム] 機能は Office 365 の [group](group.md) および [user](users.md) リソースに対してのみサポートされています。</span><span class="sxs-lookup"><span data-stu-id="d522c-112">Currently, deleted items functionality is only supported for Office 365 [groups](group.md) and [users](users.md).</span></span>

## <a name="methods"></a><span data-ttu-id="d522c-113">メソッド</span><span class="sxs-lookup"><span data-stu-id="d522c-113">Methods</span></span>

| <span data-ttu-id="d522c-114">メソッド</span><span class="sxs-lookup"><span data-stu-id="d522c-114">Method</span></span>         | <span data-ttu-id="d522c-115">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="d522c-115">Return Type</span></span> | <span data-ttu-id="d522c-116">説明</span><span class="sxs-lookup"><span data-stu-id="d522c-116">Description</span></span> |
|:---------------|:------------|:------------|
|[<span data-ttu-id="d522c-117">削除済みアイテムの取得</span><span class="sxs-lookup"><span data-stu-id="d522c-117">Get deleted item</span></span>](../api/directory-deleteditems-get.md) | [<span data-ttu-id="d522c-118">directoryObject</span><span class="sxs-lookup"><span data-stu-id="d522c-118">directoryObject</span></span>](directoryobject.md) | <span data-ttu-id="d522c-119">削除済みアイテムのプロパティを取得します。</span><span class="sxs-lookup"><span data-stu-id="d522c-119">Gets the properties of a deleted item.</span></span> |
|[<span data-ttu-id="d522c-120">削除済みアイテムの復元</span><span class="sxs-lookup"><span data-stu-id="d522c-120">Restore deleted item</span></span>](../api/directory-deleteditems-restore.md) |[<span data-ttu-id="d522c-121">directoryObject</span><span class="sxs-lookup"><span data-stu-id="d522c-121">directoryObject</span></span>](directoryobject.md)| <span data-ttu-id="d522c-122">最近削除されたアイテムを復元します。</span><span class="sxs-lookup"><span data-stu-id="d522c-122">Restores a recently deleted item.</span></span> |
|[<span data-ttu-id="d522c-123">削除済みアイテムの一覧表示</span><span class="sxs-lookup"><span data-stu-id="d522c-123">List deleted items</span></span>](../api/directory-deleteditems-list.md) |<span data-ttu-id="d522c-124">[directoryObject](directoryobject.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="d522c-124">[directoryObject](directoryobject.md) collection</span></span>| <span data-ttu-id="d522c-125">最近削除されたアイテムのリストを取得します。</span><span class="sxs-lookup"><span data-stu-id="d522c-125">Gets a list of recently deleted items.</span></span> |
|[<span data-ttu-id="d522c-126">アイテムの完全削除</span><span class="sxs-lookup"><span data-stu-id="d522c-126">Permanently delete an item</span></span>](../api/directory-deleteditems-delete.md) | <span data-ttu-id="d522c-127">なし</span><span class="sxs-lookup"><span data-stu-id="d522c-127">None</span></span> | <span data-ttu-id="d522c-128">アイテムを完全に削除します。</span><span class="sxs-lookup"><span data-stu-id="d522c-128">Permanently deletes an item.</span></span> |
|[<span data-ttu-id="d522c-129">ユーザーによって所有されている削除済みのアイテムを一覧表示します。</span><span class="sxs-lookup"><span data-stu-id="d522c-129">List deleted items owned by a user</span></span>](../api/directory-deleteditems-user-owned.md) | <span data-ttu-id="d522c-130">[directoryObject](directoryobject.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="d522c-130">[directoryObject](directoryobject.md) collection</span></span> | <span data-ttu-id="d522c-131">ユーザーによって所有されているディレクトリの項目を一覧表示します。</span><span class="sxs-lookup"><span data-stu-id="d522c-131">Lists directory items owned by a user.</span></span> |

## <a name="properties"></a><span data-ttu-id="d522c-132">プロパティ</span><span class="sxs-lookup"><span data-stu-id="d522c-132">Properties</span></span>
| <span data-ttu-id="d522c-133">プロパティ</span><span class="sxs-lookup"><span data-stu-id="d522c-133">Property</span></span>   | <span data-ttu-id="d522c-134">型</span><span class="sxs-lookup"><span data-stu-id="d522c-134">Type</span></span> |<span data-ttu-id="d522c-135">説明</span><span class="sxs-lookup"><span data-stu-id="d522c-135">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="d522c-136">id</span><span class="sxs-lookup"><span data-stu-id="d522c-136">id</span></span>|<span data-ttu-id="d522c-137">String</span><span class="sxs-lookup"><span data-stu-id="d522c-137">String</span></span>| <span data-ttu-id="d522c-138">オブジェクトの一意識別子 (例: 12345678-9abc-def0-1234-56789abcde)。</span><span class="sxs-lookup"><span data-stu-id="d522c-138">A unique identifier for the object; for example, 12345678-9abc-def0-1234-56789abcde.</span></span> <span data-ttu-id="d522c-139">キー。</span><span class="sxs-lookup"><span data-stu-id="d522c-139">Key.</span></span> <span data-ttu-id="d522c-140">null 許容ではありません。</span><span class="sxs-lookup"><span data-stu-id="d522c-140">Not nullable.</span></span> <span data-ttu-id="d522c-141">読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="d522c-141">Read-only.</span></span>|

## <a name="relationships"></a><span data-ttu-id="d522c-142">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="d522c-142">Relationships</span></span>
| <span data-ttu-id="d522c-143">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="d522c-143">Relationship</span></span> | <span data-ttu-id="d522c-144">型</span><span class="sxs-lookup"><span data-stu-id="d522c-144">Type</span></span>   |<span data-ttu-id="d522c-145">説明</span><span class="sxs-lookup"><span data-stu-id="d522c-145">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="d522c-146">deleteditems</span><span class="sxs-lookup"><span data-stu-id="d522c-146">deleteditems</span></span>|<span data-ttu-id="d522c-147">[directoryObject](directoryobject.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="d522c-147">[directoryObject](directoryobject.md) collection</span></span>| <span data-ttu-id="d522c-148">最近削除されたアイテム</span><span class="sxs-lookup"><span data-stu-id="d522c-148">Recently deleted items.</span></span> <span data-ttu-id="d522c-149">読み取り専用。</span><span class="sxs-lookup"><span data-stu-id="d522c-149">Read-only.</span></span> <span data-ttu-id="d522c-150">Null 許容型。</span><span class="sxs-lookup"><span data-stu-id="d522c-150">Nullable.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="d522c-151">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="d522c-151">JSON representation</span></span>
<span data-ttu-id="d522c-152">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="d522c-152">Here is a JSON representation of the resource.</span></span>

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