---
author: JeremyKelley
ms.author: jeremyke
title: バンドルリソースの種類
description: 他のドライブ項目の論理グループであるドライブ項目を記述するファセット
localization_priority: Normal
ms.prod: sharepoint
ms.openlocfilehash: 596dc8a77ce5b1e580b14e3e5c56c9e985b0dfbf
ms.sourcegitcommit: 56c0b609dfb1bc5d900956f407d107cdab7086e8
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/30/2019
ms.locfileid: "35932877"
---
# <a name="bundle-resource-type"></a><span data-ttu-id="d1068-103">バンドルリソースの種類</span><span class="sxs-lookup"><span data-stu-id="d1068-103">bundle resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="d1068-104">バンドルとは、一度に複数のファイルを共有するために使用されるファイルの論理的なグループです。</span><span class="sxs-lookup"><span data-stu-id="d1068-104">A bundle is a logical grouping of files used to share multiple files at once.</span></span> <span data-ttu-id="d1068-105">ファセットが含まれている[ハードドライブ][]エンティティで表され、他のすべての drive アイテムと同じ方法で共有できます。 `bundle`</span><span class="sxs-lookup"><span data-stu-id="d1068-105">It is represented by a [driveItem][] entity containing a `bundle` facet and can be shared in the same way as any other driveItem.</span></span>

<span data-ttu-id="d1068-106">`bundle` [ドライブアイテム][]のファセットは、アイテムをバンドルとして識別し、バンドル固有の情報を1つの構造にグループ化します。</span><span class="sxs-lookup"><span data-stu-id="d1068-106">The `bundle` facet on a [driveItem][] identifies an item as a bundle and groups bundle-specific information into a single structure.</span></span> <span data-ttu-id="d1068-107">このファイルは、**バンドル**エンドポイントから返される[ドライブ項目][]リソースにのみ含まれます。</span><span class="sxs-lookup"><span data-stu-id="d1068-107">It is only included on [driveItem][] resources returned from the **bundles** endpoint.</span></span>

<span data-ttu-id="d1068-108">`bundle`リソースの種類自体は自身のエンティティではないことに注意してください。また、[ドライブアイテム][]のファセットでしかありません。</span><span class="sxs-lookup"><span data-stu-id="d1068-108">Note that the `bundle` resource type itself is not an entity of its own, and is only a facet on a [driveItem][].</span></span> <span data-ttu-id="d1068-109">ドライブ`bundles`上のコレクション[][]の種類は、drive [item][]では`bundle`ありません。</span><span class="sxs-lookup"><span data-stu-id="d1068-109">The `bundles` collection on a [drive][] is of type [driveItem][], not `bundle`.</span></span>

## <a name="methods"></a><span data-ttu-id="d1068-110">メソッド</span><span class="sxs-lookup"><span data-stu-id="d1068-110">Methods</span></span>

|                        <span data-ttu-id="d1068-111">メソッド</span><span class="sxs-lookup"><span data-stu-id="d1068-111">Method</span></span>             |         <span data-ttu-id="d1068-112">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="d1068-112">Return type</span></span>      | <span data-ttu-id="d1068-113">説明</span><span class="sxs-lookup"><span data-stu-id="d1068-113">Description</span></span>        |
| :---------------------------------------- | :----------------------- | :------------------|
| <span data-ttu-id="d1068-114">[リストバンドル][bundle-list]</span><span class="sxs-lookup"><span data-stu-id="d1068-114">[List bundles][bundle-list]</span></span>               | <span data-ttu-id="d1068-115">[driveItem][] コレクション</span><span class="sxs-lookup"><span data-stu-id="d1068-115">[driveItem][] collection</span></span> | <span data-ttu-id="d1068-116">ドライブ内のすべてのバンドルを一覧表示する</span><span class="sxs-lookup"><span data-stu-id="d1068-116">List all bundles in a drive</span></span> |
| <span data-ttu-id="d1068-117">[バンドルを取得する][bundle-get]</span><span class="sxs-lookup"><span data-stu-id="d1068-117">[Get bundle][bundle-get]</span></span>                  | <span data-ttu-id="d1068-118">[driveItem][]</span><span class="sxs-lookup"><span data-stu-id="d1068-118">[driveItem][]</span></span>            | <span data-ttu-id="d1068-119">バンドルメタデータを取得する</span><span class="sxs-lookup"><span data-stu-id="d1068-119">Get bundle metadata</span></span> |
| <span data-ttu-id="d1068-120">[バンドルを作成する][bundle-create]</span><span class="sxs-lookup"><span data-stu-id="d1068-120">[Create bundle][bundle-create]</span></span>            | <span data-ttu-id="d1068-121">[driveItem][]</span><span class="sxs-lookup"><span data-stu-id="d1068-121">[driveItem][]</span></span>            | <span data-ttu-id="d1068-122">新しいバンドルを作成する</span><span class="sxs-lookup"><span data-stu-id="d1068-122">Create a new bundle</span></span> |
| <span data-ttu-id="d1068-123">[アイテムを追加する][bundle-add-item]</span><span class="sxs-lookup"><span data-stu-id="d1068-123">[Add item][bundle-add-item]</span></span>               | <span data-ttu-id="d1068-124">None</span><span class="sxs-lookup"><span data-stu-id="d1068-124">None</span></span>                     | <span data-ttu-id="d1068-125">既存のバンドルに[ドライブ項目][]を追加する</span><span class="sxs-lookup"><span data-stu-id="d1068-125">Add a [driveItem][] to an existing bundle</span></span> |
| <span data-ttu-id="d1068-126">[アイテムの削除][bundle-remove-item]</span><span class="sxs-lookup"><span data-stu-id="d1068-126">[Remove item][bundle-remove-item]</span></span>         | <span data-ttu-id="d1068-127">None</span><span class="sxs-lookup"><span data-stu-id="d1068-127">None</span></span>                     | <span data-ttu-id="d1068-128">既存のバンドルからの[ドライブ項目][]の削除</span><span class="sxs-lookup"><span data-stu-id="d1068-128">Remove a [driveItem][] from an existing bundle</span></span> |
| <span data-ttu-id="d1068-129">[バンドルの更新][bundle-update]</span><span class="sxs-lookup"><span data-stu-id="d1068-129">[Update bundle][bundle-update]</span></span>            | <span data-ttu-id="d1068-130">[driveItem][]</span><span class="sxs-lookup"><span data-stu-id="d1068-130">[driveItem][]</span></span>            | <span data-ttu-id="d1068-131">バンドルメタデータの更新</span><span class="sxs-lookup"><span data-stu-id="d1068-131">Update bundle metadata</span></span> |
| <span data-ttu-id="d1068-132">[バンドルの削除][bundle-delete]</span><span class="sxs-lookup"><span data-stu-id="d1068-132">[Delete bundle][bundle-delete]</span></span>            | <span data-ttu-id="d1068-133">None</span><span class="sxs-lookup"><span data-stu-id="d1068-133">None</span></span>                     | <span data-ttu-id="d1068-134">バンドルの削除</span><span class="sxs-lookup"><span data-stu-id="d1068-134">Delete bundle</span></span> |


## <a name="properties"></a><span data-ttu-id="d1068-135">プロパティ</span><span class="sxs-lookup"><span data-stu-id="d1068-135">Properties</span></span>

| <span data-ttu-id="d1068-136">プロパティ名</span><span class="sxs-lookup"><span data-stu-id="d1068-136">Property name</span></span> | <span data-ttu-id="d1068-137">種類</span><span class="sxs-lookup"><span data-stu-id="d1068-137">Type</span></span>      | <span data-ttu-id="d1068-138">説明</span><span class="sxs-lookup"><span data-stu-id="d1068-138">Description</span></span>
|:--------------|:----------|:------------------------------------------------
| <span data-ttu-id="d1068-139">childCount</span><span class="sxs-lookup"><span data-stu-id="d1068-139">childCount</span></span>    | <span data-ttu-id="d1068-140">Int32</span><span class="sxs-lookup"><span data-stu-id="d1068-140">Int32</span></span>     | <span data-ttu-id="d1068-141">このコンテナーの中に含まれる子の数。</span><span class="sxs-lookup"><span data-stu-id="d1068-141">Number of children contained immediately within this container.</span></span>
| <span data-ttu-id="d1068-142">album</span><span class="sxs-lookup"><span data-stu-id="d1068-142">album</span></span>         | <span data-ttu-id="d1068-143">[album][]</span><span class="sxs-lookup"><span data-stu-id="d1068-143">[album][]</span></span> | <span data-ttu-id="d1068-144">バンドルが[アルバム][]の場合は、プロパティが`album`含まれます。</span><span class="sxs-lookup"><span data-stu-id="d1068-144">If the bundle is an [album][], then the `album` property is included</span></span>

## <a name="json-representation"></a><span data-ttu-id="d1068-145">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="d1068-145">JSON representation</span></span>

<!-- { "blockType": "resource", "@odata.type": "microsoft.graph.bundle" } -->
```json
{
  "childCount": 3,
  "album": { "@odata.type": "microsoft.graph.album" },
}
```

[album]: album.md
[drive]: drive.md
[driveItem]: driveItem.md

[bundle-list]: ../api/bundle-list.md
[bundle-get]: ../api/bundle-get.md
[bundle-create]: ../api/drive-post-bundles.md
[bundle-add-item]: ../api/bundle-addItem.md
[bundle-remove-item]: ../api/bundle-removeItem.md
[bundle-update]: ../api/bundle-update.md
[bundle-delete]: ../api/bundle-delete.md
