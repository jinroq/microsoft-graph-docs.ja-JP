---
author: rgregg
ms.author: rgregg
ms.date: 09/10/2017
title: FolderView
localization_priority: Normal
ms.openlocfilehash: 717dd93d82f109926cabf0168e4e176d7c68cd35
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/11/2019
ms.locfileid: "27861538"
---
# <a name="folderview-resource-type"></a><span data-ttu-id="79aa9-102">FolderView リソースの種類</span><span class="sxs-lookup"><span data-stu-id="79aa9-102">FolderView resource type</span></span>

> <span data-ttu-id="79aa9-103">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="79aa9-103">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="79aa9-104">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="79aa9-104">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="79aa9-105">**FolderView** リソースは、フォルダーのユーザー エクスペリエンスに関する推奨事項を提供または設定します。</span><span class="sxs-lookup"><span data-stu-id="79aa9-105">The **FolderView** resource provides or sets recommendations on the user-experience of a folder.</span></span>

<span data-ttu-id="79aa9-106">これは、[driveItem][item-resource] リソースの [folder][folder-facet] プロパティから使用できます。</span><span class="sxs-lookup"><span data-stu-id="79aa9-106">It is available from the [folder][folder-facet] property of [driveItem][item-resource] resources.</span></span>

## <a name="json-representation"></a><span data-ttu-id="79aa9-107">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="79aa9-107">JSON representation</span></span>

<!-- { "blockType": "resource", "@odata.type": "microsoft.graph.folderView" } -->

```json
{
  "sortBy": "default | name | type | size | takenOrCreatedDateTime | lastModifiedDateTime | sequence",
  "sortDescending": "ascending | descending",
  "viewType": "default | icons | details | thumbnails"
}
```

## <a name="properties"></a><span data-ttu-id="79aa9-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="79aa9-108">Properties</span></span>

| <span data-ttu-id="79aa9-109">プロパティ名</span><span class="sxs-lookup"><span data-stu-id="79aa9-109">Property name</span></span>         | <span data-ttu-id="79aa9-110">Type</span><span class="sxs-lookup"><span data-stu-id="79aa9-110">Type</span></span>   | <span data-ttu-id="79aa9-111">説明</span><span class="sxs-lookup"><span data-stu-id="79aa9-111">Description</span></span>
|:----------------------|:-------|:--------------------------------------------
| <span data-ttu-id="79aa9-112">**sortBy**</span><span class="sxs-lookup"><span data-stu-id="79aa9-112">**sortBy**</span></span>            | <span data-ttu-id="79aa9-113">文字列</span><span class="sxs-lookup"><span data-stu-id="79aa9-113">string</span></span> | <span data-ttu-id="79aa9-114">フォルダーの並べ替え方法。</span><span class="sxs-lookup"><span data-stu-id="79aa9-114">The method by which the folder should be sorted.</span></span>
| <span data-ttu-id="79aa9-115">**sortOrder**</span><span class="sxs-lookup"><span data-stu-id="79aa9-115">**sortOrder**</span></span>         | <span data-ttu-id="79aa9-116">文字列</span><span class="sxs-lookup"><span data-stu-id="79aa9-116">string</span></span> | <span data-ttu-id="79aa9-117">true の場合は、アイテムが降順で並べ替えられることを示します。</span><span class="sxs-lookup"><span data-stu-id="79aa9-117">If true, indicates that items should be sorted in descending order.</span></span> <span data-ttu-id="79aa9-118">それ以外の場合は、アイテムが昇順で並べ替えられます。</span><span class="sxs-lookup"><span data-stu-id="79aa9-118">Otherwise, items should be sorted ascending.</span></span>
| <span data-ttu-id="79aa9-119">**viewType**</span><span class="sxs-lookup"><span data-stu-id="79aa9-119">**viewType**</span></span>          | <span data-ttu-id="79aa9-120">文字列</span><span class="sxs-lookup"><span data-stu-id="79aa9-120">string</span></span> | <span data-ttu-id="79aa9-121">フォルダーを表すために使用されるビューの種類。</span><span class="sxs-lookup"><span data-stu-id="79aa9-121">The type of view that should be used to represent the folder.</span></span>

<span data-ttu-id="79aa9-122">_sortBy_ プロパティを使用すると、**viewType** ファセットを優先するアプリケーションで、アイテムの並べ替え順序を制御できます。</span><span class="sxs-lookup"><span data-stu-id="79aa9-122">You can use the _sortBy_ property to control the sort order of the items in applications that respect the **viewType** facet.</span></span>

### <a name="sortby-values"></a><span data-ttu-id="79aa9-123">sortBy の値</span><span class="sxs-lookup"><span data-stu-id="79aa9-123">sortBy values</span></span>

<span data-ttu-id="79aa9-124">**sortBy** プロパティに定義されている値は次のとおりです。</span><span class="sxs-lookup"><span data-stu-id="79aa9-124">The following values are defined for the **sortBy** property.</span></span>

| <span data-ttu-id="79aa9-125">値</span><span class="sxs-lookup"><span data-stu-id="79aa9-125">Value</span></span>                    | <span data-ttu-id="79aa9-126">説明</span><span class="sxs-lookup"><span data-stu-id="79aa9-126">Description</span></span>
| ------------------------ | --------------------------------------------------
| `default`                | <span data-ttu-id="79aa9-127">アプリケーションの既定の並べ替え順序。</span><span class="sxs-lookup"><span data-stu-id="79aa9-127">The default sort order of the application.</span></span>
| `name`                   | <span data-ttu-id="79aa9-128">アイテムは、アイテムの **name** プロパティで整列されます。</span><span class="sxs-lookup"><span data-stu-id="79aa9-128">Items should be arranged by the **name** property of the items.</span></span>
| `type`                   | <span data-ttu-id="79aa9-129">アイテムは、アイテムの種類で整列されます。</span><span class="sxs-lookup"><span data-stu-id="79aa9-129">Items should be arranged by the type of item.</span></span>
| `size`                   | <span data-ttu-id="79aa9-130">アイテムは、アイテムの **size** プロパティで整列されます。</span><span class="sxs-lookup"><span data-stu-id="79aa9-130">Items should be arranged by the **size** property of the items.</span></span>
| `takenOrCreatedDateTime` | <span data-ttu-id="79aa9-131">アイテムは、**photo** ファセットの **takenDateTime** プロパティで整列されます。</span><span class="sxs-lookup"><span data-stu-id="79aa9-131">Items should be arranged by the **takenDateTime** property of the **photo** facet.</span></span> <span data-ttu-id="79aa9-132">これが使用できない場合は、**createdDateTime** プロパティが使用されます。</span><span class="sxs-lookup"><span data-stu-id="79aa9-132">If not available, the **createdDateTime** property should be used.</span></span>
| `lastModifiedDateTime`   | <span data-ttu-id="79aa9-133">アイテムは、アイテムの **lastModifiedDateTime** プロパティで整列されます。</span><span class="sxs-lookup"><span data-stu-id="79aa9-133">Items should be arranged by the **lastModifiedDateTime** property of the items.</span></span>
| `sequence`               | <span data-ttu-id="79aa9-134">アイテムは、ユーザーによって指定されたカスタム順序で並びます。</span><span class="sxs-lookup"><span data-stu-id="79aa9-134">Items follow a custom sequence specified by the user.</span></span>


### <a name="sortorder-values"></a><span data-ttu-id="79aa9-135">sortOrder の値</span><span class="sxs-lookup"><span data-stu-id="79aa9-135">sortOrder values</span></span>

<span data-ttu-id="79aa9-136">**sortOrder** プロパティに定義されている値は次のとおりです。</span><span class="sxs-lookup"><span data-stu-id="79aa9-136">The following values are defined for the **sortOrder** property.</span></span>

| <span data-ttu-id="79aa9-137">値</span><span class="sxs-lookup"><span data-stu-id="79aa9-137">Value</span></span>        | <span data-ttu-id="79aa9-138">説明</span><span class="sxs-lookup"><span data-stu-id="79aa9-138">Description</span></span>
| ------------ | --------------------------------------------------------------
| `ascending`  | <span data-ttu-id="79aa9-139">アイテムは、昇順で整列されます。</span><span class="sxs-lookup"><span data-stu-id="79aa9-139">Items should be arranged in ascending order.</span></span>
| `descending` | <span data-ttu-id="79aa9-140">アイテムは、降順で整列されます。</span><span class="sxs-lookup"><span data-stu-id="79aa9-140">Items should be arranged in descending order.</span></span>


### <a name="viewtype-values"></a><span data-ttu-id="79aa9-141">viewType の値</span><span class="sxs-lookup"><span data-stu-id="79aa9-141">viewType values</span></span>

<span data-ttu-id="79aa9-142">**viewType** プロパティに定義されている値は次のとおりです。</span><span class="sxs-lookup"><span data-stu-id="79aa9-142">The following values are defined for the **viewType** property.</span></span>

| <span data-ttu-id="79aa9-143">値</span><span class="sxs-lookup"><span data-stu-id="79aa9-143">Value</span></span>        | <span data-ttu-id="79aa9-144">説明</span><span class="sxs-lookup"><span data-stu-id="79aa9-144">Description</span></span>
| ------------ | --------------------------------------------------------------
| `default`    | <span data-ttu-id="79aa9-145">アプリケーションの既定のビューの種類。</span><span class="sxs-lookup"><span data-stu-id="79aa9-145">The default view type for the application.</span></span>
| `icons`      | <span data-ttu-id="79aa9-146">driveItem を表すためにアイコンを使用するビュー。</span><span class="sxs-lookup"><span data-stu-id="79aa9-146">A view that uses icons to represent driveItems.</span></span>
| `details`    | <span data-ttu-id="79aa9-147">各アイテムに関する追加の詳細を提示する、複数の列を持つビュー。</span><span class="sxs-lookup"><span data-stu-id="79aa9-147">A view with multiple columns that provide additional details about each item.</span></span>
| `thumbnails` | <span data-ttu-id="79aa9-148">アイテムを表すために driveItem の大きなサムネイルを使用するビュー。</span><span class="sxs-lookup"><span data-stu-id="79aa9-148">A view that uses larger thumbnails of driveItems to represent the items.</span></span>


[item-resource]: driveitem.md
[folder-facet]: folder.md

<!-- uuid: f9e446fd-190b-4692-a605-bb60e78f1f19
2017-05-03 02:34:40 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "folderView resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
