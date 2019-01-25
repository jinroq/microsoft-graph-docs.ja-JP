---
author: rgregg
ms.author: rgregg
ms.date: 09/10/2017
title: Package
localization_priority: Normal
ms.openlocfilehash: 67e82faa3f51eeae71c2dcb22ecb7a973e2070bb
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/24/2019
ms.locfileid: "29516603"
---
# <a name="package-resource-type"></a><span data-ttu-id="1c663-102">Package リソースの種類</span><span class="sxs-lookup"><span data-stu-id="1c663-102">Package resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="1c663-103">**Package** リソースは、DriveItem が「パッケージ」内で最上位項目であること、または個別の項目ではなくコレクションとして扱うべき項目のコレクションであることを示します。</span><span class="sxs-lookup"><span data-stu-id="1c663-103">The **Package** resource indicates that a DriveItem is the top level item in a "package" or a collection of items that should be treated as a collection instead of individual items.</span></span>

<span data-ttu-id="1c663-p101">OneNote のノートブックはパッケージの一例です。ノートブックがその内容を表すファイルとフォルダーで構成されているのに対し、ノートブックを表す最上位アイテムは、これが特別な扱いを必要とするデータのコレクションであることをクライアントに示す **Package** ファセットを持ちます。</span><span class="sxs-lookup"><span data-stu-id="1c663-p101">An example of a package is a OneNote notebook. While the notebook is made up of files and folders that represent the contents of the notebook, the top level item that represents the notebook has a **package** facet to indicate to clients that this is a collection of data that should be treated special.</span></span>

<span data-ttu-id="1c663-106">**package** ファセットを持つ DriveItems は、**folder** や **file** ファセットを含みませんが、**folder** ファセットを持つ項目に概念的に類似しています。</span><span class="sxs-lookup"><span data-stu-id="1c663-106">DriveItems with the **package** facet do not include a **folder** or **file** facet but are conceptually similar to an item with a **folder** facet.</span></span>

## <a name="json-representation"></a><span data-ttu-id="1c663-107">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="1c663-107">JSON representation</span></span>

<!-- { "blockType": "resource", "@odata.type": "microsoft.graph.package" } -->
```json
{
  "type": "oneNote"
}
```

| <span data-ttu-id="1c663-108">プロパティ名</span><span class="sxs-lookup"><span data-stu-id="1c663-108">Property Name</span></span> | <span data-ttu-id="1c663-109">型</span><span class="sxs-lookup"><span data-stu-id="1c663-109">Type</span></span>   | <span data-ttu-id="1c663-110">説明</span><span class="sxs-lookup"><span data-stu-id="1c663-110">Description</span></span>                                                                                                                                                                      |
|:--------------|:-------|:---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| <span data-ttu-id="1c663-111">**type**</span><span class="sxs-lookup"><span data-stu-id="1c663-111">**type**</span></span>      | <span data-ttu-id="1c663-112">string</span><span class="sxs-lookup"><span data-stu-id="1c663-112">string</span></span> | <span data-ttu-id="1c663-p102">パッケージのタイプを指定する文字列です。`oneNote` が唯一の現在定義されている値であるとしても、他のパッケージ タイプが返されるものと考え、それぞれに応じた扱いをする必要があります。</span><span class="sxs-lookup"><span data-stu-id="1c663-p102">An string indicating the type of package. While `oneNote` is the only currently defined value, you should expect other package types to be returned and handle them accordingly.</span></span> |

## <a name="remarks"></a><span data-ttu-id="1c663-115">注釈</span><span class="sxs-lookup"><span data-stu-id="1c663-115">Remarks</span></span> 

<span data-ttu-id="1c663-116">DriveItem のファセットの詳細については、「[DriveItem](driveitem.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="1c663-116">For more information about the facets on a DriveItem, see [DriveItem](driveitem.md).</span></span>


<!--
{
  "type": "#page.annotation",
  "description": "The Package facet indicates that an item is the root of a special collection of items that should be treated as a single unit.",
  "keywords": "package, facet, onenote",
  "section": "documentation",
  "suppressions": [
    "Error: /api-reference/beta/resources/package.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
