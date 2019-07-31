---
title: アイテムリソースの種類
description: Dynamics 365 Business Central の item オブジェクト。
services: project-madeira
documentationcenter: ''
author: SusanneWindfeldPedersen
localization_priority: Normal
ms.prod: dynamics-365-business-central
doc_type: resourcePageType
ms.openlocfilehash: 438fa0035b2c84b6fe702e3b1765e3d8b5adaf9d
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "36006627"
---
# <a name="items-resource-type"></a><span data-ttu-id="43fdd-103">アイテムリソースの種類</span><span class="sxs-lookup"><span data-stu-id="43fdd-103">items resource type</span></span>
<span data-ttu-id="43fdd-104">Dynamics 365 Business Central のアイテムを表します。</span><span class="sxs-lookup"><span data-stu-id="43fdd-104">Represents an item in Dynamics 365 Business Central.</span></span>

## <a name="methods"></a><span data-ttu-id="43fdd-105">メソッド</span><span class="sxs-lookup"><span data-stu-id="43fdd-105">Methods</span></span>

| <span data-ttu-id="43fdd-106">メソッド</span><span class="sxs-lookup"><span data-stu-id="43fdd-106">Method</span></span>                                      |<span data-ttu-id="43fdd-107">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="43fdd-107">Return Type</span></span>|<span data-ttu-id="43fdd-108">説明</span><span class="sxs-lookup"><span data-stu-id="43fdd-108">Description</span></span> |
|:--------------------------------------------|:----------|:-----------|
|[<span data-ttu-id="43fdd-109">項目を取得する</span><span class="sxs-lookup"><span data-stu-id="43fdd-109">Get items</span></span>](../api/dynamics-item-get.md)      |<span data-ttu-id="43fdd-110">items</span><span class="sxs-lookup"><span data-stu-id="43fdd-110">items</span></span>     |<span data-ttu-id="43fdd-111">アイテムオブジェクトを取得します。</span><span class="sxs-lookup"><span data-stu-id="43fdd-111">Gets an item object.</span></span>   |
|[<span data-ttu-id="43fdd-112">投稿アイテム</span><span class="sxs-lookup"><span data-stu-id="43fdd-112">Post items</span></span>](../api/dynamics-create-item.md)  |<span data-ttu-id="43fdd-113">items</span><span class="sxs-lookup"><span data-stu-id="43fdd-113">items</span></span>     |<span data-ttu-id="43fdd-114">アイテムオブジェクトを作成します。</span><span class="sxs-lookup"><span data-stu-id="43fdd-114">Creates an item object.</span></span>|
|[<span data-ttu-id="43fdd-115">Patch 項目</span><span class="sxs-lookup"><span data-stu-id="43fdd-115">Patch item</span></span>](../api/dynamics-item-update.md)  |<span data-ttu-id="43fdd-116">items</span><span class="sxs-lookup"><span data-stu-id="43fdd-116">items</span></span>     |<span data-ttu-id="43fdd-117">アイテムオブジェクトを更新します。</span><span class="sxs-lookup"><span data-stu-id="43fdd-117">Updates an item object.</span></span>|
|[<span data-ttu-id="43fdd-118">アイテムの削除</span><span class="sxs-lookup"><span data-stu-id="43fdd-118">Delete items</span></span>](../api/dynamics-item-delete.md)|<span data-ttu-id="43fdd-119">none</span><span class="sxs-lookup"><span data-stu-id="43fdd-119">none</span></span>      |<span data-ttu-id="43fdd-120">アイテムオブジェクトを削除します。</span><span class="sxs-lookup"><span data-stu-id="43fdd-120">Deletes an item object.</span></span>|

## <a name="properties"></a><span data-ttu-id="43fdd-121">プロパティ</span><span class="sxs-lookup"><span data-stu-id="43fdd-121">Properties</span></span>
| <span data-ttu-id="43fdd-122">プロパティ</span><span class="sxs-lookup"><span data-stu-id="43fdd-122">Property</span></span>           | <span data-ttu-id="43fdd-123">型</span><span class="sxs-lookup"><span data-stu-id="43fdd-123">Type</span></span> |<span data-ttu-id="43fdd-124">説明</span><span class="sxs-lookup"><span data-stu-id="43fdd-124">Description</span></span>                                          |
|:-------------------|:-------|:----------------------------------------------------|
|<span data-ttu-id="43fdd-125">id</span><span class="sxs-lookup"><span data-stu-id="43fdd-125">id</span></span>                  |<span data-ttu-id="43fdd-126">GUID</span><span class="sxs-lookup"><span data-stu-id="43fdd-126">GUID</span></span>    |<span data-ttu-id="43fdd-127">アイテムの一意の ID です。</span><span class="sxs-lookup"><span data-stu-id="43fdd-127">The unique ID of the item.</span></span> <span data-ttu-id="43fdd-128">編集できません。</span><span class="sxs-lookup"><span data-stu-id="43fdd-128">Non-editable.</span></span>             |
|<span data-ttu-id="43fdd-129">番号</span><span class="sxs-lookup"><span data-stu-id="43fdd-129">number</span></span>              |<span data-ttu-id="43fdd-130">string</span><span class="sxs-lookup"><span data-stu-id="43fdd-130">string</span></span>  |<span data-ttu-id="43fdd-131">アイテム番号を指定します。</span><span class="sxs-lookup"><span data-stu-id="43fdd-131">The item number.</span></span>                                     |
|<span data-ttu-id="43fdd-132">displayName</span><span class="sxs-lookup"><span data-stu-id="43fdd-132">displayName</span></span>         |<span data-ttu-id="43fdd-133">string</span><span class="sxs-lookup"><span data-stu-id="43fdd-133">string</span></span>  |<span data-ttu-id="43fdd-134">アイテムの説明を指定します。</span><span class="sxs-lookup"><span data-stu-id="43fdd-134">Specifies a description of the item.</span></span>                 |
|<span data-ttu-id="43fdd-135">type</span><span class="sxs-lookup"><span data-stu-id="43fdd-135">type</span></span>                |<span data-ttu-id="43fdd-136">数値</span><span class="sxs-lookup"><span data-stu-id="43fdd-136">numeric</span></span> |<span data-ttu-id="43fdd-137">アイテムの在庫の種類。</span><span class="sxs-lookup"><span data-stu-id="43fdd-137">The inventory type for the item.</span></span> <span data-ttu-id="43fdd-138">1 = 在庫アイテム、2 = サービスアイテム。</span><span class="sxs-lookup"><span data-stu-id="43fdd-138">1 = inventory item, 2 = service item.</span></span> <span data-ttu-id="43fdd-139">これは必須プロパティです。</span><span class="sxs-lookup"><span data-stu-id="43fdd-139">This is a required property.</span></span>|
|<span data-ttu-id="43fdd-140">ブロック</span><span class="sxs-lookup"><span data-stu-id="43fdd-140">blocked</span></span>             |<span data-ttu-id="43fdd-141">ブール値</span><span class="sxs-lookup"><span data-stu-id="43fdd-141">boolean</span></span> |<span data-ttu-id="43fdd-142">アイテムが検疫状態にあるなどの理由で、アイテムのトランザクションを投稿できないことを指定します。</span><span class="sxs-lookup"><span data-stu-id="43fdd-142">Specifies that transactions with the item cannot be posted, for example, because the item is in quarantine.</span></span> <span data-ttu-id="43fdd-143">アイテムがブロックされている場合は**true**に設定します。</span><span class="sxs-lookup"><span data-stu-id="43fdd-143">Set to **true**, if item is blocked.</span></span>|
|<span data-ttu-id="43fdd-144">baseUnitOfMeasureId</span><span class="sxs-lookup"><span data-stu-id="43fdd-144">baseUnitOfMeasureId</span></span> |<span data-ttu-id="43fdd-145">GUID</span><span class="sxs-lookup"><span data-stu-id="43fdd-145">GUID</span></span>    |<span data-ttu-id="43fdd-146">測定単位の ID を指定します。</span><span class="sxs-lookup"><span data-stu-id="43fdd-146">Specifies the ID of the unit of measure.</span></span>             |
|<span data-ttu-id="43fdd-147">baseUnitOfMeasure</span><span class="sxs-lookup"><span data-stu-id="43fdd-147">baseUnitOfMeasure</span></span>   |[<span data-ttu-id="43fdd-148">ナビゲーション.UnitOfMeasure</span><span class="sxs-lookup"><span data-stu-id="43fdd-148">NAV.UnitOfMeasure</span></span>](../resources/dynamics-complextypes.md)|<span data-ttu-id="43fdd-149">品目が在庫に保持される単位を指定します。</span><span class="sxs-lookup"><span data-stu-id="43fdd-149">Specifies the unit in which the item is held in inventory.</span></span>|
|<span data-ttu-id="43fdd-150">gtin</span><span class="sxs-lookup"><span data-stu-id="43fdd-150">gtin</span></span>                |<span data-ttu-id="43fdd-151">数値</span><span class="sxs-lookup"><span data-stu-id="43fdd-151">numeric</span></span> |<span data-ttu-id="43fdd-152">これは、グローバルな取引項目番号です。</span><span class="sxs-lookup"><span data-stu-id="43fdd-152">This is the Global Trade Item Number.</span></span>                |
|<span data-ttu-id="43fdd-153">itemCategoryId</span><span class="sxs-lookup"><span data-stu-id="43fdd-153">itemCategoryId</span></span>      |<span data-ttu-id="43fdd-154">GUID</span><span class="sxs-lookup"><span data-stu-id="43fdd-154">GUID</span></span> |<span data-ttu-id="43fdd-155">アイテムが属するカテゴリを指定します。</span><span class="sxs-lookup"><span data-stu-id="43fdd-155">Specifies the category that the item belongs to.</span></span> <span data-ttu-id="43fdd-156">アイテムカテゴリには、割り当てられたアイテム属性も含まれます。</span><span class="sxs-lookup"><span data-stu-id="43fdd-156">Item categories also contain any assigned item attributes.</span></span>|
|<span data-ttu-id="43fdd-157">inventory</span><span class="sxs-lookup"><span data-stu-id="43fdd-157">inventory</span></span>           |<span data-ttu-id="43fdd-158">decimal</span><span class="sxs-lookup"><span data-stu-id="43fdd-158">decimal</span></span> |<span data-ttu-id="43fdd-159">アイテムの、在庫にある、断片、箱、缶などの単位数を指定します。</span><span class="sxs-lookup"><span data-stu-id="43fdd-159">Specifies how many units, such as pieces, boxes, or cans, of the item are in inventory.</span></span> <span data-ttu-id="43fdd-160">読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="43fdd-160">Read-Only.</span></span>|
|<span data-ttu-id="43fdd-161">販売</span><span class="sxs-lookup"><span data-stu-id="43fdd-161">unitPrice</span></span>           |<span data-ttu-id="43fdd-162">decimal</span><span class="sxs-lookup"><span data-stu-id="43fdd-162">decimal</span></span> |<span data-ttu-id="43fdd-163">指定した通貨でのアイテムの1単位の価格を指定します。</span><span class="sxs-lookup"><span data-stu-id="43fdd-163">Specifies the price for one unit of the item in the specified currency.</span></span>|
|<span data-ttu-id="43fdd-164">priceIncludesTax</span><span class="sxs-lookup"><span data-stu-id="43fdd-164">priceIncludesTax</span></span>    |<span data-ttu-id="43fdd-165">ブール値</span><span class="sxs-lookup"><span data-stu-id="43fdd-165">boolean</span></span> |<span data-ttu-id="43fdd-166">UnitPrice に税が含まれることを指定します。</span><span class="sxs-lookup"><span data-stu-id="43fdd-166">Specifies that the unitPrice includes tax.</span></span> <span data-ttu-id="43fdd-167">UnitPrice に tax が含まれる場合は**true**に設定します。</span><span class="sxs-lookup"><span data-stu-id="43fdd-167">Set to **true**, if unitPrice includes tax.</span></span>|
|<span data-ttu-id="43fdd-168">unitCost</span><span class="sxs-lookup"><span data-stu-id="43fdd-168">unitCost</span></span>            |<span data-ttu-id="43fdd-169">decimal</span><span class="sxs-lookup"><span data-stu-id="43fdd-169">decimal</span></span> |<span data-ttu-id="43fdd-170">アイテムの単位あたりのコストを指定します。</span><span class="sxs-lookup"><span data-stu-id="43fdd-170">Specifies the cost per unit of the item.</span></span>             |
|<span data-ttu-id="43fdd-171">taxGroupId</span><span class="sxs-lookup"><span data-stu-id="43fdd-171">taxGroupId</span></span>          |<span data-ttu-id="43fdd-172">GUID</span><span class="sxs-lookup"><span data-stu-id="43fdd-172">GUID</span></span>    |<span data-ttu-id="43fdd-173">アイテムの税グループの ID を指定します。</span><span class="sxs-lookup"><span data-stu-id="43fdd-173">Specifies the ID of the Tax Group for the item.</span></span>      |
|<span data-ttu-id="43fdd-174">taxGroupCode</span><span class="sxs-lookup"><span data-stu-id="43fdd-174">taxGroupCode</span></span>        |<span data-ttu-id="43fdd-175">数値</span><span class="sxs-lookup"><span data-stu-id="43fdd-175">numeric</span></span> |<span data-ttu-id="43fdd-176">税グループは、同一の税用語の対象となる在庫品目またはリソースのグループを表します。</span><span class="sxs-lookup"><span data-stu-id="43fdd-176">A Tax Group represents a group of inventory items or resources that are subject to identical tax terms.</span></span>|
|<span data-ttu-id="43fdd-177">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="43fdd-177">lastModifiedDateTime</span></span>|<span data-ttu-id="43fdd-178">datetime</span><span class="sxs-lookup"><span data-stu-id="43fdd-178">datetime</span></span>|<span data-ttu-id="43fdd-179">アイテムが最後に変更された datetime。</span><span class="sxs-lookup"><span data-stu-id="43fdd-179">The last datetime the item was modified.</span></span> <span data-ttu-id="43fdd-180">読み取り専用。</span><span class="sxs-lookup"><span data-stu-id="43fdd-180">Read-Only.</span></span>  |  


## <a name="relationships"></a><span data-ttu-id="43fdd-181">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="43fdd-181">Relationships</span></span>
<span data-ttu-id="43fdd-182">税グループ (taxGroupCode) は、税グループテーブルに存在する必要があります。</span><span class="sxs-lookup"><span data-stu-id="43fdd-182">A Tax Group(taxGroupCode) must exist in the Tax Group table.</span></span>

## <a name="json-representation"></a><span data-ttu-id="43fdd-183">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="43fdd-183">JSON representation</span></span>

<span data-ttu-id="43fdd-184">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="43fdd-184">Here is a JSON representation of the resource.</span></span>


```json
{
      "id": "GUID",
      "number": "string",
      "displayName": "string",
      "type": "string",
      "blocked": "boolean",
      "baseUnitOfMeasureId": "GUID",
      "baseUnitOfMeasure": "NAV.UnitOfMeasure",
      "gtin": "numeric",
      "itemCategoryId": "GUID",
      "inventory": "decimal",
      "unitPrice": "decimal",
      "priceIncludesTax": "boolean",
      "unitCost": "decimal",
      "taxGroupId": "GUID",
      "taxGroupCode": "string",
      "lastModifiedDateTime": "datetime"
}

```


