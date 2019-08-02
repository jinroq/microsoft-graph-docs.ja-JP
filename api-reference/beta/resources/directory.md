---
title: directory リソースの種類 (削除済みアイテム)
description: . 削除されたアイテムは、最大 30 日間、復元可能な状態に維持されます。 30 日が経過すると、アイテムは完全に削除されます。
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 4b35c2c56c7033cd668b311c17169f5c719e5948
ms.sourcegitcommit: bbed891d16995b4a8ce866169dddb96abdc28776
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/02/2019
ms.locfileid: "36062083"
---
# <a name="directory-resource-type-deleted-items"></a><span data-ttu-id="7d72c-105">directory リソースの種類 (削除済みアイテム)</span><span class="sxs-lookup"><span data-stu-id="7d72c-105">directory resource type (deleted items)</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="7d72c-106">ディレクトリ内の削除済みアイテムを表します。</span><span class="sxs-lookup"><span data-stu-id="7d72c-106">Represents a deleted item in the directory.</span></span> <span data-ttu-id="7d72c-107">アイテムが削除されると、そのアイテムは削除済みアイテムの「コンテナー」に追加されます。</span><span class="sxs-lookup"><span data-stu-id="7d72c-107">When an item is deleted, it is added to the deleted items "container".</span></span> <span data-ttu-id="7d72c-108">削除されたアイテムは、最大 30 日間、復元可能な状態に維持されます。</span><span class="sxs-lookup"><span data-stu-id="7d72c-108">Deleted items will remain available to restore for up to 30 days.</span></span> <span data-ttu-id="7d72c-109">30 日が経過すると、アイテムは完全に削除されます。</span><span class="sxs-lookup"><span data-stu-id="7d72c-109">After 30 days, the items are permanently deleted.</span></span>

<span data-ttu-id="7d72c-110">現在、[削除済みアイテム] 機能は Office 365 の [group](group.md) および [user](users.md) リソースに対してのみサポートされています。</span><span class="sxs-lookup"><span data-stu-id="7d72c-110">Currently, deleted items functionality is only supported for Office 365 [groups](group.md) and [users](users.md).</span></span>

## <a name="methods"></a><span data-ttu-id="7d72c-111">メソッド</span><span class="sxs-lookup"><span data-stu-id="7d72c-111">Methods</span></span>

| <span data-ttu-id="7d72c-112">メソッド</span><span class="sxs-lookup"><span data-stu-id="7d72c-112">Method</span></span>         | <span data-ttu-id="7d72c-113">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="7d72c-113">Return Type</span></span> | <span data-ttu-id="7d72c-114">説明</span><span class="sxs-lookup"><span data-stu-id="7d72c-114">Description</span></span> |
|:---------------|:------------|:------------|
|[<span data-ttu-id="7d72c-115">削除済みアイテムの取得</span><span class="sxs-lookup"><span data-stu-id="7d72c-115">Get deleted item</span></span>](../api/directory-deleteditems-get.md) | [<span data-ttu-id="7d72c-116">directoryObject</span><span class="sxs-lookup"><span data-stu-id="7d72c-116">directoryObject</span></span>](directoryobject.md) | <span data-ttu-id="7d72c-117">削除済みアイテムのプロパティを取得します。</span><span class="sxs-lookup"><span data-stu-id="7d72c-117">Gets the properties of a deleted item.</span></span> |
|[<span data-ttu-id="7d72c-118">削除済みアイテムの復元</span><span class="sxs-lookup"><span data-stu-id="7d72c-118">Restore deleted item</span></span>](../api/directory-deleteditems-restore.md) |[<span data-ttu-id="7d72c-119">directoryObject</span><span class="sxs-lookup"><span data-stu-id="7d72c-119">directoryObject</span></span>](directoryobject.md)| <span data-ttu-id="7d72c-120">最近削除されたアイテムを復元します。</span><span class="sxs-lookup"><span data-stu-id="7d72c-120">Restores a recently deleted item.</span></span> |
|[<span data-ttu-id="7d72c-121">削除済みアイテムの一覧表示</span><span class="sxs-lookup"><span data-stu-id="7d72c-121">List deleted items</span></span>](../api/directory-deleteditems-list.md) |<span data-ttu-id="7d72c-122">[directoryObject](directoryobject.md) collection</span><span class="sxs-lookup"><span data-stu-id="7d72c-122">[directoryObject](directoryobject.md) collection</span></span>| <span data-ttu-id="7d72c-123">最近削除されたアイテムのリストを取得します。</span><span class="sxs-lookup"><span data-stu-id="7d72c-123">Gets a list of recently deleted items.</span></span> |
|[<span data-ttu-id="7d72c-124">アイテムの完全削除</span><span class="sxs-lookup"><span data-stu-id="7d72c-124">Permanently delete an item</span></span>](../api/directory-deleteditems-delete.md) | <span data-ttu-id="7d72c-125">なし</span><span class="sxs-lookup"><span data-stu-id="7d72c-125">None</span></span> | <span data-ttu-id="7d72c-126">アイテムを完全に削除します。</span><span class="sxs-lookup"><span data-stu-id="7d72c-126">Permanently deletes an item.</span></span> |
|[<span data-ttu-id="7d72c-127">ユーザーが所有する削除済みアイテムを一覧表示する</span><span class="sxs-lookup"><span data-stu-id="7d72c-127">List deleted items owned by a user</span></span>](../api/directory-deleteditems-user-owned.md) | <span data-ttu-id="7d72c-128">[directoryObject](directoryobject.md) collection</span><span class="sxs-lookup"><span data-stu-id="7d72c-128">[directoryObject](directoryobject.md) collection</span></span> | <span data-ttu-id="7d72c-129">ユーザーが所有しているディレクトリアイテムを一覧表示します。</span><span class="sxs-lookup"><span data-stu-id="7d72c-129">Lists directory items owned by a user.</span></span> |
|[<span data-ttu-id="7d72c-130">リスト featureRolloutPolicies</span><span class="sxs-lookup"><span data-stu-id="7d72c-130">List featureRolloutPolicies</span></span>](../api/directory-list-featurerolloutpolicies.md) | <span data-ttu-id="7d72c-131">[featureRolloutPolicy](featurerolloutpolicy.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="7d72c-131">[featureRolloutPolicy](featurerolloutpolicy.md) collection</span></span> | <span data-ttu-id="7d72c-132">FeatureRolloutPolicy オブジェクトのリストを取得します。</span><span class="sxs-lookup"><span data-stu-id="7d72c-132">Retrieve a list of featureRolloutPolicy objects.</span></span> |
|[<span data-ttu-id="7d72c-133">FeatureRolloutPolicy を作成する</span><span class="sxs-lookup"><span data-stu-id="7d72c-133">Create featureRolloutPolicy</span></span>](../api/directory-post-featurerolloutpolicies.md) | [<span data-ttu-id="7d72c-134">featureRolloutPolicy</span><span class="sxs-lookup"><span data-stu-id="7d72c-134">featureRolloutPolicy</span></span>](featurerolloutpolicy.md) | <span data-ttu-id="7d72c-135">新しい featureRolloutPolicy オブジェクトを作成します。</span><span class="sxs-lookup"><span data-stu-id="7d72c-135">Create a new featureRolloutPolicy object.</span></span> |
| [<span data-ttu-id="7d72c-136">FeatureRolloutPolicy を取得する</span><span class="sxs-lookup"><span data-stu-id="7d72c-136">Get featureRolloutPolicy</span></span>](../api/featurerolloutpolicy-get.md) | [<span data-ttu-id="7d72c-137">featureRolloutPolicy</span><span class="sxs-lookup"><span data-stu-id="7d72c-137">featureRolloutPolicy</span></span>](featurerolloutpolicy.md) | <span data-ttu-id="7d72c-138">Featurerolloutpolicy オブジェクトのプロパティとリレーションシップを取得します。</span><span class="sxs-lookup"><span data-stu-id="7d72c-138">Retrieve the properties and relationships of featurerolloutpolicy object.</span></span> |
| [<span data-ttu-id="7d72c-139">FeatureRolloutPolicy の更新</span><span class="sxs-lookup"><span data-stu-id="7d72c-139">Update featureRolloutPolicy</span></span>](../api/featurerolloutpolicy-update.md) | [<span data-ttu-id="7d72c-140">featureRolloutPolicy</span><span class="sxs-lookup"><span data-stu-id="7d72c-140">featureRolloutPolicy</span></span>](featurerolloutpolicy.md) | <span data-ttu-id="7d72c-141">Featurerolloutpolicy オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="7d72c-141">Update the properties of featurerolloutpolicy object.</span></span> |
| [<span data-ttu-id="7d72c-142">FeatureRolloutPolicy の削除</span><span class="sxs-lookup"><span data-stu-id="7d72c-142">Delete featureRolloutPolicy</span></span>](../api/featurerolloutpolicy-delete.md) | <span data-ttu-id="7d72c-143">None</span><span class="sxs-lookup"><span data-stu-id="7d72c-143">None</span></span> | <span data-ttu-id="7d72c-144">FeatureRolloutPolicy オブジェクトを削除します。</span><span class="sxs-lookup"><span data-stu-id="7d72c-144">Delete a featureRolloutPolicy object.</span></span> |

## <a name="properties"></a><span data-ttu-id="7d72c-145">プロパティ</span><span class="sxs-lookup"><span data-stu-id="7d72c-145">Properties</span></span>
| <span data-ttu-id="7d72c-146">プロパティ</span><span class="sxs-lookup"><span data-stu-id="7d72c-146">Property</span></span>   | <span data-ttu-id="7d72c-147">型</span><span class="sxs-lookup"><span data-stu-id="7d72c-147">Type</span></span> |<span data-ttu-id="7d72c-148">説明</span><span class="sxs-lookup"><span data-stu-id="7d72c-148">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="7d72c-149">id</span><span class="sxs-lookup"><span data-stu-id="7d72c-149">id</span></span>|<span data-ttu-id="7d72c-150">String</span><span class="sxs-lookup"><span data-stu-id="7d72c-150">String</span></span>| <span data-ttu-id="7d72c-151">オブジェクトの一意識別子 (例: 12345678-9abc-def0-1234-56789abcde)。</span><span class="sxs-lookup"><span data-stu-id="7d72c-151">A unique identifier for the object; for example, 12345678-9abc-def0-1234-56789abcde.</span></span> <span data-ttu-id="7d72c-152">キー。</span><span class="sxs-lookup"><span data-stu-id="7d72c-152">Key.</span></span> <span data-ttu-id="7d72c-153">null 許容ではありません。</span><span class="sxs-lookup"><span data-stu-id="7d72c-153">Not nullable.</span></span> <span data-ttu-id="7d72c-154">読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="7d72c-154">Read-only.</span></span>|

## <a name="relationships"></a><span data-ttu-id="7d72c-155">関係</span><span class="sxs-lookup"><span data-stu-id="7d72c-155">Relationships</span></span>
| <span data-ttu-id="7d72c-156">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="7d72c-156">Relationship</span></span> | <span data-ttu-id="7d72c-157">型</span><span class="sxs-lookup"><span data-stu-id="7d72c-157">Type</span></span>   |<span data-ttu-id="7d72c-158">説明</span><span class="sxs-lookup"><span data-stu-id="7d72c-158">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="7d72c-159">deleteditems</span><span class="sxs-lookup"><span data-stu-id="7d72c-159">deleteditems</span></span>|<span data-ttu-id="7d72c-160">[directoryObject](directoryobject.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="7d72c-160">[directoryObject](directoryobject.md) collection</span></span>| <span data-ttu-id="7d72c-161">最近削除されたアイテム</span><span class="sxs-lookup"><span data-stu-id="7d72c-161">Recently deleted items.</span></span> <span data-ttu-id="7d72c-162">読み取り専用。</span><span class="sxs-lookup"><span data-stu-id="7d72c-162">Read-only.</span></span> <span data-ttu-id="7d72c-163">Null 許容型。</span><span class="sxs-lookup"><span data-stu-id="7d72c-163">Nullable.</span></span>|
|<span data-ttu-id="7d72c-164">featureRolloutPolicies</span><span class="sxs-lookup"><span data-stu-id="7d72c-164">featureRolloutPolicies</span></span>|<span data-ttu-id="7d72c-165">[featureRolloutPolicy](featurerolloutpolicy.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="7d72c-165">[featureRolloutPolicy](featurerolloutpolicy.md) collection</span></span>| <span data-ttu-id="7d72c-166">Null 許容型。</span><span class="sxs-lookup"><span data-stu-id="7d72c-166">Nullable.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="7d72c-167">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="7d72c-167">JSON representation</span></span>
<span data-ttu-id="7d72c-168">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="7d72c-168">Here is a JSON representation of the resource.</span></span>

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
