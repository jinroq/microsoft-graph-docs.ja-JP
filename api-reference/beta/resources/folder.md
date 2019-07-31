---
author: JeremyKelley
description: 'Folder リソースは、アイテム上のフォルダー関連のデータを 1 つの構造にグループ化します。 '
ms.date: 09/10/2017
title: フォルダー
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
ms.openlocfilehash: f9cbbba6ae20c56800a5f6f492319f47b7d8017c
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "35971992"
---
# <a name="folder-resource-type"></a><span data-ttu-id="fa14e-103">Folder リソース型</span><span class="sxs-lookup"><span data-stu-id="fa14e-103">Folder resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="fa14e-p101">**フォルダー**リソースは、アイテム上のフォルダー関連のデータを 1 つの構造にグループ化します。**フォルダー**ファセットが null 以外の **[DriveItems](driveitem.md)** は、他の DriveItems のコンテナーです。</span><span class="sxs-lookup"><span data-stu-id="fa14e-p101">The **Folder** resource groups folder-related data on an item into a single structure. [**DriveItems**](driveitem.md) with a non-null **folder** facet are containers for other DriveItems.</span></span>

## <a name="json-representation"></a><span data-ttu-id="fa14e-106">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="fa14e-106">JSON representation</span></span>

<span data-ttu-id="fa14e-107">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="fa14e-107">Here is a JSON representation of the resource.</span></span>

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

## <a name="properties"></a><span data-ttu-id="fa14e-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="fa14e-108">Properties</span></span>

| <span data-ttu-id="fa14e-109">プロパティ</span><span class="sxs-lookup"><span data-stu-id="fa14e-109">Property</span></span>       | <span data-ttu-id="fa14e-110">型</span><span class="sxs-lookup"><span data-stu-id="fa14e-110">Type</span></span>           | <span data-ttu-id="fa14e-111">説明</span><span class="sxs-lookup"><span data-stu-id="fa14e-111">Description</span></span>
|:---------------|:---------------|:-------------------------------------------
| <span data-ttu-id="fa14e-112">**childCount**</span><span class="sxs-lookup"><span data-stu-id="fa14e-112">**childCount**</span></span> | <span data-ttu-id="fa14e-113">Int64</span><span class="sxs-lookup"><span data-stu-id="fa14e-113">Int64</span></span>          | <span data-ttu-id="fa14e-114">このコンテナーの中に含まれる子の数。</span><span class="sxs-lookup"><span data-stu-id="fa14e-114">Number of children contained immediately within this container.</span></span>
| <span data-ttu-id="fa14e-115">**view**</span><span class="sxs-lookup"><span data-stu-id="fa14e-115">**view**</span></span>       | <span data-ttu-id="fa14e-116">[folderView][]</span><span class="sxs-lookup"><span data-stu-id="fa14e-116">[folderView][]</span></span> | <span data-ttu-id="fa14e-117">フォルダーに推奨されるビューを定義するプロパティのコレクション。</span><span class="sxs-lookup"><span data-stu-id="fa14e-117">A collection of properties defining the recommended view for the folder.</span></span>


## <a name="remarks"></a><span data-ttu-id="fa14e-118">備考</span><span class="sxs-lookup"><span data-stu-id="fa14e-118">Remarks</span></span> 

<span data-ttu-id="fa14e-119">DriveItem のファセットの詳細については、「[DriveItem][]」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="fa14e-119">For more information about the facets on a DriveItem, see [DriveItem][].</span></span>

[folderView]: folderview.md
[DriveItem]: driveitem.md

<!--
{
  "type": "#page.annotation",
  "description": "folder resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
