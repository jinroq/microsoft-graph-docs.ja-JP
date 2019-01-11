---
author: rgregg
ms.author: rgregg
ms.date: 09/10/2017
title: Package
localization_priority: Normal
ms.openlocfilehash: ab3d9298b0a03e31a9e33e9c187c1a0af8691cc3
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/11/2019
ms.locfileid: "27833944"
---
# <a name="package-resource-type"></a><span data-ttu-id="e65f7-102">Package リソースの種類</span><span class="sxs-lookup"><span data-stu-id="e65f7-102">Package resource type</span></span>

> <span data-ttu-id="e65f7-103">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="e65f7-103">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="e65f7-104">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="e65f7-104">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="e65f7-105">**Package** リソースは、DriveItem が「パッケージ」内で最上位項目であること、または個別の項目ではなくコレクションとして扱うべき項目のコレクションであることを示します。</span><span class="sxs-lookup"><span data-stu-id="e65f7-105">The **Package** resource indicates that a DriveItem is the top level item in a "package" or a collection of items that should be treated as a collection instead of individual items.</span></span>

<span data-ttu-id="e65f7-106">OneNote のノートブックはパッケージの一例です。</span><span class="sxs-lookup"><span data-stu-id="e65f7-106">An example of a package is a OneNote notebook.</span></span> <span data-ttu-id="e65f7-107">ノートブックがその内容を表すファイルとフォルダーで構成されているのに対し、ノートブックを表す最上位項目は、これが特別な扱いを必要とするデータのコレクションであることをクライアントに示す **package** ファセットを持ちます。</span><span class="sxs-lookup"><span data-stu-id="e65f7-107">While the notebook is made up of files and folders that represent the contents of the notebook, the top level item that represents the notebook has a **package** facet to indicate to clients that this is a collection of data that should be treated special.</span></span>

<span data-ttu-id="e65f7-108">**package** ファセットを持つ DriveItems は、**folder** や **file** ファセットを含みませんが、**folder** ファセットを持つ項目に概念的に類似しています。</span><span class="sxs-lookup"><span data-stu-id="e65f7-108">DriveItems with the **package** facet do not include a **folder** or **file** facet but are conceptually similar to an item with a **folder** facet.</span></span>

## <a name="json-representation"></a><span data-ttu-id="e65f7-109">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="e65f7-109">JSON representation</span></span>

<!-- { "blockType": "resource", "@odata.type": "microsoft.graph.package" } -->
```json
{
  "type": "oneNote"
}
```

| <span data-ttu-id="e65f7-110">プロパティ名</span><span class="sxs-lookup"><span data-stu-id="e65f7-110">Property Name</span></span> | <span data-ttu-id="e65f7-111">種類</span><span class="sxs-lookup"><span data-stu-id="e65f7-111">Type</span></span>   | <span data-ttu-id="e65f7-112">説明</span><span class="sxs-lookup"><span data-stu-id="e65f7-112">Description</span></span>                                                                                                                                                                      |
|:--------------|:-------|:---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| <span data-ttu-id="e65f7-113">**type**</span><span class="sxs-lookup"><span data-stu-id="e65f7-113">**type**</span></span>      | <span data-ttu-id="e65f7-114">string</span><span class="sxs-lookup"><span data-stu-id="e65f7-114">string</span></span> | <span data-ttu-id="e65f7-p103">パッケージのタイプを指定する文字列です。`oneNote` が唯一の現在定義されている値であるとしても、他のパッケージ タイプが返されるものと考え、それぞれに応じた扱いをする必要があります。</span><span class="sxs-lookup"><span data-stu-id="e65f7-p103">An string indicating the type of package. While `oneNote` is the only currently defined value, you should expect other package types to be returned and handle them accordingly.</span></span> |

## <a name="remarks"></a><span data-ttu-id="e65f7-117">注釈</span><span class="sxs-lookup"><span data-stu-id="e65f7-117">Remarks</span></span> 

<span data-ttu-id="e65f7-118">DriveItem のファセットの詳細については、「[DriveItem](driveitem.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="e65f7-118">For more information about the facets on a DriveItem, see [DriveItem](driveitem.md).</span></span>


<!-- {
  "type": "#page.annotation",
  "description": "The Package facet indicates that an item is the root of a special collection of items that should be treated as a single unit.",
  "keywords": "package, facet, onenote",
  "section": "documentation"
} -->
