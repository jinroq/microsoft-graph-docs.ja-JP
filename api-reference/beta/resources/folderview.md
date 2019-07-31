---
author: JeremyKelley
description: FolderView リソースは、フォルダーのユーザー エクスペリエンスに関する推奨事項を提供または設定します。
ms.date: 09/10/2017
title: FolderView
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
ms.openlocfilehash: 5238c749d509339cd0e922e49b7e2d4d2da3b23f
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "35973549"
---
# <a name="folderview-resource-type"></a><span data-ttu-id="742f0-103">FolderView リソースの種類</span><span class="sxs-lookup"><span data-stu-id="742f0-103">FolderView resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="742f0-104">**FolderView** リソースは、フォルダーのユーザー エクスペリエンスに関する推奨事項を提供または設定します。</span><span class="sxs-lookup"><span data-stu-id="742f0-104">The **FolderView** resource provides or sets recommendations on the user-experience of a folder.</span></span>

<span data-ttu-id="742f0-105">このプロパティは、 [Drive item][item-resource]リソースの[folder][folder-facet]プロパティから使用できます。</span><span class="sxs-lookup"><span data-stu-id="742f0-105">It is available from the [folder][folder-facet] property of [driveItem][item-resource] resources.</span></span>

## <a name="json-representation"></a><span data-ttu-id="742f0-106">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="742f0-106">JSON representation</span></span>

<!-- { "blockType": "resource", "@odata.type": "microsoft.graph.folderView" } -->

```json
{
  "sortBy": "default | name | type | size | takenOrCreatedDateTime | lastModifiedDateTime | sequence",
  "viewType": "default | icons | details | thumbnails",
  "sortOrder": "string"
}
```

## <a name="properties"></a><span data-ttu-id="742f0-107">プロパティ</span><span class="sxs-lookup"><span data-stu-id="742f0-107">Properties</span></span>

| <span data-ttu-id="742f0-108">プロパティ名</span><span class="sxs-lookup"><span data-stu-id="742f0-108">Property name</span></span>         | <span data-ttu-id="742f0-109">種類</span><span class="sxs-lookup"><span data-stu-id="742f0-109">Type</span></span>   | <span data-ttu-id="742f0-110">説明</span><span class="sxs-lookup"><span data-stu-id="742f0-110">Description</span></span>
|:----------------------|:-------|:--------------------------------------------
| <span data-ttu-id="742f0-111">**sortBy**</span><span class="sxs-lookup"><span data-stu-id="742f0-111">**sortBy**</span></span>            | <span data-ttu-id="742f0-112">string</span><span class="sxs-lookup"><span data-stu-id="742f0-112">string</span></span> | <span data-ttu-id="742f0-113">フォルダーの並べ替え方法。</span><span class="sxs-lookup"><span data-stu-id="742f0-113">The method by which the folder should be sorted.</span></span>
| <span data-ttu-id="742f0-114">**sortOrder**</span><span class="sxs-lookup"><span data-stu-id="742f0-114">**sortOrder**</span></span>         | <span data-ttu-id="742f0-115">string</span><span class="sxs-lookup"><span data-stu-id="742f0-115">string</span></span> | <span data-ttu-id="742f0-p101">true の場合は、アイテムが降順で並べ替えられることを示します。 それ以外の場合は、アイテムが昇順で並べ替えられます。</span><span class="sxs-lookup"><span data-stu-id="742f0-p101">If true, indicates that items should be sorted in descending order. Otherwise, items should be sorted ascending.</span></span>
| <span data-ttu-id="742f0-118">**viewType**</span><span class="sxs-lookup"><span data-stu-id="742f0-118">**viewType**</span></span>          | <span data-ttu-id="742f0-119">string</span><span class="sxs-lookup"><span data-stu-id="742f0-119">string</span></span> | <span data-ttu-id="742f0-120">フォルダーを表すために使用されるビューの種類。</span><span class="sxs-lookup"><span data-stu-id="742f0-120">The type of view that should be used to represent the folder.</span></span>

<span data-ttu-id="742f0-121">_sortBy_ プロパティを使用すると、**viewType** ファセットを優先するアプリケーションで、アイテムの並べ替え順序を制御できます。</span><span class="sxs-lookup"><span data-stu-id="742f0-121">You can use the _sortBy_ property to control the sort order of the items in applications that respect the **viewType** facet.</span></span>

### <a name="sortby-values"></a><span data-ttu-id="742f0-122">sortBy の値</span><span class="sxs-lookup"><span data-stu-id="742f0-122">sortBy values</span></span>

<span data-ttu-id="742f0-123">**sortBy** プロパティに定義されている値は次のとおりです。</span><span class="sxs-lookup"><span data-stu-id="742f0-123">The following values are defined for the **sortBy** property.</span></span>

| <span data-ttu-id="742f0-124">値</span><span class="sxs-lookup"><span data-stu-id="742f0-124">Value</span></span>                    | <span data-ttu-id="742f0-125">説明</span><span class="sxs-lookup"><span data-stu-id="742f0-125">Description</span></span>
| ------------------------ | --------------------------------------------------
| `default`                | <span data-ttu-id="742f0-126">アプリケーションの既定の並べ替え順序。</span><span class="sxs-lookup"><span data-stu-id="742f0-126">The default sort order of the application.</span></span>
| `name`                   | <span data-ttu-id="742f0-127">アイテムは、アイテムの **name** プロパティで整列されます。</span><span class="sxs-lookup"><span data-stu-id="742f0-127">Items should be arranged by the **name** property of the items.</span></span>
| `type`                   | <span data-ttu-id="742f0-128">アイテムは、アイテムの種類で整列されます。</span><span class="sxs-lookup"><span data-stu-id="742f0-128">Items should be arranged by the type of item.</span></span>
| `size`                   | <span data-ttu-id="742f0-129">アイテムは、アイテムの **size** プロパティで整列されます。</span><span class="sxs-lookup"><span data-stu-id="742f0-129">Items should be arranged by the **size** property of the items.</span></span>
| `takenOrCreatedDateTime` | <span data-ttu-id="742f0-p102">アイテムは、**photo** ファセットの **takenDateTime** プロパティで整列されます。 これが使用できない場合は、**createdDateTime** プロパティが使用されます。</span><span class="sxs-lookup"><span data-stu-id="742f0-p102">Items should be arranged by the **takenDateTime** property of the **photo** facet. If not available, the **createdDateTime** property should be used.</span></span>
| `lastModifiedDateTime`   | <span data-ttu-id="742f0-132">アイテムは、アイテムの **lastModifiedDateTime** プロパティで整列されます。</span><span class="sxs-lookup"><span data-stu-id="742f0-132">Items should be arranged by the **lastModifiedDateTime** property of the items.</span></span>
| `sequence`               | <span data-ttu-id="742f0-133">アイテムは、ユーザーによって指定されたカスタム順序で並びます。</span><span class="sxs-lookup"><span data-stu-id="742f0-133">Items follow a custom sequence specified by the user.</span></span>


### <a name="sortorder-values"></a><span data-ttu-id="742f0-134">sortOrder の値</span><span class="sxs-lookup"><span data-stu-id="742f0-134">sortOrder values</span></span>

<span data-ttu-id="742f0-135">**sortOrder** プロパティに定義されている値は次のとおりです。</span><span class="sxs-lookup"><span data-stu-id="742f0-135">The following values are defined for the **sortOrder** property.</span></span>

| <span data-ttu-id="742f0-136">値</span><span class="sxs-lookup"><span data-stu-id="742f0-136">Value</span></span>        | <span data-ttu-id="742f0-137">説明</span><span class="sxs-lookup"><span data-stu-id="742f0-137">Description</span></span>
| ------------ | --------------------------------------------------------------
| `ascending`  | <span data-ttu-id="742f0-138">アイテムは、昇順で整列されます。</span><span class="sxs-lookup"><span data-stu-id="742f0-138">Items should be arranged in ascending order.</span></span>
| `descending` | <span data-ttu-id="742f0-139">アイテムは、降順で整列されます。</span><span class="sxs-lookup"><span data-stu-id="742f0-139">Items should be arranged in descending order.</span></span>


### <a name="viewtype-values"></a><span data-ttu-id="742f0-140">viewType の値</span><span class="sxs-lookup"><span data-stu-id="742f0-140">viewType values</span></span>

<span data-ttu-id="742f0-141">**viewType** プロパティに定義されている値は次のとおりです。</span><span class="sxs-lookup"><span data-stu-id="742f0-141">The following values are defined for the **viewType** property.</span></span>

| <span data-ttu-id="742f0-142">値</span><span class="sxs-lookup"><span data-stu-id="742f0-142">Value</span></span>        | <span data-ttu-id="742f0-143">説明</span><span class="sxs-lookup"><span data-stu-id="742f0-143">Description</span></span>
| ------------ | --------------------------------------------------------------
| `default`    | <span data-ttu-id="742f0-144">アプリケーションの既定のビューの種類。</span><span class="sxs-lookup"><span data-stu-id="742f0-144">The default view type for the application.</span></span>
| `icons`      | <span data-ttu-id="742f0-145">driveItem を表すためにアイコンを使用するビュー。</span><span class="sxs-lookup"><span data-stu-id="742f0-145">A view that uses icons to represent driveItems.</span></span>
| `details`    | <span data-ttu-id="742f0-146">各アイテムに関する追加の詳細を提示する、複数の列を持つビュー。</span><span class="sxs-lookup"><span data-stu-id="742f0-146">A view with multiple columns that provide additional details about each item.</span></span>
| `thumbnails` | <span data-ttu-id="742f0-147">アイテムを表すために driveItem の大きなサムネイルを使用するビュー。</span><span class="sxs-lookup"><span data-stu-id="742f0-147">A view that uses larger thumbnails of driveItems to represent the items.</span></span>


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
