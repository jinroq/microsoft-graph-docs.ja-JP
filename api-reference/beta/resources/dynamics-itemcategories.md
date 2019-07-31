---
title: itemCategories リソースの種類
description: Dynamics 365 Business Central のアイテムカテゴリ。
services: project-madeira
documentationcenter: ''
author: SusanneWindfeldPedersen
localization_priority: Normal
ms.prod: dynamics-365-business-central
doc_type: resourcePageType
ms.openlocfilehash: 18017c580637bb53a70b5f7a331ff7be1dc7a07c
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "35972923"
---
# <a name="itemcategories-resource-type"></a><span data-ttu-id="1009d-103">itemCategories リソースの種類</span><span class="sxs-lookup"><span data-stu-id="1009d-103">itemCategories resource type</span></span>
<span data-ttu-id="1009d-104">Dynamics 365 Business Central の複数のアイテムのカテゴリを表します。</span><span class="sxs-lookup"><span data-stu-id="1009d-104">Represents a category for a number of items in Dynamics 365 Business Central.</span></span>

## <a name="methods"></a><span data-ttu-id="1009d-105">メソッド</span><span class="sxs-lookup"><span data-stu-id="1009d-105">Methods</span></span>

| <span data-ttu-id="1009d-106">メソッド</span><span class="sxs-lookup"><span data-stu-id="1009d-106">Method</span></span>                                                          | <span data-ttu-id="1009d-107">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="1009d-107">Return Type</span></span>  |<span data-ttu-id="1009d-108">説明</span><span class="sxs-lookup"><span data-stu-id="1009d-108">Description</span></span>             |
|:----------------------------------------------------------------|:-------------|:-----------------------|
|[<span data-ttu-id="1009d-109">ItemCategories を取得する</span><span class="sxs-lookup"><span data-stu-id="1009d-109">Get itemCategories</span></span>](../api/dynamics-itemcategories-get.md)      |<span data-ttu-id="1009d-110">itemCategories</span><span class="sxs-lookup"><span data-stu-id="1009d-110">itemCategories</span></span>|<span data-ttu-id="1009d-111">アイテムカテゴリを取得します。</span><span class="sxs-lookup"><span data-stu-id="1009d-111">Get an item category.</span></span>   |
|[<span data-ttu-id="1009d-112">アイテムカテゴリを投稿する</span><span class="sxs-lookup"><span data-stu-id="1009d-112">Post itemCategories</span></span>](../api/dynamics-create-itemcategories.md)  |<span data-ttu-id="1009d-113">itemCategories</span><span class="sxs-lookup"><span data-stu-id="1009d-113">itemCategories</span></span>|<span data-ttu-id="1009d-114">アイテムカテゴリを作成します。</span><span class="sxs-lookup"><span data-stu-id="1009d-114">Create an item category.</span></span>|
|[<span data-ttu-id="1009d-115">Patch itemCategories</span><span class="sxs-lookup"><span data-stu-id="1009d-115">Patch itemCategories</span></span>](../api/dynamics-itemcategories-update.md) |<span data-ttu-id="1009d-116">itemCategories</span><span class="sxs-lookup"><span data-stu-id="1009d-116">itemCategories</span></span>|<span data-ttu-id="1009d-117">アイテムカテゴリを更新します。</span><span class="sxs-lookup"><span data-stu-id="1009d-117">Update an item category.</span></span>|
|[<span data-ttu-id="1009d-118">ItemCategories の削除</span><span class="sxs-lookup"><span data-stu-id="1009d-118">Delete itemCategories</span></span>](../api/dynamics-itemcategories-delete.md)|<span data-ttu-id="1009d-119">none</span><span class="sxs-lookup"><span data-stu-id="1009d-119">none</span></span>          |<span data-ttu-id="1009d-120">アイテムカテゴリを削除します。</span><span class="sxs-lookup"><span data-stu-id="1009d-120">Delete an item category.</span></span>|

## <a name="properties"></a><span data-ttu-id="1009d-121">プロパティ</span><span class="sxs-lookup"><span data-stu-id="1009d-121">Properties</span></span>
| <span data-ttu-id="1009d-122">プロパティ</span><span class="sxs-lookup"><span data-stu-id="1009d-122">Property</span></span>           | <span data-ttu-id="1009d-123">型</span><span class="sxs-lookup"><span data-stu-id="1009d-123">Type</span></span>   |<span data-ttu-id="1009d-124">説明</span><span class="sxs-lookup"><span data-stu-id="1009d-124">Description</span></span>                                     |
|:-------------------|:-------|:-----------------------------------------------|
|<span data-ttu-id="1009d-125">id</span><span class="sxs-lookup"><span data-stu-id="1009d-125">id</span></span>                  |<span data-ttu-id="1009d-126">GUID</span><span class="sxs-lookup"><span data-stu-id="1009d-126">GUID</span></span>    |<span data-ttu-id="1009d-127">ItemCategory の一意の ID。</span><span class="sxs-lookup"><span data-stu-id="1009d-127">The unique ID of the itemCategory.</span></span> <span data-ttu-id="1009d-128">編集できません。</span><span class="sxs-lookup"><span data-stu-id="1009d-128">Non-editable.</span></span>|
|<span data-ttu-id="1009d-129">code</span><span class="sxs-lookup"><span data-stu-id="1009d-129">code</span></span>                |<span data-ttu-id="1009d-130">string</span><span class="sxs-lookup"><span data-stu-id="1009d-130">string</span></span>  |<span data-ttu-id="1009d-131">ItemCategory コード。</span><span class="sxs-lookup"><span data-stu-id="1009d-131">The itemCategory code.</span></span>                          |
|<span data-ttu-id="1009d-132">displayName</span><span class="sxs-lookup"><span data-stu-id="1009d-132">displayName</span></span>         |<span data-ttu-id="1009d-133">string</span><span class="sxs-lookup"><span data-stu-id="1009d-133">string</span></span>  |<span data-ttu-id="1009d-134">ItemCategories の表示名。</span><span class="sxs-lookup"><span data-stu-id="1009d-134">The itemCategories display name.</span></span>                |
|<span data-ttu-id="1009d-135">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="1009d-135">lastModifiedDateTime</span></span>|<span data-ttu-id="1009d-136">datetime</span><span class="sxs-lookup"><span data-stu-id="1009d-136">datetime</span></span>|<span data-ttu-id="1009d-137">ItemCategory が変更された最後の datetime。</span><span class="sxs-lookup"><span data-stu-id="1009d-137">The last datetime the itemCategory was modified.</span></span> <span data-ttu-id="1009d-138">読み取り専用。</span><span class="sxs-lookup"><span data-stu-id="1009d-138">Read-Only.</span></span>|  


## <a name="relationships"></a><span data-ttu-id="1009d-139">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="1009d-139">Relationships</span></span>
<span data-ttu-id="1009d-140">なし</span><span class="sxs-lookup"><span data-stu-id="1009d-140">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="1009d-141">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="1009d-141">JSON representation</span></span>

<span data-ttu-id="1009d-142">ここでは、itemCategories の JSON 表記を示します。</span><span class="sxs-lookup"><span data-stu-id="1009d-142">Here is a JSON representation of the itemCategories.</span></span>

```json
{
  "id": "GUID",
  "code": "string",
  "displayName": "string",
  "lastModifiedDateTime": "datetime"
}
```

