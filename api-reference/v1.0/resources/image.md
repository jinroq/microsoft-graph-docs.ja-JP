---
author: rgregg
ms.author: rgregg
ms.date: 09/10/2017
title: Image
ms.openlocfilehash: 3652eeb71f6a73fe0089dafc9908cc8b3451aa34
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27023650"
---
# <a name="image-resource-type"></a><span data-ttu-id="6273b-102">イメージ リソースの種類</span><span class="sxs-lookup"><span data-stu-id="6273b-102">Image resource type</span></span>

<span data-ttu-id="6273b-p101">**イメージ** リソースは、イメージ関連のプロパティを 1 つの構造にグループ化します。[**DriveItem**](driveitem.md) に null 以外の**イメージ** ファセットがある場合は、アイテムはビットマップ イメージを表します。</span><span class="sxs-lookup"><span data-stu-id="6273b-p101">The **Image** resource groups image-related properties into a single structure. If a [**DriveItem**](driveitem.md) has a non-null **image** facet, the item represents a bitmap image.</span></span>

<span data-ttu-id="6273b-105">**注:** サービスがイメージの幅と高さを決定できない場合は、**イメージ** リソースが空になる可能性があります。</span><span class="sxs-lookup"><span data-stu-id="6273b-105">**Note:** If the service is unable to determine the width and height of the image, the **Image** resource may be empty.</span></span>

## <a name="json-representation"></a><span data-ttu-id="6273b-106">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="6273b-106">JSON representation</span></span>

<!-- { "blockType": "resource", "@odata.type": "microsoft.graph.image" } -->
```json
{
  "width": 100,
  "height": 200
}
```

## <a name="properties"></a><span data-ttu-id="6273b-107">プロパティ</span><span class="sxs-lookup"><span data-stu-id="6273b-107">Properties</span></span>

| <span data-ttu-id="6273b-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="6273b-108">Property</span></span>   | <span data-ttu-id="6273b-109">型</span><span class="sxs-lookup"><span data-stu-id="6273b-109">Type</span></span>  | <span data-ttu-id="6273b-110">説明</span><span class="sxs-lookup"><span data-stu-id="6273b-110">Description</span></span>                                |
|:-----------|:------|:-------------------------------------------|
| <span data-ttu-id="6273b-111">**height**</span><span class="sxs-lookup"><span data-stu-id="6273b-111">**height**</span></span> | <span data-ttu-id="6273b-112">Int32</span><span class="sxs-lookup"><span data-stu-id="6273b-112">Int32</span></span> | <span data-ttu-id="6273b-p102">省略可能。イメージの高さ (ピクセル単位)。読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="6273b-p102">Optional. Height of the image, in pixels. Read-only.</span></span> |
| <span data-ttu-id="6273b-116">**width**</span><span class="sxs-lookup"><span data-stu-id="6273b-116">**width**</span></span>  | <span data-ttu-id="6273b-117">Int32</span><span class="sxs-lookup"><span data-stu-id="6273b-117">Int32</span></span> | <span data-ttu-id="6273b-p103">省略可能。イメージの幅 (ピクセル単位)。読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="6273b-p103">Optional. Width of the image, in pixels. Read-only.</span></span>  |

## <a name="remarks"></a><span data-ttu-id="6273b-121">注釈</span><span class="sxs-lookup"><span data-stu-id="6273b-121">Remarks</span></span>

<span data-ttu-id="6273b-122">OneDrive for Business では、このリソースは、ファイル拡張子に基づいてイメージであると予期されるアイテムに対して返されます。</span><span class="sxs-lookup"><span data-stu-id="6273b-122">In OneDrive for Business, this resource is returned on items that are expected to be images based on file extension.</span></span>

<span data-ttu-id="6273b-123">DriveItem のファセットの詳細については、「[DriveItem](driveitem.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="6273b-123">For more information about the facets on a DriveItem, see [DriveItem](driveitem.md).</span></span>


<!-- {
  "type": "#page.annotation",
  "description": "The image facet describes properties of an image like width and height",
  "keywords": "image,width,height,item,facet",
  "section": "documentation",
  "tocPath": "Facets/Image"
} -->
