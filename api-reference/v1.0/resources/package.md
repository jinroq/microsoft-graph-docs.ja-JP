---
author: rgregg
ms.author: rgregg
ms.date: 09/10/2017
title: パッケージ
ms.openlocfilehash: 12ae750a0f4fbe0e951554308d4041928c31a16d
ms.sourcegitcommit: abf4b739257e3ffd9d045f783ec595d846172590
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/21/2018
ms.locfileid: "23267543"
---
# <a name="package-resource-type"></a><span data-ttu-id="4f739-102">Package リソースの種類</span><span class="sxs-lookup"><span data-stu-id="4f739-102">Package resource type</span></span>

<span data-ttu-id="4f739-103">**Package** リソースは、DriveItem が「パッケージ」内で最上位項目であること、または個別の項目ではなくコレクションとして扱うべき項目のコレクションであることを示します。</span><span class="sxs-lookup"><span data-stu-id="4f739-103">The **Package** resource indicates that a DriveItem is the top level item in a "package" or a collection of items that should be treated as a collection instead of individual items.</span></span>

<span data-ttu-id="4f739-104">OneNote のノートブックはパッケージの一例です。</span><span class="sxs-lookup"><span data-stu-id="4f739-104">An example of a package is a OneNote notebook.</span></span> <span data-ttu-id="4f739-105">ノートブックがその内容を表すファイルとフォルダーで構成されているのに対し、ノートブックを表す最上位項目は、これが特別な扱いを必要とするデータのコレクションであることをクライアントに示す **package** ファセットを持ちます。</span><span class="sxs-lookup"><span data-stu-id="4f739-105">While the notebook is made up of files and folders that represent the contents of the notebook, the top level item that represents the notebook has a **package** facet to indicate to clients that this is a collection of data that should be treated special.</span></span>

<span data-ttu-id="4f739-106">**package** ファセットを持つ DriveItems は、**folder** や **file** ファセットを含みませんが、**folder** ファセットを持つ項目に概念的に類似しています。</span><span class="sxs-lookup"><span data-stu-id="4f739-106">DriveItems with the **package** facet do not include a **folder** or **file** facet but are conceptually similar to an item with a **folder** facet.</span></span>

## <a name="json-representation"></a><span data-ttu-id="4f739-107">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="4f739-107">JSON representation</span></span>

<!-- { "blockType": "resource", "@odata.type": "microsoft.graph.package" } -->
```json
{
  "type": "oneNote"
}
```

## <a name="properties"></a><span data-ttu-id="4f739-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="4f739-108">Properties</span></span>

| <span data-ttu-id="4f739-109">プロパティ名</span><span class="sxs-lookup"><span data-stu-id="4f739-109">Property Name</span></span> | <span data-ttu-id="4f739-110">型</span><span class="sxs-lookup"><span data-stu-id="4f739-110">Type</span></span>   | <span data-ttu-id="4f739-111">説明</span><span class="sxs-lookup"><span data-stu-id="4f739-111">Description</span></span>                                                                                                                                                                      |
|:--------------|:-------|:---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| <span data-ttu-id="4f739-112">型</span><span class="sxs-lookup"><span data-stu-id="4f739-112">type</span></span>          | <span data-ttu-id="4f739-113">文字列</span><span class="sxs-lookup"><span data-stu-id="4f739-113">string</span></span> | <span data-ttu-id="4f739-114">パッケージのタイプを示す文字列です。</span><span class="sxs-lookup"><span data-stu-id="4f739-114">A string indicating the type of package.</span></span> <span data-ttu-id="4f739-115">`oneNote` が現在唯一定義されている値であるとしても、他のパッケージ タイプが返されるものと考え、それに応じて対応する必要があります。</span><span class="sxs-lookup"><span data-stu-id="4f739-115">An string indicating the type of package. While `oneNote` is the only currently defined value, you should expect other package types to be returned and handle them accordingly.</span></span> |

## <a name="remarks"></a><span data-ttu-id="4f739-116">注釈</span><span class="sxs-lookup"><span data-stu-id="4f739-116">Remarks</span></span> 

<span data-ttu-id="4f739-117">DriveItem のファセットの詳細については、「[DriveItem](driveitem.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="4f739-117">For more information about the facets on a DriveItem, see [DriveItem](driveitem.md).</span></span>


<!-- {
  "type": "#page.annotation",
  "description": "The Package facet indicates that an item is the root of a special collection of items that should be treated as a single unit.",
  "keywords": "package, facet, onenote",
  "section": "documentation",
  "tocPath": "Facets/Package"
} -->
