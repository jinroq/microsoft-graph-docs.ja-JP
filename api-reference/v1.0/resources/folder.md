---
author: JeremyKelley
ms.author: JeremyKelley
ms.date: 09/10/2017
title: フォルダー
localization_priority: Normal
ms.openlocfilehash: 2c98cb57bfd860b568b1cba95ed7f6fcf455eea1
ms.sourcegitcommit: b877a8dc9aeaf74f975ca495b401ffff001d7699
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 03/08/2019
ms.locfileid: "30480818"
---
# <a name="folder-resource-type"></a><span data-ttu-id="0af3e-102">Folder リソース型</span><span class="sxs-lookup"><span data-stu-id="0af3e-102">Folder resource type</span></span>

<span data-ttu-id="0af3e-p101">**フォルダー**リソースは、アイテム上のフォルダー関連のデータを 1 つの構造にグループ化します。**フォルダー**ファセットが null 以外の **[DriveItems](driveitem.md)** は、他の DriveItems のコンテナーです。</span><span class="sxs-lookup"><span data-stu-id="0af3e-p101">The **Folder** resource groups folder-related data on an item into a single structure. [**DriveItems**](driveitem.md) with a non-null **folder** facet are containers for other DriveItems.</span></span>

## <a name="json-representation"></a><span data-ttu-id="0af3e-105">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="0af3e-105">JSON representation</span></span>

<span data-ttu-id="0af3e-106">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="0af3e-106">Here is a JSON representation of the resource.</span></span>

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

## <a name="properties"></a><span data-ttu-id="0af3e-107">プロパティ</span><span class="sxs-lookup"><span data-stu-id="0af3e-107">Properties</span></span>

| <span data-ttu-id="0af3e-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="0af3e-108">Property</span></span>       | <span data-ttu-id="0af3e-109">種類</span><span class="sxs-lookup"><span data-stu-id="0af3e-109">Type</span></span>           | <span data-ttu-id="0af3e-110">説明</span><span class="sxs-lookup"><span data-stu-id="0af3e-110">Description</span></span>
|:---------------|:---------------|:-------------------------------------------
| <span data-ttu-id="0af3e-111">**childCount**</span><span class="sxs-lookup"><span data-stu-id="0af3e-111">**childCount**</span></span> | <span data-ttu-id="0af3e-112">Int32</span><span class="sxs-lookup"><span data-stu-id="0af3e-112">Int32</span></span>          | <span data-ttu-id="0af3e-113">このコンテナーの中に含まれる子の数。</span><span class="sxs-lookup"><span data-stu-id="0af3e-113">Number of children contained immediately within this container.</span></span>
| <span data-ttu-id="0af3e-114">**view**</span><span class="sxs-lookup"><span data-stu-id="0af3e-114">**view**</span></span>       | <span data-ttu-id="0af3e-115">[folderView][]</span><span class="sxs-lookup"><span data-stu-id="0af3e-115">[folderView][]</span></span> | <span data-ttu-id="0af3e-116">フォルダーに推奨されるビューを定義するプロパティのコレクション。</span><span class="sxs-lookup"><span data-stu-id="0af3e-116">A collection of properties defining the recommended view for the folder.</span></span>

## <a name="remarks"></a><span data-ttu-id="0af3e-117">備考</span><span class="sxs-lookup"><span data-stu-id="0af3e-117">Remarks</span></span> 

<span data-ttu-id="0af3e-118">DriveItem のファセットの詳細については、「[DriveItem][]」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="0af3e-118">For more information about the facets on a DriveItem, see [DriveItem][].</span></span>

[folderView]: folderview.md
[DriveItem]: driveitem.md

<!-- {
  "type": "#page.annotation",
  "description": "The Folder facet describes properties of a folder",
  "keywords": "folder,item,facet",
  "section": "documentation",
  "tocPath": "Facets/Folder"
} -->
