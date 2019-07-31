---
author: JeremyKelley
description: " または、個別のアイテムではなく、コレクションとして扱われるアイテムのコレクションです。"
ms.date: 09/10/2017
title: プログラム
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
ms.openlocfilehash: 6ae382d1f69a88d814339370264dc5dc7fac9414
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "35966266"
---
# <a name="package-resource-type"></a><span data-ttu-id="9ea1e-103">Package リソースの種類</span><span class="sxs-lookup"><span data-stu-id="9ea1e-103">Package resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="9ea1e-104">**Package** リソースは、DriveItem が「パッケージ」内で最上位項目であること、または個別の項目ではなくコレクションとして扱うべき項目のコレクションであることを示します。</span><span class="sxs-lookup"><span data-stu-id="9ea1e-104">The **Package** resource indicates that a DriveItem is the top level item in a "package" or a collection of items that should be treated as a collection instead of individual items.</span></span>

<span data-ttu-id="9ea1e-p101">OneNote のノートブックはパッケージの一例です。ノートブックがその内容を表すファイルとフォルダーで構成されているのに対し、ノートブックを表す最上位項目は、これが特別な扱いを必要とするデータのコレクションであることをクライアントに示す **package** ファセットを持ちます。</span><span class="sxs-lookup"><span data-stu-id="9ea1e-p101">An example of a package is a OneNote notebook. While the notebook is made up of files and folders that represent the contents of the notebook, the top level item that represents the notebook has a **package** facet to indicate to clients that this is a collection of data that should be treated special.</span></span>

<span data-ttu-id="9ea1e-107">**package** ファセットを持つ DriveItems は、**folder** や **file** ファセットを含みませんが、**folder** ファセットを持つ項目に概念的に類似しています。</span><span class="sxs-lookup"><span data-stu-id="9ea1e-107">DriveItems with the **package** facet do not include a **folder** or **file** facet but are conceptually similar to an item with a **folder** facet.</span></span>

## <a name="json-representation"></a><span data-ttu-id="9ea1e-108">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="9ea1e-108">JSON representation</span></span>

<!-- { "blockType": "resource", "@odata.type": "microsoft.graph.package" } -->
```json
{
  "type": "oneNote"
}
```

| <span data-ttu-id="9ea1e-109">プロパティ名</span><span class="sxs-lookup"><span data-stu-id="9ea1e-109">Property Name</span></span> | <span data-ttu-id="9ea1e-110">型</span><span class="sxs-lookup"><span data-stu-id="9ea1e-110">Type</span></span>   | <span data-ttu-id="9ea1e-111">説明</span><span class="sxs-lookup"><span data-stu-id="9ea1e-111">Description</span></span>                                                                                                                                                                      |
|:--------------|:-------|:---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| <span data-ttu-id="9ea1e-112">**type**</span><span class="sxs-lookup"><span data-stu-id="9ea1e-112">**type**</span></span>      | <span data-ttu-id="9ea1e-113">string</span><span class="sxs-lookup"><span data-stu-id="9ea1e-113">string</span></span> | <span data-ttu-id="9ea1e-p102">パッケージのタイプを指定する文字列です。`oneNote` が唯一の現在定義されている値であるとしても、他のパッケージ タイプが返されるものと考え、それぞれに応じた扱いをする必要があります。</span><span class="sxs-lookup"><span data-stu-id="9ea1e-p102">An string indicating the type of package. While `oneNote` is the only currently defined value, you should expect other package types to be returned and handle them accordingly.</span></span> |

## <a name="remarks"></a><span data-ttu-id="9ea1e-116">注釈</span><span class="sxs-lookup"><span data-stu-id="9ea1e-116">Remarks</span></span> 

<span data-ttu-id="9ea1e-117">DriveItem のファセットの詳細については、「[DriveItem](driveitem.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="9ea1e-117">For more information about the facets on a DriveItem, see [DriveItem](driveitem.md).</span></span>


<!--
{
  "type": "#page.annotation",
  "description": "The Package facet indicates that an item is the root of a special collection of items that should be treated as a single unit.",
  "keywords": "package, facet, onenote",
  "section": "documentation",
  "suppressions": []
}
-->
