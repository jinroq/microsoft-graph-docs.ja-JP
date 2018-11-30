---
author: rgregg
ms.author: rgregg
ms.date: 09/10/2017
title: Folder
ms.openlocfilehash: dc90624b14a88d06b45302f421a7e3fcfa802a67
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27020262"
---
# <a name="folder-resource-type"></a><span data-ttu-id="6c83d-102">Folder リソース型</span><span class="sxs-lookup"><span data-stu-id="6c83d-102">Folder resource type</span></span>

<span data-ttu-id="6c83d-p101">**フォルダー**リソースは、アイテム上のフォルダー関連のデータを 1 つの構造にグループ化します。**フォルダー**ファセットが null 以外の [**DriveItems**](driveitem.md) は、他の DriveItems のコンテナーです。</span><span class="sxs-lookup"><span data-stu-id="6c83d-p101">The **Folder** resource groups folder-related data on an item into a single structure. [**DriveItems**](driveitem.md) with a non-null **folder** facet are containers for other DriveItems.</span></span>

## <a name="json-representation"></a><span data-ttu-id="6c83d-105">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="6c83d-105">JSON representation</span></span>

<span data-ttu-id="6c83d-106">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="6c83d-106">Here is a JSON representation of the resource.</span></span>

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

## <a name="properties"></a><span data-ttu-id="6c83d-107">プロパティ</span><span class="sxs-lookup"><span data-stu-id="6c83d-107">Properties</span></span>

| <span data-ttu-id="6c83d-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="6c83d-108">Property</span></span>       | <span data-ttu-id="6c83d-109">型</span><span class="sxs-lookup"><span data-stu-id="6c83d-109">Type</span></span>           | <span data-ttu-id="6c83d-110">説明</span><span class="sxs-lookup"><span data-stu-id="6c83d-110">Description</span></span>
|:---------------|:---------------|:-------------------------------------------
| <span data-ttu-id="6c83d-111">**childCount**</span><span class="sxs-lookup"><span data-stu-id="6c83d-111">**childCount**</span></span> | <span data-ttu-id="6c83d-112">Int32</span><span class="sxs-lookup"><span data-stu-id="6c83d-112">Int32</span></span>          | <span data-ttu-id="6c83d-113">このコンテナーの中に含まれる子の数。</span><span class="sxs-lookup"><span data-stu-id="6c83d-113">Number of children contained immediately within this container.</span></span>
| <span data-ttu-id="6c83d-114">**view**</span><span class="sxs-lookup"><span data-stu-id="6c83d-114">**view**</span></span>       | <span data-ttu-id="6c83d-115">[folderView][]</span><span class="sxs-lookup"><span data-stu-id="6c83d-115">[folderView][]</span></span> | <span data-ttu-id="6c83d-116">フォルダーに推奨されるビューを定義するプロパティのコレクション。</span><span class="sxs-lookup"><span data-stu-id="6c83d-116">A collection of properties defining the recommended view for the folder.</span></span>

## <a name="remarks"></a><span data-ttu-id="6c83d-117">備考</span><span class="sxs-lookup"><span data-stu-id="6c83d-117">Remarks</span></span> 

<span data-ttu-id="6c83d-118">DriveItem のファセットの詳細については、「[DriveItem][]」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="6c83d-118">For more information about the facets on a DriveItem, see [DriveItem][].</span></span>

[folderView]: folderview.md
[DriveItem]: driveitem.md

<!-- {
  "type": "#page.annotation",
  "description": "The Folder facet describes properties of a folder",
  "keywords": "folder,item,facet",
  "section": "documentation",
  "tocPath": "Facets/Folder"
} -->
