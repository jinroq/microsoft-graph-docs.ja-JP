---
author: JeremyKelley
ms.author: JeremyKelley
ms.date: 09/10/2017
title: プログラム
localization_priority: Normal
description: " または、個別のアイテムではなく、コレクションとして扱われるアイテムのコレクションです。"
ms.prod: ''
doc_type: resourcePageType
ms.openlocfilehash: d8eff13e0cfdc6b355cc289833e7b3050ded2641
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "36035666"
---
# <a name="package-resource-type"></a><span data-ttu-id="e8198-103">Package リソースの種類</span><span class="sxs-lookup"><span data-stu-id="e8198-103">Package resource type</span></span>

<span data-ttu-id="e8198-104">**Package** リソースは、DriveItem が「パッケージ」内で最上位項目であること、または個別の項目ではなくコレクションとして扱うべき項目のコレクションであることを示します。</span><span class="sxs-lookup"><span data-stu-id="e8198-104">The **Package** resource indicates that a DriveItem is the top level item in a "package" or a collection of items that should be treated as a collection instead of individual items.</span></span>

<span data-ttu-id="e8198-p101">OneNote のノートブックはパッケージの一例です。ノートブックがその内容を表すファイルとフォルダーで構成されているのに対し、ノートブックを表す最上位項目は、これが特別な扱いを必要とするデータのコレクションであることをクライアントに示す **package** ファセットを持ちます。</span><span class="sxs-lookup"><span data-stu-id="e8198-p101">An example of a package is a OneNote notebook. While the notebook is made up of files and folders that represent the contents of the notebook, the top level item that represents the notebook has a **package** facet to indicate to clients that this is a collection of data that should be treated special.</span></span>

<span data-ttu-id="e8198-107">**package** ファセットを持つ DriveItems は、**folder** や **file** ファセットを含みませんが、**folder** ファセットを持つ項目に概念的に類似しています。</span><span class="sxs-lookup"><span data-stu-id="e8198-107">DriveItems with the **package** facet do not include a **folder** or **file** facet but are conceptually similar to an item with a **folder** facet.</span></span>

## <a name="json-representation"></a><span data-ttu-id="e8198-108">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="e8198-108">JSON representation</span></span>

<!-- { "blockType": "resource", "@odata.type": "microsoft.graph.package" } -->
```json
{
  "type": "oneNote"
}
```

## <a name="properties"></a><span data-ttu-id="e8198-109">プロパティ</span><span class="sxs-lookup"><span data-stu-id="e8198-109">Properties</span></span>

| <span data-ttu-id="e8198-110">プロパティ名</span><span class="sxs-lookup"><span data-stu-id="e8198-110">Property Name</span></span> | <span data-ttu-id="e8198-111">型</span><span class="sxs-lookup"><span data-stu-id="e8198-111">Type</span></span>   | <span data-ttu-id="e8198-112">説明</span><span class="sxs-lookup"><span data-stu-id="e8198-112">Description</span></span>                                                                                                                                                                      |
|:--------------|:-------|:---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| <span data-ttu-id="e8198-113">type</span><span class="sxs-lookup"><span data-stu-id="e8198-113">type</span></span>          | <span data-ttu-id="e8198-114">string</span><span class="sxs-lookup"><span data-stu-id="e8198-114">string</span></span> | <span data-ttu-id="e8198-115">パッケージの種類を示す文字列。</span><span class="sxs-lookup"><span data-stu-id="e8198-115">A string indicating the type of package.</span></span> <span data-ttu-id="e8198-116">が唯一の現在定義されている値であるとしても、他のパッケージ タイプが返されるものと考え、それぞれに応じた扱いをする必要があります。</span><span class="sxs-lookup"><span data-stu-id="e8198-116">While `oneNote` is the only currently defined value, you should expect other package types to be returned and handle them accordingly.</span></span> |

## <a name="remarks"></a><span data-ttu-id="e8198-117">注釈</span><span class="sxs-lookup"><span data-stu-id="e8198-117">Remarks</span></span> 

<span data-ttu-id="e8198-118">DriveItem のファセットの詳細については、「[DriveItem](driveitem.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="e8198-118">For more information about the facets on a DriveItem, see [DriveItem](driveitem.md).</span></span>


<!-- {
  "type": "#page.annotation",
  "description": "The Package facet indicates that an item is the root of a special collection of items that should be treated as a single unit.",
  "keywords": "package, facet, onenote",
  "section": "documentation",
  "tocPath": "Facets/Package"
} -->
