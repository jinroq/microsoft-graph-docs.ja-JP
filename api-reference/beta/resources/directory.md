---
title: directory リソースの種類 (削除済みアイテム)
description: . 削除されたアイテムは、最大 30 日間、復元可能な状態に維持されます。 30 日が経過すると、アイテムは完全に削除されます。
localization_priority: Normal
author: lleonard-msft
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 2593603afa145d30b5e26a240bb5cd471eab9942
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/12/2019
ms.locfileid: "27966553"
---
# <a name="directory-resource-type-deleted-items"></a><span data-ttu-id="e5633-105">directory リソースの種類 (削除済みアイテム)</span><span class="sxs-lookup"><span data-stu-id="e5633-105">directory resource type (deleted items)</span></span>

> <span data-ttu-id="e5633-106">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="e5633-106">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="e5633-107">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="e5633-107">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="e5633-108">ディレクトリ内の削除済みアイテムを表します。</span><span class="sxs-lookup"><span data-stu-id="e5633-108">Represents a deleted item in the directory.</span></span> <span data-ttu-id="e5633-109">アイテムが削除されると、そのアイテムは削除済みアイテムの「コンテナー」に追加されます。</span><span class="sxs-lookup"><span data-stu-id="e5633-109">When an item is deleted, it is added to the deleted items "container".</span></span> <span data-ttu-id="e5633-110">削除されたアイテムは、最大 30 日間、復元可能な状態に維持されます。</span><span class="sxs-lookup"><span data-stu-id="e5633-110">Deleted items will remain available to restore for up to 30 days.</span></span> <span data-ttu-id="e5633-111">30 日が経過すると、アイテムは完全に削除されます。</span><span class="sxs-lookup"><span data-stu-id="e5633-111">After 30 days, the items are permanently deleted.</span></span>

<span data-ttu-id="e5633-112">現在、[削除済みアイテム] 機能は Office 365 の [group](group.md) および [user](users.md) リソースに対してのみサポートされています。</span><span class="sxs-lookup"><span data-stu-id="e5633-112">Currently, deleted items functionality is only supported for Office 365 [groups](group.md) and [users](users.md).</span></span>

## <a name="methods"></a><span data-ttu-id="e5633-113">メソッド</span><span class="sxs-lookup"><span data-stu-id="e5633-113">Methods</span></span>

| <span data-ttu-id="e5633-114">メソッド</span><span class="sxs-lookup"><span data-stu-id="e5633-114">Method</span></span>         | <span data-ttu-id="e5633-115">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="e5633-115">Return Type</span></span> | <span data-ttu-id="e5633-116">説明</span><span class="sxs-lookup"><span data-stu-id="e5633-116">Description</span></span> |
|:---------------|:------------|:------------|
|[<span data-ttu-id="e5633-117">削除済みアイテムの取得</span><span class="sxs-lookup"><span data-stu-id="e5633-117">Get deleted item</span></span>](../api/directory-deleteditems-get.md) | [<span data-ttu-id="e5633-118">directoryObject</span><span class="sxs-lookup"><span data-stu-id="e5633-118">directoryObject</span></span>](directoryobject.md) | <span data-ttu-id="e5633-119">削除済みアイテムのプロパティを取得します。</span><span class="sxs-lookup"><span data-stu-id="e5633-119">Gets the properties of a deleted item.</span></span> |
|[<span data-ttu-id="e5633-120">削除済みアイテムの復元</span><span class="sxs-lookup"><span data-stu-id="e5633-120">Restore deleted item</span></span>](../api/directory-deleteditems-restore.md) |[<span data-ttu-id="e5633-121">directoryObject</span><span class="sxs-lookup"><span data-stu-id="e5633-121">directoryObject</span></span>](directoryobject.md)| <span data-ttu-id="e5633-122">最近削除されたアイテムを復元します。</span><span class="sxs-lookup"><span data-stu-id="e5633-122">Restores a recently deleted item.</span></span> |
|[<span data-ttu-id="e5633-123">削除済みアイテムの一覧表示</span><span class="sxs-lookup"><span data-stu-id="e5633-123">List deleted items</span></span>](../api/directory-deleteditems-list.md) |<span data-ttu-id="e5633-124">[directoryObject](directoryobject.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="e5633-124">[directoryObject](directoryobject.md) collection</span></span>| <span data-ttu-id="e5633-125">最近削除されたアイテムのリストを取得します。</span><span class="sxs-lookup"><span data-stu-id="e5633-125">Gets a list of recently deleted items.</span></span> |
|[<span data-ttu-id="e5633-126">アイテムの完全削除</span><span class="sxs-lookup"><span data-stu-id="e5633-126">Permanently delete an item</span></span>](../api/directory-deleteditems-delete.md) | <span data-ttu-id="e5633-127">なし</span><span class="sxs-lookup"><span data-stu-id="e5633-127">None</span></span> | <span data-ttu-id="e5633-128">アイテムを完全に削除します。</span><span class="sxs-lookup"><span data-stu-id="e5633-128">Permanently deletes an item.</span></span> |
|[<span data-ttu-id="e5633-129">ユーザーによって所有されている削除済みのアイテムを一覧表示します。</span><span class="sxs-lookup"><span data-stu-id="e5633-129">List deleted items owned by a user</span></span>](../api/directory-deleteditems-user-owned.md) | <span data-ttu-id="e5633-130">[directoryObject](directoryobject.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="e5633-130">[directoryObject](directoryobject.md) collection</span></span> | <span data-ttu-id="e5633-131">ユーザーによって所有されているディレクトリの項目を一覧表示します。</span><span class="sxs-lookup"><span data-stu-id="e5633-131">Lists directory items owned by a user.</span></span> |

## <a name="properties"></a><span data-ttu-id="e5633-132">プロパティ</span><span class="sxs-lookup"><span data-stu-id="e5633-132">Properties</span></span>
| <span data-ttu-id="e5633-133">プロパティ</span><span class="sxs-lookup"><span data-stu-id="e5633-133">Property</span></span>   | <span data-ttu-id="e5633-134">種類</span><span class="sxs-lookup"><span data-stu-id="e5633-134">Type</span></span> |<span data-ttu-id="e5633-135">説明</span><span class="sxs-lookup"><span data-stu-id="e5633-135">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="e5633-136">ID</span><span class="sxs-lookup"><span data-stu-id="e5633-136">id</span></span>|<span data-ttu-id="e5633-137">String</span><span class="sxs-lookup"><span data-stu-id="e5633-137">String</span></span>| <span data-ttu-id="e5633-138">オブジェクトの一意識別子 (例: 12345678-9abc-def0-1234-56789abcde)。</span><span class="sxs-lookup"><span data-stu-id="e5633-138">A unique identifier for the object; for example, 12345678-9abc-def0-1234-56789abcde.</span></span> <span data-ttu-id="e5633-139">キー。</span><span class="sxs-lookup"><span data-stu-id="e5633-139">Key.</span></span> <span data-ttu-id="e5633-140">null 許容ではありません。</span><span class="sxs-lookup"><span data-stu-id="e5633-140">Not nullable.</span></span> <span data-ttu-id="e5633-141">読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="e5633-141">Read-only.</span></span>|

## <a name="relationships"></a><span data-ttu-id="e5633-142">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="e5633-142">Relationships</span></span>
| <span data-ttu-id="e5633-143">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="e5633-143">Relationship</span></span> | <span data-ttu-id="e5633-144">型</span><span class="sxs-lookup"><span data-stu-id="e5633-144">Type</span></span>   |<span data-ttu-id="e5633-145">説明</span><span class="sxs-lookup"><span data-stu-id="e5633-145">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="e5633-146">deleteditems</span><span class="sxs-lookup"><span data-stu-id="e5633-146">deleteditems</span></span>|<span data-ttu-id="e5633-147">[directoryObject](directoryobject.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="e5633-147">[directoryObject](directoryobject.md) collection</span></span>| <span data-ttu-id="e5633-148">最近削除されたアイテム</span><span class="sxs-lookup"><span data-stu-id="e5633-148">Recently deleted items.</span></span> <span data-ttu-id="e5633-149">読み取り専用。</span><span class="sxs-lookup"><span data-stu-id="e5633-149">Read-only.</span></span> <span data-ttu-id="e5633-150">Null 許容型。</span><span class="sxs-lookup"><span data-stu-id="e5633-150">Nullable.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="e5633-151">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="e5633-151">JSON representation</span></span>
<span data-ttu-id="e5633-152">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="e5633-152">Here is a JSON representation of the resource.</span></span>

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
