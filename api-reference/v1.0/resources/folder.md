---
author: rgregg
ms.author: rgregg
ms.date: 09/10/2017
title: Folder
ms.openlocfilehash: 664597297700f7af096ef30cfbd5342a45a6c157
ms.sourcegitcommit: 7aea7a97e36e6d146214de3a90fdbc71628aadba
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 09/28/2017
---
# <a name="folder-resource-type"></a><span data-ttu-id="bc25a-102">Folder リソース型</span><span class="sxs-lookup"><span data-stu-id="bc25a-102">Folder resource type</span></span>

<span data-ttu-id="bc25a-103">**Folder** リソースは、アイテム上のフォルダー関連のデータを 1 つの構造にグループ化します。</span><span class="sxs-lookup"><span data-stu-id="bc25a-103">The **Folder** resource groups folder-related data on an item into a single structure. DriveItems with a non-null folder facet are containers for other DriveItems.</span></span> 
<span data-ttu-id="bc25a-104">null でない **folder** ファセットを持つ [**DriveItem**](driveitem.md) は、他の DriveItem のコンテナーです。</span><span class="sxs-lookup"><span data-stu-id="bc25a-104">The Folder resource groups folder-related data on an item into a single structure. [**DriveItems**](driveitem.md) with a non-null **folder** facet are containers for other DriveItems.</span></span>

## <a name="json-representation"></a><span data-ttu-id="bc25a-105">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="bc25a-105">JSON representation</span></span>

<span data-ttu-id="bc25a-106">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="bc25a-106">Here is a JSON representation of the resource.</span></span>

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

## <a name="properties"></a><span data-ttu-id="bc25a-107">プロパティ</span><span class="sxs-lookup"><span data-stu-id="bc25a-107">Properties</span></span>

| <span data-ttu-id="bc25a-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="bc25a-108">Property</span></span>       | <span data-ttu-id="bc25a-109">型</span><span class="sxs-lookup"><span data-stu-id="bc25a-109">Type</span></span>           | <span data-ttu-id="bc25a-110">説明</span><span class="sxs-lookup"><span data-stu-id="bc25a-110">Description</span></span>
|:---------------|:---------------|:-------------------------------------------
| <span data-ttu-id="bc25a-111">**childCount**</span><span class="sxs-lookup"><span data-stu-id="bc25a-111">**childCount**</span></span> | <span data-ttu-id="bc25a-112">Int64</span><span class="sxs-lookup"><span data-stu-id="bc25a-112">Int64</span></span>          | <span data-ttu-id="bc25a-113">このコンテナーの中に含まれる子の数。</span><span class="sxs-lookup"><span data-stu-id="bc25a-113">Number of children contained immediately within this container.</span></span>
| <span data-ttu-id="bc25a-114">**view**</span><span class="sxs-lookup"><span data-stu-id="bc25a-114">**view**</span></span>       | <span data-ttu-id="bc25a-115">[folderView][]</span><span class="sxs-lookup"><span data-stu-id="bc25a-115">[folderView facet][]</span></span> | <span data-ttu-id="bc25a-116">フォルダーに推奨されるビューを定義するプロパティのコレクション。</span><span class="sxs-lookup"><span data-stu-id="bc25a-116">A collection of properties defining the recommended view for the folder.</span></span>

## <a name="remarks"></a><span data-ttu-id="bc25a-117">備考</span><span class="sxs-lookup"><span data-stu-id="bc25a-117">Remarks</span></span> 

<span data-ttu-id="bc25a-118">DriveItem のファセットの詳細については、「[DriveItem][]」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="bc25a-118">For more information about the facets on a DriveItem, see [DriveItem][].</span></span>

[folderView]: folderView.md
[DriveItem]: driveItem.md

<!-- {
  "type": "#page.annotation",
  "description": "The Folder facet describes properties of a folder",
  "keywords": "folder,item,facet",
  "section": "documentation",
  "tocPath": "Facets/Folder"
} -->
