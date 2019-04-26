---
author: JeremyKelley
ms.author: JeremyKelley
ms.date: 09/10/2017
title: フォルダー
localization_priority: Normal
ms.openlocfilehash: 2c98cb57bfd860b568b1cba95ed7f6fcf455eea1
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32564261"
---
# <a name="folder-resource-type"></a><span data-ttu-id="3af27-102">Folder リソース型</span><span class="sxs-lookup"><span data-stu-id="3af27-102">Folder resource type</span></span>

<span data-ttu-id="3af27-p101">**フォルダー**リソースは、アイテム上のフォルダー関連のデータを 1 つの構造にグループ化します。**フォルダー**ファセットが null 以外の **[DriveItems](driveitem.md)** は、他の DriveItems のコンテナーです。</span><span class="sxs-lookup"><span data-stu-id="3af27-p101">The **Folder** resource groups folder-related data on an item into a single structure. [**DriveItems**](driveitem.md) with a non-null **folder** facet are containers for other DriveItems.</span></span>

## <a name="json-representation"></a><span data-ttu-id="3af27-105">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="3af27-105">JSON representation</span></span>

<span data-ttu-id="3af27-106">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="3af27-106">Here is a JSON representation of the resource.</span></span>

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

## <a name="properties"></a><span data-ttu-id="3af27-107">プロパティ</span><span class="sxs-lookup"><span data-stu-id="3af27-107">Properties</span></span>

| <span data-ttu-id="3af27-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="3af27-108">Property</span></span>       | <span data-ttu-id="3af27-109">型</span><span class="sxs-lookup"><span data-stu-id="3af27-109">Type</span></span>           | <span data-ttu-id="3af27-110">説明</span><span class="sxs-lookup"><span data-stu-id="3af27-110">Description</span></span>
|:---------------|:---------------|:-------------------------------------------
| <span data-ttu-id="3af27-111">**childCount**</span><span class="sxs-lookup"><span data-stu-id="3af27-111">**childCount**</span></span> | <span data-ttu-id="3af27-112">Int32</span><span class="sxs-lookup"><span data-stu-id="3af27-112">Int32</span></span>          | <span data-ttu-id="3af27-113">このコンテナーの中に含まれる子の数。</span><span class="sxs-lookup"><span data-stu-id="3af27-113">Number of children contained immediately within this container.</span></span>
| <span data-ttu-id="3af27-114">**view**</span><span class="sxs-lookup"><span data-stu-id="3af27-114">**view**</span></span>       | <span data-ttu-id="3af27-115">[folderView][]</span><span class="sxs-lookup"><span data-stu-id="3af27-115">[folderView][]</span></span> | <span data-ttu-id="3af27-116">フォルダーに推奨されるビューを定義するプロパティのコレクション。</span><span class="sxs-lookup"><span data-stu-id="3af27-116">A collection of properties defining the recommended view for the folder.</span></span>

## <a name="remarks"></a><span data-ttu-id="3af27-117">備考</span><span class="sxs-lookup"><span data-stu-id="3af27-117">Remarks</span></span> 

<span data-ttu-id="3af27-118">DriveItem のファセットの詳細については、「[DriveItem][]」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="3af27-118">For more information about the facets on a DriveItem, see [DriveItem][].</span></span>

[folderView]: folderview.md
[DriveItem]: driveitem.md

<!-- {
  "type": "#page.annotation",
  "description": "The Folder facet describes properties of a folder",
  "keywords": "folder,item,facet",
  "section": "documentation",
  "tocPath": "Facets/Folder"
} -->
