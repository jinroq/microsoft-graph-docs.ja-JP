---
author: rgregg
ms.author: rgregg
ms.date: 09/10/2017
title: FolderView
ms.openlocfilehash: 1658751371f3a3ae186d5a092ae5610f016d26b4
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27066778"
---
# <a name="folderview-resource-type"></a><span data-ttu-id="9d080-102">FolderView リソースの種類</span><span class="sxs-lookup"><span data-stu-id="9d080-102">FolderView resource type</span></span>

> <span data-ttu-id="9d080-103">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="9d080-103">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="9d080-104">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="9d080-104">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="9d080-105">**FolderView** リソースは、フォルダーのユーザー エクスペリエンスに関する推奨事項を提供または設定します。</span><span class="sxs-lookup"><span data-stu-id="9d080-105">The **FolderView** resource provides or sets recommendations on the user-experience of a folder.</span></span>

<span data-ttu-id="9d080-106">これは、[driveItem][item-resource] リソースの [folder][folder-facet] プロパティから使用できます。</span><span class="sxs-lookup"><span data-stu-id="9d080-106">It is available from the [folder][folder-facet] property of [driveItem][item-resource] resources.</span></span>

## <a name="json-representation"></a><span data-ttu-id="9d080-107">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="9d080-107">JSON representation</span></span>

<!-- { "blockType": "resource", "@odata.type": "microsoft.graph.folderView" } -->

```json
{
  "sortBy": "default | name | type | size | takenOrCreatedDateTime | lastModifiedDateTime | sequence",
  "sortDescending": "ascending | descending",
  "viewType": "default | icons | details | thumbnails"
}
```

## <a name="properties"></a><span data-ttu-id="9d080-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="9d080-108">Properties</span></span>

| <span data-ttu-id="9d080-109">プロパティ名</span><span class="sxs-lookup"><span data-stu-id="9d080-109">Property name</span></span>         | <span data-ttu-id="9d080-110">型</span><span class="sxs-lookup"><span data-stu-id="9d080-110">Type</span></span>   | <span data-ttu-id="9d080-111">説明</span><span class="sxs-lookup"><span data-stu-id="9d080-111">Description</span></span>
|:----------------------|:-------|:--------------------------------------------
| <span data-ttu-id="9d080-112">**sortBy**</span><span class="sxs-lookup"><span data-stu-id="9d080-112">**sortBy**</span></span>            | <span data-ttu-id="9d080-113">文字列</span><span class="sxs-lookup"><span data-stu-id="9d080-113">string</span></span> | <span data-ttu-id="9d080-114">フォルダーの並べ替え方法。</span><span class="sxs-lookup"><span data-stu-id="9d080-114">The method by which the folder should be sorted.</span></span>
| <span data-ttu-id="9d080-115">**sortOrder**</span><span class="sxs-lookup"><span data-stu-id="9d080-115">**sortOrder**</span></span>         | <span data-ttu-id="9d080-116">文字列</span><span class="sxs-lookup"><span data-stu-id="9d080-116">string</span></span> | <span data-ttu-id="9d080-117">true の場合は、アイテムが降順で並べ替えられることを示します。</span><span class="sxs-lookup"><span data-stu-id="9d080-117">If true, indicates that items should be sorted in descending order.</span></span> <span data-ttu-id="9d080-118">それ以外の場合は、アイテムが昇順で並べ替えられます。</span><span class="sxs-lookup"><span data-stu-id="9d080-118">Otherwise, items should be sorted ascending.</span></span>
| <span data-ttu-id="9d080-119">**viewType**</span><span class="sxs-lookup"><span data-stu-id="9d080-119">**viewType**</span></span>          | <span data-ttu-id="9d080-120">文字列</span><span class="sxs-lookup"><span data-stu-id="9d080-120">string</span></span> | <span data-ttu-id="9d080-121">フォルダーを表すために使用されるビューの種類。</span><span class="sxs-lookup"><span data-stu-id="9d080-121">The type of view that should be used to represent the folder.</span></span>

<span data-ttu-id="9d080-122">_sortBy_ プロパティを使用すると、**viewType** ファセットを優先するアプリケーションで、アイテムの並べ替え順序を制御できます。</span><span class="sxs-lookup"><span data-stu-id="9d080-122">You can use the _sortBy_ property to control the sort order of the items in applications that respect the **viewType** facet.</span></span>

### <a name="sortby-values"></a><span data-ttu-id="9d080-123">sortBy の値</span><span class="sxs-lookup"><span data-stu-id="9d080-123">sortBy values</span></span>

<span data-ttu-id="9d080-124">**sortBy** プロパティに定義されている値は次のとおりです。</span><span class="sxs-lookup"><span data-stu-id="9d080-124">The following values are defined for the **sortBy** property.</span></span>

| <span data-ttu-id="9d080-125">値</span><span class="sxs-lookup"><span data-stu-id="9d080-125">Value</span></span>                    | <span data-ttu-id="9d080-126">説明</span><span class="sxs-lookup"><span data-stu-id="9d080-126">Description</span></span>
| ------------------------ | --------------------------------------------------
| `default`                | <span data-ttu-id="9d080-127">アプリケーションの既定の並べ替え順序。</span><span class="sxs-lookup"><span data-stu-id="9d080-127">The default sort order of the application.</span></span>
| `name`                   | <span data-ttu-id="9d080-128">アイテムは、アイテムの **name** プロパティで整列されます。</span><span class="sxs-lookup"><span data-stu-id="9d080-128">Items should be arranged by the **name** property of the items.</span></span>
| `type`                   | <span data-ttu-id="9d080-129">アイテムは、アイテムの種類で整列されます。</span><span class="sxs-lookup"><span data-stu-id="9d080-129">Items should be arranged by the type of item.</span></span>
| `size`                   | <span data-ttu-id="9d080-130">アイテムは、アイテムの **size** プロパティで整列されます。</span><span class="sxs-lookup"><span data-stu-id="9d080-130">Items should be arranged by the **size** property of the items.</span></span>
| `takenOrCreatedDateTime` | <span data-ttu-id="9d080-131">アイテムは、**photo** ファセットの **takenDateTime** プロパティで整列されます。</span><span class="sxs-lookup"><span data-stu-id="9d080-131">Items should be arranged by the **takenDateTime** property of the **photo** facet.</span></span> <span data-ttu-id="9d080-132">これが使用できない場合は、**createdDateTime** プロパティが使用されます。</span><span class="sxs-lookup"><span data-stu-id="9d080-132">If not available, the **createdDateTime** property should be used.</span></span>
| `lastModifiedDateTime`   | <span data-ttu-id="9d080-133">アイテムは、アイテムの **lastModifiedDateTime** プロパティで整列されます。</span><span class="sxs-lookup"><span data-stu-id="9d080-133">Items should be arranged by the **lastModifiedDateTime** property of the items.</span></span>
| `sequence`               | <span data-ttu-id="9d080-134">アイテムは、ユーザーによって指定されたカスタム順序で並びます。</span><span class="sxs-lookup"><span data-stu-id="9d080-134">Items follow a custom sequence specified by the user.</span></span>


### <a name="sortorder-values"></a><span data-ttu-id="9d080-135">sortOrder の値</span><span class="sxs-lookup"><span data-stu-id="9d080-135">sortOrder values</span></span>

<span data-ttu-id="9d080-136">**sortOrder** プロパティに定義されている値は次のとおりです。</span><span class="sxs-lookup"><span data-stu-id="9d080-136">The following values are defined for the **sortOrder** property.</span></span>

| <span data-ttu-id="9d080-137">値</span><span class="sxs-lookup"><span data-stu-id="9d080-137">Value</span></span>        | <span data-ttu-id="9d080-138">説明</span><span class="sxs-lookup"><span data-stu-id="9d080-138">Description</span></span>
| ------------ | --------------------------------------------------------------
| `ascending`  | <span data-ttu-id="9d080-139">アイテムは、昇順で整列されます。</span><span class="sxs-lookup"><span data-stu-id="9d080-139">Items should be arranged in ascending order.</span></span>
| `descending` | <span data-ttu-id="9d080-140">アイテムは、降順で整列されます。</span><span class="sxs-lookup"><span data-stu-id="9d080-140">Items should be arranged in descending order.</span></span>


### <a name="viewtype-values"></a><span data-ttu-id="9d080-141">viewType の値</span><span class="sxs-lookup"><span data-stu-id="9d080-141">viewType values</span></span>

<span data-ttu-id="9d080-142">**viewType** プロパティに定義されている値は次のとおりです。</span><span class="sxs-lookup"><span data-stu-id="9d080-142">The following values are defined for the **viewType** property.</span></span>

| <span data-ttu-id="9d080-143">値</span><span class="sxs-lookup"><span data-stu-id="9d080-143">Value</span></span>        | <span data-ttu-id="9d080-144">説明</span><span class="sxs-lookup"><span data-stu-id="9d080-144">Description</span></span>
| ------------ | --------------------------------------------------------------
| `default`    | <span data-ttu-id="9d080-145">アプリケーションの既定のビューの種類。</span><span class="sxs-lookup"><span data-stu-id="9d080-145">The default view type for the application.</span></span>
| `icons`      | <span data-ttu-id="9d080-146">driveItem を表すためにアイコンを使用するビュー。</span><span class="sxs-lookup"><span data-stu-id="9d080-146">A view that uses icons to represent driveItems.</span></span>
| `details`    | <span data-ttu-id="9d080-147">各アイテムに関する追加の詳細を提示する、複数の列を持つビュー。</span><span class="sxs-lookup"><span data-stu-id="9d080-147">A view with multiple columns that provide additional details about each item.</span></span>
| `thumbnails` | <span data-ttu-id="9d080-148">アイテムを表すために driveItem の大きなサムネイルを使用するビュー。</span><span class="sxs-lookup"><span data-stu-id="9d080-148">A view that uses larger thumbnails of driveItems to represent the items.</span></span>


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
