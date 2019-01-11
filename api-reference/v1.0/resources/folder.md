---
author: rgregg
ms.author: rgregg
ms.date: 09/10/2017
title: Folder
localization_priority: Normal
ms.openlocfilehash: fab5db026b47aa84f7d097a19782b70eac6b6064
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/11/2019
ms.locfileid: "27821421"
---
# <a name="folder-resource-type"></a><span data-ttu-id="89600-102">Folder リソース型</span><span class="sxs-lookup"><span data-stu-id="89600-102">Folder resource type</span></span>

<span data-ttu-id="89600-p101">**フォルダー**リソースは、アイテム上のフォルダー関連のデータを 1 つの構造にグループ化します。**フォルダー**ファセットが null 以外の [**DriveItems**](driveitem.md) は、他の DriveItems のコンテナーです。</span><span class="sxs-lookup"><span data-stu-id="89600-p101">The **Folder** resource groups folder-related data on an item into a single structure. [**DriveItems**](driveitem.md) with a non-null **folder** facet are containers for other DriveItems.</span></span>

## <a name="json-representation"></a><span data-ttu-id="89600-105">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="89600-105">JSON representation</span></span>

<span data-ttu-id="89600-106">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="89600-106">Here is a JSON representation of the resource.</span></span>

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

## <a name="properties"></a><span data-ttu-id="89600-107">プロパティ</span><span class="sxs-lookup"><span data-stu-id="89600-107">Properties</span></span>

| <span data-ttu-id="89600-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="89600-108">Property</span></span>       | <span data-ttu-id="89600-109">型</span><span class="sxs-lookup"><span data-stu-id="89600-109">Type</span></span>           | <span data-ttu-id="89600-110">説明</span><span class="sxs-lookup"><span data-stu-id="89600-110">Description</span></span>
|:---------------|:---------------|:-------------------------------------------
| <span data-ttu-id="89600-111">**childCount**</span><span class="sxs-lookup"><span data-stu-id="89600-111">**childCount**</span></span> | <span data-ttu-id="89600-112">Int32</span><span class="sxs-lookup"><span data-stu-id="89600-112">Int32</span></span>          | <span data-ttu-id="89600-113">このコンテナーの中に含まれる子の数。</span><span class="sxs-lookup"><span data-stu-id="89600-113">Number of children contained immediately within this container.</span></span>
| <span data-ttu-id="89600-114">**view**</span><span class="sxs-lookup"><span data-stu-id="89600-114">**view**</span></span>       | <span data-ttu-id="89600-115">[folderView][]</span><span class="sxs-lookup"><span data-stu-id="89600-115">[folderView][]</span></span> | <span data-ttu-id="89600-116">フォルダーに推奨されるビューを定義するプロパティのコレクション。</span><span class="sxs-lookup"><span data-stu-id="89600-116">A collection of properties defining the recommended view for the folder.</span></span>

## <a name="remarks"></a><span data-ttu-id="89600-117">備考</span><span class="sxs-lookup"><span data-stu-id="89600-117">Remarks</span></span> 

<span data-ttu-id="89600-118">DriveItem のファセットの詳細については、「[DriveItem][]」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="89600-118">For more information about the facets on a DriveItem, see [DriveItem][].</span></span>

[folderView]: folderview.md
[DriveItem]: driveitem.md

<!-- {
  "type": "#page.annotation",
  "description": "The Folder facet describes properties of a folder",
  "keywords": "folder,item,facet",
  "section": "documentation",
  "tocPath": "Facets/Folder"
} -->
