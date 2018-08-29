---
author: rgregg
ms.author: rgregg
ms.date: 09/10/2017
title: Folder
ms.openlocfilehash: c0ab787f1c1f04ff77eeb69979dc6a825d4f3c33
ms.sourcegitcommit: abf4b739257e3ffd9d045f783ec595d846172590
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/21/2018
ms.locfileid: "23266563"
---
# <a name="folder-resource-type"></a><span data-ttu-id="43dd9-102">Folder リソース型</span><span class="sxs-lookup"><span data-stu-id="43dd9-102">Folder resource type</span></span>

<span data-ttu-id="43dd9-p101">**フォルダー**リソースは、アイテム上のフォルダー関連のデータを 1 つの構造にグループ化します。**フォルダー**ファセットが null 以外の [**DriveItems**](driveitem.md) は、他の DriveItems のコンテナーです。</span><span class="sxs-lookup"><span data-stu-id="43dd9-p101">The **Folder** resource groups folder-related data on an item into a single structure. [**DriveItems**](driveitem.md) with a non-null **folder** facet are containers for other DriveItems.</span></span>

## <a name="json-representation"></a><span data-ttu-id="43dd9-105">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="43dd9-105">JSON representation</span></span>

<span data-ttu-id="43dd9-106">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="43dd9-106">Here is a JSON representation of the resource.</span></span>

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

## <a name="properties"></a><span data-ttu-id="43dd9-107">プロパティ</span><span class="sxs-lookup"><span data-stu-id="43dd9-107">Properties</span></span>

| <span data-ttu-id="43dd9-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="43dd9-108">Property</span></span>       | <span data-ttu-id="43dd9-109">型</span><span class="sxs-lookup"><span data-stu-id="43dd9-109">Type</span></span>           | <span data-ttu-id="43dd9-110">説明</span><span class="sxs-lookup"><span data-stu-id="43dd9-110">Description</span></span>
|:---------------|:---------------|:-------------------------------------------
| <span data-ttu-id="43dd9-111">**childCount**</span><span class="sxs-lookup"><span data-stu-id="43dd9-111">**childCount**</span></span> | <span data-ttu-id="43dd9-112">Int32</span><span class="sxs-lookup"><span data-stu-id="43dd9-112">Int32</span></span>          | <span data-ttu-id="43dd9-113">このコンテナーの中に含まれる子の数。</span><span class="sxs-lookup"><span data-stu-id="43dd9-113">Number of children contained immediately within this container.</span></span>
| <span data-ttu-id="43dd9-114">**view**</span><span class="sxs-lookup"><span data-stu-id="43dd9-114">**view**</span></span>       | <span data-ttu-id="43dd9-115">[folderView][]</span><span class="sxs-lookup"><span data-stu-id="43dd9-115">[folderView][]</span></span> | <span data-ttu-id="43dd9-116">フォルダーの推奨ビューを定義するプロパティのコレクション。</span><span class="sxs-lookup"><span data-stu-id="43dd9-116">A collection of properties defining the recommended view for the folder.</span></span>

## <a name="remarks"></a><span data-ttu-id="43dd9-117">備考</span><span class="sxs-lookup"><span data-stu-id="43dd9-117">Remarks</span></span> 

<span data-ttu-id="43dd9-118">DriveItem のファセットの詳細については、「[DriveItem][]」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="43dd9-118">For more information about the facets on a DriveItem, see [DriveItem][].</span></span>

[folderView]: folderView.md
[DriveItem]: driveItem.md

<!-- {
  "type": "#page.annotation",
  "description": "The Folder facet describes properties of a folder",
  "keywords": "folder,item,facet",
  "section": "documentation",
  "tocPath": "Facets/Folder"
} -->
