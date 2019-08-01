---
author: JeremyKelley
ms.author: JeremyKelley
ms.date: 09/10/2017
title: フォルダー
localization_priority: Normal
description: 'Folder リソースは、アイテム上のフォルダー関連のデータを 1 つの構造にグループ化します。 '
ms.prod: ''
doc_type: resourcePageType
ms.openlocfilehash: f4b43c672b297ce50a5a6aa3dbb3f3d83a1d53be
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "36030332"
---
# <a name="folder-resource-type"></a><span data-ttu-id="e49aa-103">Folder リソース型</span><span class="sxs-lookup"><span data-stu-id="e49aa-103">Folder resource type</span></span>

<span data-ttu-id="e49aa-p101">**フォルダー**リソースは、アイテム上のフォルダー関連のデータを 1 つの構造にグループ化します。**フォルダー**ファセットが null 以外の **[DriveItems](driveitem.md)** は、他の DriveItems のコンテナーです。</span><span class="sxs-lookup"><span data-stu-id="e49aa-p101">The **Folder** resource groups folder-related data on an item into a single structure. [**DriveItems**](driveitem.md) with a non-null **folder** facet are containers for other DriveItems.</span></span>

## <a name="json-representation"></a><span data-ttu-id="e49aa-106">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="e49aa-106">JSON representation</span></span>

<span data-ttu-id="e49aa-107">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="e49aa-107">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.folder"
}-->

```json
{
  "childCount": 1024,
  "view": { "@odata.type": "microsoft.graph.folderView" }
}
```

## <a name="properties"></a><span data-ttu-id="e49aa-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="e49aa-108">Properties</span></span>

| <span data-ttu-id="e49aa-109">プロパティ</span><span class="sxs-lookup"><span data-stu-id="e49aa-109">Property</span></span>       | <span data-ttu-id="e49aa-110">型</span><span class="sxs-lookup"><span data-stu-id="e49aa-110">Type</span></span>           | <span data-ttu-id="e49aa-111">説明</span><span class="sxs-lookup"><span data-stu-id="e49aa-111">Description</span></span>
|:---------------|:---------------|:-------------------------------------------
| <span data-ttu-id="e49aa-112">**childCount**</span><span class="sxs-lookup"><span data-stu-id="e49aa-112">**childCount**</span></span> | <span data-ttu-id="e49aa-113">Int32</span><span class="sxs-lookup"><span data-stu-id="e49aa-113">Int32</span></span>          | <span data-ttu-id="e49aa-114">このコンテナーの中に含まれる子の数。</span><span class="sxs-lookup"><span data-stu-id="e49aa-114">Number of children contained immediately within this container.</span></span>
| <span data-ttu-id="e49aa-115">**view**</span><span class="sxs-lookup"><span data-stu-id="e49aa-115">**view**</span></span>       | <span data-ttu-id="e49aa-116">[folderView][]</span><span class="sxs-lookup"><span data-stu-id="e49aa-116">[folderView][]</span></span> | <span data-ttu-id="e49aa-117">フォルダーに推奨されるビューを定義するプロパティのコレクション。</span><span class="sxs-lookup"><span data-stu-id="e49aa-117">A collection of properties defining the recommended view for the folder.</span></span>

## <a name="remarks"></a><span data-ttu-id="e49aa-118">備考</span><span class="sxs-lookup"><span data-stu-id="e49aa-118">Remarks</span></span> 

<span data-ttu-id="e49aa-119">DriveItem のファセットの詳細については、「[DriveItem][]」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="e49aa-119">For more information about the facets on a DriveItem, see [DriveItem][].</span></span>

[folderView]: folderview.md
[DriveItem]: driveitem.md

<!-- {
  "type": "#page.annotation",
  "description": "The Folder facet describes properties of a folder",
  "keywords": "folder,item,facet",
  "section": "documentation",
  "tocPath": "Facets/Folder"
} -->
