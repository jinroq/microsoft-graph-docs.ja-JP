---
author: JeremyKelley
ms.author: JeremyKelley
ms.date: 09/10/2017
title: FolderView
localization_priority: Normal
ms.openlocfilehash: fa1ecc3152492ceeee61a9bc94ae1b4dfbb8ff3d
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/26/2019
ms.locfileid: "33333735"
---
# <a name="folderview-resource-type"></a><span data-ttu-id="6262b-102">FolderView リソースの種類</span><span class="sxs-lookup"><span data-stu-id="6262b-102">FolderView resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="6262b-103">**FolderView** リソースは、フォルダーのユーザー エクスペリエンスに関する推奨事項を提供または設定します。</span><span class="sxs-lookup"><span data-stu-id="6262b-103">The **FolderView** resource provides or sets recommendations on the user-experience of a folder.</span></span>

<span data-ttu-id="6262b-104">これは、[driveItem][item-resource] リソースの [folder][folder-facet] プロパティから使用できます。</span><span class="sxs-lookup"><span data-stu-id="6262b-104">It is available from the [folder][folder-facet] property of [driveItem][item-resource] resources.</span></span>

## <a name="json-representation"></a><span data-ttu-id="6262b-105">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="6262b-105">JSON representation</span></span>

<!-- { "blockType": "resource", "@odata.type": "microsoft.graph.folderView" } -->

```json
{
  "sortBy": "default | name | type | size | takenOrCreatedDateTime | lastModifiedDateTime | sequence",
  "viewType": "default | icons | details | thumbnails",
  "sortOrder": "string"
}
```

## <a name="properties"></a><span data-ttu-id="6262b-106">プロパティ</span><span class="sxs-lookup"><span data-stu-id="6262b-106">Properties</span></span>

| <span data-ttu-id="6262b-107">プロパティ名</span><span class="sxs-lookup"><span data-stu-id="6262b-107">Property name</span></span>         | <span data-ttu-id="6262b-108">種類</span><span class="sxs-lookup"><span data-stu-id="6262b-108">Type</span></span>   | <span data-ttu-id="6262b-109">説明</span><span class="sxs-lookup"><span data-stu-id="6262b-109">Description</span></span>
|:----------------------|:-------|:--------------------------------------------
| <span data-ttu-id="6262b-110">**sortBy**</span><span class="sxs-lookup"><span data-stu-id="6262b-110">**sortBy**</span></span>            | <span data-ttu-id="6262b-111">string</span><span class="sxs-lookup"><span data-stu-id="6262b-111">string</span></span> | <span data-ttu-id="6262b-112">フォルダーの並べ替え方法。</span><span class="sxs-lookup"><span data-stu-id="6262b-112">The method by which the folder should be sorted.</span></span>
| <span data-ttu-id="6262b-113">**sortOrder**</span><span class="sxs-lookup"><span data-stu-id="6262b-113">**sortOrder**</span></span>         | <span data-ttu-id="6262b-114">string</span><span class="sxs-lookup"><span data-stu-id="6262b-114">string</span></span> | <span data-ttu-id="6262b-p101">true の場合は、アイテムが降順で並べ替えられることを示します。 それ以外の場合は、アイテムが昇順で並べ替えられます。</span><span class="sxs-lookup"><span data-stu-id="6262b-p101">If true, indicates that items should be sorted in descending order. Otherwise, items should be sorted ascending.</span></span>
| <span data-ttu-id="6262b-117">**viewType**</span><span class="sxs-lookup"><span data-stu-id="6262b-117">**viewType**</span></span>          | <span data-ttu-id="6262b-118">string</span><span class="sxs-lookup"><span data-stu-id="6262b-118">string</span></span> | <span data-ttu-id="6262b-119">フォルダーを表すために使用されるビューの種類。</span><span class="sxs-lookup"><span data-stu-id="6262b-119">The type of view that should be used to represent the folder.</span></span>

<span data-ttu-id="6262b-120">_sortBy_ プロパティを使用すると、**viewType** ファセットを優先するアプリケーションで、アイテムの並べ替え順序を制御できます。</span><span class="sxs-lookup"><span data-stu-id="6262b-120">You can use the _sortBy_ property to control the sort order of the items in applications that respect the **viewType** facet.</span></span>

### <a name="sortby-values"></a><span data-ttu-id="6262b-121">sortBy の値</span><span class="sxs-lookup"><span data-stu-id="6262b-121">sortBy values</span></span>

<span data-ttu-id="6262b-122">**sortBy** プロパティに定義されている値は次のとおりです。</span><span class="sxs-lookup"><span data-stu-id="6262b-122">The following values are defined for the **sortBy** property.</span></span>

| <span data-ttu-id="6262b-123">値</span><span class="sxs-lookup"><span data-stu-id="6262b-123">Value</span></span>                    | <span data-ttu-id="6262b-124">説明</span><span class="sxs-lookup"><span data-stu-id="6262b-124">Description</span></span>
| ------------------------ | --------------------------------------------------
| `default`                | <span data-ttu-id="6262b-125">アプリケーションの既定の並べ替え順序。</span><span class="sxs-lookup"><span data-stu-id="6262b-125">The default sort order of the application.</span></span>
| `name`                   | <span data-ttu-id="6262b-126">アイテムは、アイテムの **name** プロパティで整列されます。</span><span class="sxs-lookup"><span data-stu-id="6262b-126">Items should be arranged by the **name** property of the items.</span></span>
| `type`                   | <span data-ttu-id="6262b-127">アイテムは、アイテムの種類で整列されます。</span><span class="sxs-lookup"><span data-stu-id="6262b-127">Items should be arranged by the type of item.</span></span>
| `size`                   | <span data-ttu-id="6262b-128">アイテムは、アイテムの **size** プロパティで整列されます。</span><span class="sxs-lookup"><span data-stu-id="6262b-128">Items should be arranged by the **size** property of the items.</span></span>
| `takenOrCreatedDateTime` | <span data-ttu-id="6262b-p102">アイテムは、**photo** ファセットの **takenDateTime** プロパティで整列されます。 これが使用できない場合は、**createdDateTime** プロパティが使用されます。</span><span class="sxs-lookup"><span data-stu-id="6262b-p102">Items should be arranged by the **takenDateTime** property of the **photo** facet. If not available, the **createdDateTime** property should be used.</span></span>
| `lastModifiedDateTime`   | <span data-ttu-id="6262b-131">アイテムは、アイテムの **lastModifiedDateTime** プロパティで整列されます。</span><span class="sxs-lookup"><span data-stu-id="6262b-131">Items should be arranged by the **lastModifiedDateTime** property of the items.</span></span>
| `sequence`               | <span data-ttu-id="6262b-132">アイテムは、ユーザーによって指定されたカスタム順序で並びます。</span><span class="sxs-lookup"><span data-stu-id="6262b-132">Items follow a custom sequence specified by the user.</span></span>


### <a name="sortorder-values"></a><span data-ttu-id="6262b-133">sortOrder の値</span><span class="sxs-lookup"><span data-stu-id="6262b-133">sortOrder values</span></span>

<span data-ttu-id="6262b-134">**sortOrder** プロパティに定義されている値は次のとおりです。</span><span class="sxs-lookup"><span data-stu-id="6262b-134">The following values are defined for the **sortOrder** property.</span></span>

| <span data-ttu-id="6262b-135">値</span><span class="sxs-lookup"><span data-stu-id="6262b-135">Value</span></span>        | <span data-ttu-id="6262b-136">説明</span><span class="sxs-lookup"><span data-stu-id="6262b-136">Description</span></span>
| ------------ | --------------------------------------------------------------
| `ascending`  | <span data-ttu-id="6262b-137">アイテムは、昇順で整列されます。</span><span class="sxs-lookup"><span data-stu-id="6262b-137">Items should be arranged in ascending order.</span></span>
| `descending` | <span data-ttu-id="6262b-138">アイテムは、降順で整列されます。</span><span class="sxs-lookup"><span data-stu-id="6262b-138">Items should be arranged in descending order.</span></span>


### <a name="viewtype-values"></a><span data-ttu-id="6262b-139">viewType の値</span><span class="sxs-lookup"><span data-stu-id="6262b-139">viewType values</span></span>

<span data-ttu-id="6262b-140">**viewType** プロパティに定義されている値は次のとおりです。</span><span class="sxs-lookup"><span data-stu-id="6262b-140">The following values are defined for the **viewType** property.</span></span>

| <span data-ttu-id="6262b-141">値</span><span class="sxs-lookup"><span data-stu-id="6262b-141">Value</span></span>        | <span data-ttu-id="6262b-142">説明</span><span class="sxs-lookup"><span data-stu-id="6262b-142">Description</span></span>
| ------------ | --------------------------------------------------------------
| `default`    | <span data-ttu-id="6262b-143">アプリケーションの既定のビューの種類。</span><span class="sxs-lookup"><span data-stu-id="6262b-143">The default view type for the application.</span></span>
| `icons`      | <span data-ttu-id="6262b-144">driveItem を表すためにアイコンを使用するビュー。</span><span class="sxs-lookup"><span data-stu-id="6262b-144">A view that uses icons to represent driveItems.</span></span>
| `details`    | <span data-ttu-id="6262b-145">各アイテムに関する追加の詳細を提示する、複数の列を持つビュー。</span><span class="sxs-lookup"><span data-stu-id="6262b-145">A view with multiple columns that provide additional details about each item.</span></span>
| `thumbnails` | <span data-ttu-id="6262b-146">アイテムを表すために driveItem の大きなサムネイルを使用するビュー。</span><span class="sxs-lookup"><span data-stu-id="6262b-146">A view that uses larger thumbnails of driveItems to represent the items.</span></span>


[item-resource]: driveitem.md
[folder-facet]: folder.md

<!-- uuid: f9e446fd-190b-4692-a605-bb60e78f1f19
2017-05-03 02:34:40 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "folderView resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
