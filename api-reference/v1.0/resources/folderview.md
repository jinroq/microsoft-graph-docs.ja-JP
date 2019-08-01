---
author: JeremyKelley
ms.author: JeremyKelley
ms.date: 09/10/2017
title: FolderView
localization_priority: Normal
description: FolderView リソースは、フォルダーのユーザー エクスペリエンスに関する推奨事項を提供または設定します。
ms.prod: ''
doc_type: resourcePageType
ms.openlocfilehash: 67ec2e079348cc45664804d39314e6c81f4548e3
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "36032453"
---
# <a name="folderview-resource-type"></a><span data-ttu-id="9a590-103">FolderView リソースの種類</span><span class="sxs-lookup"><span data-stu-id="9a590-103">FolderView resource type</span></span>

<span data-ttu-id="9a590-104">**FolderView** リソースは、フォルダーのユーザー エクスペリエンスに関する推奨事項を提供または設定します。</span><span class="sxs-lookup"><span data-stu-id="9a590-104">The **FolderView** resource provides or sets recommendations on the user-experience of a folder.</span></span>

<span data-ttu-id="9a590-105">このプロパティは、 [Drive item][item-resource]リソースの[folder][folder-facet]プロパティから使用できます。</span><span class="sxs-lookup"><span data-stu-id="9a590-105">It is available from the [folder][folder-facet] property of [driveItem][item-resource] resources.</span></span>

## <a name="json-representation"></a><span data-ttu-id="9a590-106">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="9a590-106">JSON representation</span></span>

<!-- { "blockType": "resource", "@odata.type": "microsoft.graph.folderView" } -->

```json
{
  "sortBy": "default | name | type | size | takenOrCreatedDateTime | lastModifiedDateTime | sequence",
  "sortOrder": "ascending | descending",
  "viewType": "default | icons | details | thumbnails"
}
```

## <a name="properties"></a><span data-ttu-id="9a590-107">プロパティ</span><span class="sxs-lookup"><span data-stu-id="9a590-107">Properties</span></span>

| <span data-ttu-id="9a590-108">プロパティ名</span><span class="sxs-lookup"><span data-stu-id="9a590-108">Property name</span></span>         | <span data-ttu-id="9a590-109">種類</span><span class="sxs-lookup"><span data-stu-id="9a590-109">Type</span></span>   | <span data-ttu-id="9a590-110">説明</span><span class="sxs-lookup"><span data-stu-id="9a590-110">Description</span></span>
|:----------------------|:-------|:--------------------------------------------
| <span data-ttu-id="9a590-111">**sortBy**</span><span class="sxs-lookup"><span data-stu-id="9a590-111">**sortBy**</span></span>            | <span data-ttu-id="9a590-112">string</span><span class="sxs-lookup"><span data-stu-id="9a590-112">string</span></span> | <span data-ttu-id="9a590-113">フォルダーの並べ替え方法。</span><span class="sxs-lookup"><span data-stu-id="9a590-113">The method by which the folder should be sorted.</span></span>
| <span data-ttu-id="9a590-114">**sortOrder**</span><span class="sxs-lookup"><span data-stu-id="9a590-114">**sortOrder**</span></span>         | <span data-ttu-id="9a590-115">string</span><span class="sxs-lookup"><span data-stu-id="9a590-115">string</span></span> | <span data-ttu-id="9a590-p101">true の場合は、アイテムが降順で並べ替えられることを示します。 それ以外の場合は、アイテムが昇順で並べ替えられます。</span><span class="sxs-lookup"><span data-stu-id="9a590-p101">If true, indicates that items should be sorted in descending order. Otherwise, items should be sorted ascending.</span></span>
| <span data-ttu-id="9a590-118">**viewType**</span><span class="sxs-lookup"><span data-stu-id="9a590-118">**viewType**</span></span>          | <span data-ttu-id="9a590-119">string</span><span class="sxs-lookup"><span data-stu-id="9a590-119">string</span></span> | <span data-ttu-id="9a590-120">フォルダーを表すために使用されるビューの種類。</span><span class="sxs-lookup"><span data-stu-id="9a590-120">The type of view that should be used to represent the folder.</span></span>

<span data-ttu-id="9a590-121">_sortBy_ プロパティを使用すると、**viewType** ファセットを優先するアプリケーションで、アイテムの並べ替え順序を制御できます。</span><span class="sxs-lookup"><span data-stu-id="9a590-121">You can use the _sortBy_ property to control the sort order of the items in applications that respect the **viewType** facet.</span></span>

### <a name="sortby-options"></a><span data-ttu-id="9a590-122">sortBy オプション</span><span class="sxs-lookup"><span data-stu-id="9a590-122">sortBy options</span></span>

<span data-ttu-id="9a590-123">**sortBy** プロパティに定義されている値は次のとおりです。</span><span class="sxs-lookup"><span data-stu-id="9a590-123">The following values are defined for the **sortBy** property.</span></span>

| <span data-ttu-id="9a590-124">値</span><span class="sxs-lookup"><span data-stu-id="9a590-124">Value</span></span>                    | <span data-ttu-id="9a590-125">説明</span><span class="sxs-lookup"><span data-stu-id="9a590-125">Description</span></span>
| ------------------------ | --------------------------------------------------
| `default`                | <span data-ttu-id="9a590-126">アプリケーションの既定の並べ替え順序。</span><span class="sxs-lookup"><span data-stu-id="9a590-126">The default sort order of the application.</span></span>
| `name`                   | <span data-ttu-id="9a590-127">アイテムは、アイテムの **name** プロパティで整列されます。</span><span class="sxs-lookup"><span data-stu-id="9a590-127">Items should be arranged by the **name** property of the items.</span></span>
| `type`                   | <span data-ttu-id="9a590-128">アイテムは、アイテムの種類で整列されます。</span><span class="sxs-lookup"><span data-stu-id="9a590-128">Items should be arranged by the type of item.</span></span>
| `size`                   | <span data-ttu-id="9a590-129">アイテムは、アイテムの **size** プロパティで整列されます。</span><span class="sxs-lookup"><span data-stu-id="9a590-129">Items should be arranged by the **size** property of the items.</span></span>
| `takenOrCreatedDateTime` | <span data-ttu-id="9a590-p102">アイテムは、**photo** ファセットの **takenDateTime** プロパティで整列されます。 これが使用できない場合は、**createdDateTime** プロパティが使用されます。</span><span class="sxs-lookup"><span data-stu-id="9a590-p102">Items should be arranged by the **takenDateTime** property of the **photo** facet. If not available, the **createdDateTime** property should be used.</span></span>
| `lastModifiedDateTime`   | <span data-ttu-id="9a590-132">アイテムは、アイテムの **lastModifiedDateTime** プロパティで整列されます。</span><span class="sxs-lookup"><span data-stu-id="9a590-132">Items should be arranged by the **lastModifiedDateTime** property of the items.</span></span>
| `sequence`               | <span data-ttu-id="9a590-133">アイテムは、ユーザーによって指定されたカスタム順序で並びます。</span><span class="sxs-lookup"><span data-stu-id="9a590-133">Items follow a custom sequence specified by the user.</span></span>


### <a name="sortorder-options"></a><span data-ttu-id="9a590-134">ソート順序オプション</span><span class="sxs-lookup"><span data-stu-id="9a590-134">sortOrder options</span></span>

<span data-ttu-id="9a590-135">**sortOrder** プロパティに定義されている値は次のとおりです。</span><span class="sxs-lookup"><span data-stu-id="9a590-135">The following values are defined for the **sortOrder** property.</span></span>

| <span data-ttu-id="9a590-136">値</span><span class="sxs-lookup"><span data-stu-id="9a590-136">Value</span></span>        | <span data-ttu-id="9a590-137">説明</span><span class="sxs-lookup"><span data-stu-id="9a590-137">Description</span></span>
| ------------ | --------------------------------------------------------------
| `ascending`  | <span data-ttu-id="9a590-138">アイテムは、昇順で整列されます。</span><span class="sxs-lookup"><span data-stu-id="9a590-138">Items should be arranged in ascending order.</span></span>
| `descending` | <span data-ttu-id="9a590-139">アイテムは、降順で整列されます。</span><span class="sxs-lookup"><span data-stu-id="9a590-139">Items should be arranged in descending order.</span></span>


### <a name="viewtype-options"></a><span data-ttu-id="9a590-140">viewType オプション</span><span class="sxs-lookup"><span data-stu-id="9a590-140">viewType options</span></span>

<span data-ttu-id="9a590-141">**viewType** プロパティに定義されている値は次のとおりです。</span><span class="sxs-lookup"><span data-stu-id="9a590-141">The following values are defined for the **viewType** property.</span></span>

| <span data-ttu-id="9a590-142">値</span><span class="sxs-lookup"><span data-stu-id="9a590-142">Value</span></span>        | <span data-ttu-id="9a590-143">説明</span><span class="sxs-lookup"><span data-stu-id="9a590-143">Description</span></span>
| ------------ | --------------------------------------------------------------
| `default`    | <span data-ttu-id="9a590-144">アプリケーションの既定のビューの種類。</span><span class="sxs-lookup"><span data-stu-id="9a590-144">The default view type for the application.</span></span>
| `icons`      | <span data-ttu-id="9a590-145">driveItem を表すためにアイコンを使用するビュー。</span><span class="sxs-lookup"><span data-stu-id="9a590-145">A view that uses icons to represent driveItems.</span></span>
| `details`    | <span data-ttu-id="9a590-146">各アイテムに関する追加の詳細を提示する、複数の列を持つビュー。</span><span class="sxs-lookup"><span data-stu-id="9a590-146">A view with multiple columns that provide additional details about each item.</span></span>
| `thumbnails` | <span data-ttu-id="9a590-147">アイテムを表すために driveItem の大きなサムネイルを使用するビュー。</span><span class="sxs-lookup"><span data-stu-id="9a590-147">A view that uses larger thumbnails of driveItems to represent the items.</span></span>


[item-resource]: driveitem.md
[folder-facet]: folder.md

<!-- {
  "type": "#page.annotation",
  "description": "The FolderView facet provides or sets recommendations on the user-experience of a folder.",
  "keywords": "view, folderview, sortby, sortorder, viewtype, coversourceid, folder",
  "section": "documentation",
  "suppressions": [
    "Warning: /api-reference/v1.0/resources/folderview.md:
      Found potential enums in resource example that weren't defined in a table:(default,icons,details,thumbnails) are in resource, but () are in table",
    "Warning: /api-reference/v1.0/resources/folderview.md:
      Found potential enums in resource example that weren't defined in a table:(default,name,type,size,takenOrCreatedDateTime,lastModifiedDateTime,sequence) are in resource, but () are in table",
    "Warning: /api-reference/v1.0/resources/folderview.md:
      Found potential enums in resource example that weren't defined in a table:(ascending,descending) are in resource, but () are in table"
  ],
  "tocPath": "Facets/FolderView"
} -->
