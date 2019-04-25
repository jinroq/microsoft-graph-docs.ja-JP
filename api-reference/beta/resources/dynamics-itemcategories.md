---
title: itemcategories リソースの種類
description: Dynamics 365 Business Central のアイテムカテゴリ。
services: project-madeira
documentationcenter: ''
author: SusanneWindfeldPedersen
localization_priority: Normal
ms.prod: dynamics-365-business-central
ms.openlocfilehash: e18319683f6dbceddccc9cf83e48cd3ef89f895d
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32543057"
---
# <a name="itemcategories-resource-type"></a><span data-ttu-id="86be1-103">itemcategories リソースの種類</span><span class="sxs-lookup"><span data-stu-id="86be1-103">itemCategories resource type</span></span>
<span data-ttu-id="86be1-104">Dynamics 365 Business Central の複数のアイテムのカテゴリを表します。</span><span class="sxs-lookup"><span data-stu-id="86be1-104">Represents a category for a number of items in Dynamics 365 Business Central.</span></span>

## <a name="methods"></a><span data-ttu-id="86be1-105">メソッド</span><span class="sxs-lookup"><span data-stu-id="86be1-105">Methods</span></span>

| <span data-ttu-id="86be1-106">メソッド</span><span class="sxs-lookup"><span data-stu-id="86be1-106">Method</span></span>                                                          | <span data-ttu-id="86be1-107">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="86be1-107">Return Type</span></span>  |<span data-ttu-id="86be1-108">説明</span><span class="sxs-lookup"><span data-stu-id="86be1-108">Description</span></span>             |
|:----------------------------------------------------------------|:-------------|:-----------------------|
|[<span data-ttu-id="86be1-109">itemcategories を取得する</span><span class="sxs-lookup"><span data-stu-id="86be1-109">Get itemCategories</span></span>](../api/dynamics-itemcategories-get.md)      |<span data-ttu-id="86be1-110">itemcategories</span><span class="sxs-lookup"><span data-stu-id="86be1-110">itemCategories</span></span>|<span data-ttu-id="86be1-111">アイテムカテゴリを取得します。</span><span class="sxs-lookup"><span data-stu-id="86be1-111">Get an item category.</span></span>   |
|[<span data-ttu-id="86be1-112">アイテムカテゴリを投稿する</span><span class="sxs-lookup"><span data-stu-id="86be1-112">Post itemCategories</span></span>](../api/dynamics-create-itemcategories.md)  |<span data-ttu-id="86be1-113">itemcategories</span><span class="sxs-lookup"><span data-stu-id="86be1-113">itemCategories</span></span>|<span data-ttu-id="86be1-114">アイテムカテゴリを作成します。</span><span class="sxs-lookup"><span data-stu-id="86be1-114">Create an item category.</span></span>|
|[<span data-ttu-id="86be1-115">Patch itemcategories</span><span class="sxs-lookup"><span data-stu-id="86be1-115">Patch itemCategories</span></span>](../api/dynamics-itemcategories-update.md) |<span data-ttu-id="86be1-116">itemcategories</span><span class="sxs-lookup"><span data-stu-id="86be1-116">itemCategories</span></span>|<span data-ttu-id="86be1-117">アイテムカテゴリを更新します。</span><span class="sxs-lookup"><span data-stu-id="86be1-117">Update an item category.</span></span>|
|[<span data-ttu-id="86be1-118">itemcategories の削除</span><span class="sxs-lookup"><span data-stu-id="86be1-118">Delete itemCategories</span></span>](../api/dynamics-itemcategories-delete.md)|<span data-ttu-id="86be1-119">なし</span><span class="sxs-lookup"><span data-stu-id="86be1-119">none</span></span>          |<span data-ttu-id="86be1-120">アイテムカテゴリを削除します。</span><span class="sxs-lookup"><span data-stu-id="86be1-120">Delete an item category.</span></span>|

## <a name="properties"></a><span data-ttu-id="86be1-121">プロパティ</span><span class="sxs-lookup"><span data-stu-id="86be1-121">Properties</span></span>
| <span data-ttu-id="86be1-122">プロパティ</span><span class="sxs-lookup"><span data-stu-id="86be1-122">Property</span></span>           | <span data-ttu-id="86be1-123">型</span><span class="sxs-lookup"><span data-stu-id="86be1-123">Type</span></span>   |<span data-ttu-id="86be1-124">説明</span><span class="sxs-lookup"><span data-stu-id="86be1-124">Description</span></span>                                     |
|:-------------------|:-------|:-----------------------------------------------|
|<span data-ttu-id="86be1-125">id</span><span class="sxs-lookup"><span data-stu-id="86be1-125">id</span></span>                  |<span data-ttu-id="86be1-126">GUID</span><span class="sxs-lookup"><span data-stu-id="86be1-126">GUID</span></span>    |<span data-ttu-id="86be1-127">itemcategory の一意の ID。</span><span class="sxs-lookup"><span data-stu-id="86be1-127">The unique ID of the itemCategory.</span></span> <span data-ttu-id="86be1-128">編集できません。</span><span class="sxs-lookup"><span data-stu-id="86be1-128">Non-editable.</span></span>|
|<span data-ttu-id="86be1-129">code</span><span class="sxs-lookup"><span data-stu-id="86be1-129">code</span></span>                |<span data-ttu-id="86be1-130">string</span><span class="sxs-lookup"><span data-stu-id="86be1-130">string</span></span>  |<span data-ttu-id="86be1-131">itemcategory コード。</span><span class="sxs-lookup"><span data-stu-id="86be1-131">The itemCategory code.</span></span>                          |
|<span data-ttu-id="86be1-132">displayName</span><span class="sxs-lookup"><span data-stu-id="86be1-132">displayName</span></span>         |<span data-ttu-id="86be1-133">string</span><span class="sxs-lookup"><span data-stu-id="86be1-133">string</span></span>  |<span data-ttu-id="86be1-134">itemcategories の表示名。</span><span class="sxs-lookup"><span data-stu-id="86be1-134">The itemCategories display name.</span></span>                |
|<span data-ttu-id="86be1-135">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="86be1-135">lastModifiedDateTime</span></span>|<span data-ttu-id="86be1-136">datetime</span><span class="sxs-lookup"><span data-stu-id="86be1-136">datetime</span></span>|<span data-ttu-id="86be1-137">itemcategory が変更された最後の datetime。</span><span class="sxs-lookup"><span data-stu-id="86be1-137">The last datetime the itemCategory was modified.</span></span> <span data-ttu-id="86be1-138">読み取り専用。</span><span class="sxs-lookup"><span data-stu-id="86be1-138">Read-Only.</span></span>|  


## <a name="relationships"></a><span data-ttu-id="86be1-139">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="86be1-139">Relationships</span></span>
<span data-ttu-id="86be1-140">なし</span><span class="sxs-lookup"><span data-stu-id="86be1-140">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="86be1-141">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="86be1-141">JSON representation</span></span>

<span data-ttu-id="86be1-142">ここでは、itemcategories の JSON 表記を示します。</span><span class="sxs-lookup"><span data-stu-id="86be1-142">Here is a JSON representation of the itemCategories.</span></span>

```json
{
  "id": "GUID",
  "code": "string",
  "displayName": "string",
  "lastModifiedDateTime": "datetime"
}
```

