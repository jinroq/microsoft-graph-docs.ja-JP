---
author: rgregg
ms.author: rgregg
ms.date: 09/10/2017
title: Image
ms.openlocfilehash: 4488aedaf5c71f6484a0ccf33949fac2569d7af1
ms.sourcegitcommit: 7aea7a97e36e6d146214de3a90fdbc71628aadba
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 09/28/2017
---
# <a name="image-resource-type"></a><span data-ttu-id="373bf-102">Image リソース型</span><span class="sxs-lookup"><span data-stu-id="373bf-102">Image resource type</span></span>

<span data-ttu-id="373bf-p101">**イメージ** リソースは、イメージ関連のプロパティを 1 つの構造にグループ化します。[**DriveItem**](driveitem.md) に null 以外の**イメージ** ファセットがある場合は、アイテムはビットマップ イメージを表します。</span><span class="sxs-lookup"><span data-stu-id="373bf-p101">The **Image** resource groups image-related properties into a single structure. If a [**DriveItem**](driveitem.md) has a non-null **image** facet, the item represents a bitmap image.</span></span>

<span data-ttu-id="373bf-105">**注:**サービスがイメージの幅と高さを決定できない場合は、**イメージ** リソースが空になる可能性があります。</span><span class="sxs-lookup"><span data-stu-id="373bf-105">**Note:** If the service is unable to determine the width and height of the image, the **Image** resource may be empty.</span></span>

## <a name="json-representation"></a><span data-ttu-id="373bf-106">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="373bf-106">JSON representation</span></span>

<!-- { "blockType": "resource", "@odata.type": "microsoft.graph.image" } -->
```json
{
  "width": 100,
  "height": 200
}
```

## <a name="properties"></a><span data-ttu-id="373bf-107">プロパティ</span><span class="sxs-lookup"><span data-stu-id="373bf-107">Properties</span></span>

| <span data-ttu-id="373bf-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="373bf-108">Property</span></span>   | <span data-ttu-id="373bf-109">型</span><span class="sxs-lookup"><span data-stu-id="373bf-109">Type</span></span>  | <span data-ttu-id="373bf-110">説明</span><span class="sxs-lookup"><span data-stu-id="373bf-110">Description</span></span>                                |
|:-----------|:------|:-------------------------------------------|
| <span data-ttu-id="373bf-111">**height**</span><span class="sxs-lookup"><span data-stu-id="373bf-111">**height**</span></span> | <span data-ttu-id="373bf-112">Int32</span><span class="sxs-lookup"><span data-stu-id="373bf-112">Int32</span></span> | <span data-ttu-id="373bf-p102">省略可能。イメージの高さ (ピクセル単位)。読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="373bf-p102">Optional. Height of the image, in pixels. Read-only.</span></span> |
| <span data-ttu-id="373bf-116">**width**</span><span class="sxs-lookup"><span data-stu-id="373bf-116">**width**</span></span>  | <span data-ttu-id="373bf-117">Int32</span><span class="sxs-lookup"><span data-stu-id="373bf-117">Int32</span></span> | <span data-ttu-id="373bf-p103">省略可能。イメージの幅 (ピクセル単位)。読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="373bf-p103">Optional. Width of the image, in pixels. Read-only.</span></span>  |

## <a name="remarks"></a><span data-ttu-id="373bf-121">注釈</span><span class="sxs-lookup"><span data-stu-id="373bf-121">Remarks</span></span>

<span data-ttu-id="373bf-122">OneDrive for Business では、このリソースは、ファイル拡張子に基づいてイメージであると予期されるアイテム上に返されます。</span><span class="sxs-lookup"><span data-stu-id="373bf-122">In OneDrive for Business, this resource is returned on items that are expected to be images based on file extension. This resource returns no properties in OneDrive for Business.</span></span>

<span data-ttu-id="373bf-123">DriveItem のファセットの詳細については、「[DriveItem](driveitem.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="373bf-123">For more information about the facets on a DriveItem, see [DriveItem](driveitem.md).</span></span>


<!-- {
  "type": "#page.annotation",
  "description": "The image facet describes properties of an image like width and height",
  "keywords": "image,width,height,item,facet",
  "section": "documentation",
  "tocPath": "Facets/Image"
} -->
