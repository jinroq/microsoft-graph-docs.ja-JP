---
author: JeremyKelley
ms.author: JeremyKelley
ms.date: 09/10/2017
title: パッケージ
localization_priority: Normal
ms.openlocfilehash: c64dfce910456ef9b9415e3332c099d7814a71f2
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32462530"
---
# <a name="package-resource-type"></a><span data-ttu-id="4c4e1-102">Package リソースの種類</span><span class="sxs-lookup"><span data-stu-id="4c4e1-102">Package resource type</span></span>

<span data-ttu-id="4c4e1-103">**Package** リソースは、DriveItem が「パッケージ」内で最上位項目であること、または個別の項目ではなくコレクションとして扱うべき項目のコレクションであることを示します。</span><span class="sxs-lookup"><span data-stu-id="4c4e1-103">The **Package** resource indicates that a DriveItem is the top level item in a "package" or a collection of items that should be treated as a collection instead of individual items.</span></span>

<span data-ttu-id="4c4e1-p101">OneNote のノートブックはパッケージの一例です。ノートブックがその内容を表すファイルとフォルダーで構成されているのに対し、ノートブックを表す最上位項目は、これが特別な扱いを必要とするデータのコレクションであることをクライアントに示す **package** ファセットを持ちます。</span><span class="sxs-lookup"><span data-stu-id="4c4e1-p101">An example of a package is a OneNote notebook. While the notebook is made up of files and folders that represent the contents of the notebook, the top level item that represents the notebook has a **package** facet to indicate to clients that this is a collection of data that should be treated special.</span></span>

<span data-ttu-id="4c4e1-106">**package** ファセットを持つ DriveItems は、**folder** や **file** ファセットを含みませんが、**folder** ファセットを持つ項目に概念的に類似しています。</span><span class="sxs-lookup"><span data-stu-id="4c4e1-106">DriveItems with the **package** facet do not include a **folder** or **file** facet but are conceptually similar to an item with a **folder** facet.</span></span>

## <a name="json-representation"></a><span data-ttu-id="4c4e1-107">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="4c4e1-107">JSON representation</span></span>

<!-- { "blockType": "resource", "@odata.type": "microsoft.graph.package" } -->
```json
{
  "type": "oneNote"
}
```

## <a name="properties"></a><span data-ttu-id="4c4e1-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="4c4e1-108">Properties</span></span>

| <span data-ttu-id="4c4e1-109">プロパティ名</span><span class="sxs-lookup"><span data-stu-id="4c4e1-109">Property Name</span></span> | <span data-ttu-id="4c4e1-110">型</span><span class="sxs-lookup"><span data-stu-id="4c4e1-110">Type</span></span>   | <span data-ttu-id="4c4e1-111">説明</span><span class="sxs-lookup"><span data-stu-id="4c4e1-111">Description</span></span>                                                                                                                                                                      |
|:--------------|:-------|:---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| <span data-ttu-id="4c4e1-112">type</span><span class="sxs-lookup"><span data-stu-id="4c4e1-112">type</span></span>          | <span data-ttu-id="4c4e1-113">string</span><span class="sxs-lookup"><span data-stu-id="4c4e1-113">string</span></span> | <span data-ttu-id="4c4e1-114">パッケージの種類を示す文字列。</span><span class="sxs-lookup"><span data-stu-id="4c4e1-114">A string indicating the type of package.</span></span> <span data-ttu-id="4c4e1-115">が唯一の現在定義されている値であるとしても、他のパッケージ タイプが返されるものと考え、それぞれに応じた扱いをする必要があります。</span><span class="sxs-lookup"><span data-stu-id="4c4e1-115">While `oneNote` is the only currently defined value, you should expect other package types to be returned and handle them accordingly.</span></span> |

## <a name="remarks"></a><span data-ttu-id="4c4e1-116">注釈</span><span class="sxs-lookup"><span data-stu-id="4c4e1-116">Remarks</span></span> 

<span data-ttu-id="4c4e1-117">DriveItem のファセットの詳細については、「[DriveItem](driveitem.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="4c4e1-117">For more information about the facets on a DriveItem, see [DriveItem](driveitem.md).</span></span>


<!-- {
  "type": "#page.annotation",
  "description": "The Package facet indicates that an item is the root of a special collection of items that should be treated as a single unit.",
  "keywords": "package, facet, onenote",
  "section": "documentation",
  "tocPath": "Facets/Package"
} -->
