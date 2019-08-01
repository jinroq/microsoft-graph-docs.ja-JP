---
author: JeremyKelley
ms.author: JeremyKelley
ms.date: 09/10/2017
title: イメージ
localization_priority: Normal
description: イメージリソースは、画像関連のプロパティを1つの構造体にグループ化します。
ms.prod: ''
doc_type: resourcePageType
ms.openlocfilehash: d8b9f871ed465f3f6f617638a8dba38d575509a1
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "36032404"
---
# <a name="image-resource-type"></a><span data-ttu-id="96c43-103">イメージ リソースの種類</span><span class="sxs-lookup"><span data-stu-id="96c43-103">Image resource type</span></span>

<span data-ttu-id="96c43-p101">**イメージ** リソースは、イメージ関連のプロパティを 1 つの構造にグループ化します。[**DriveItem**](driveitem.md) に null 以外の**イメージ** ファセットがある場合は、アイテムはビットマップ イメージを表します。</span><span class="sxs-lookup"><span data-stu-id="96c43-p101">The **Image** resource groups image-related properties into a single structure. If a [**DriveItem**](driveitem.md) has a non-null **image** facet, the item represents a bitmap image.</span></span>

<span data-ttu-id="96c43-106">**注:** サービスがイメージの幅と高さを決定できない場合は、**イメージ** リソースが空になる可能性があります。</span><span class="sxs-lookup"><span data-stu-id="96c43-106">**Note:** If the service is unable to determine the width and height of the image, the **Image** resource may be empty.</span></span>

## <a name="json-representation"></a><span data-ttu-id="96c43-107">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="96c43-107">JSON representation</span></span>

<!-- { "blockType": "resource", "@odata.type": "microsoft.graph.image" } -->
```json
{
  "width": 100,
  "height": 200
}
```

## <a name="properties"></a><span data-ttu-id="96c43-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="96c43-108">Properties</span></span>

| <span data-ttu-id="96c43-109">プロパティ</span><span class="sxs-lookup"><span data-stu-id="96c43-109">Property</span></span>   | <span data-ttu-id="96c43-110">型</span><span class="sxs-lookup"><span data-stu-id="96c43-110">Type</span></span>  | <span data-ttu-id="96c43-111">説明</span><span class="sxs-lookup"><span data-stu-id="96c43-111">Description</span></span>                                |
|:-----------|:------|:-------------------------------------------|
| <span data-ttu-id="96c43-112">**height**</span><span class="sxs-lookup"><span data-stu-id="96c43-112">**height**</span></span> | <span data-ttu-id="96c43-113">Int32</span><span class="sxs-lookup"><span data-stu-id="96c43-113">Int32</span></span> | <span data-ttu-id="96c43-p102">省略可能。イメージの高さ (ピクセル単位)。読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="96c43-p102">Optional. Height of the image, in pixels. Read-only.</span></span> |
| <span data-ttu-id="96c43-117">**width**</span><span class="sxs-lookup"><span data-stu-id="96c43-117">**width**</span></span>  | <span data-ttu-id="96c43-118">Int32</span><span class="sxs-lookup"><span data-stu-id="96c43-118">Int32</span></span> | <span data-ttu-id="96c43-p103">省略可能。イメージの幅 (ピクセル単位)。読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="96c43-p103">Optional. Width of the image, in pixels. Read-only.</span></span>  |

## <a name="remarks"></a><span data-ttu-id="96c43-122">注釈</span><span class="sxs-lookup"><span data-stu-id="96c43-122">Remarks</span></span>

<span data-ttu-id="96c43-123">OneDrive for Business では、このリソースは、ファイル拡張子に基づいてイメージであると予期されるアイテムに対して返されます。</span><span class="sxs-lookup"><span data-stu-id="96c43-123">In OneDrive for Business, this resource is returned on items that are expected to be images based on file extension.</span></span>

<span data-ttu-id="96c43-124">DriveItem のファセットの詳細については、「[DriveItem](driveitem.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="96c43-124">For more information about the facets on a DriveItem, see [DriveItem](driveitem.md).</span></span>


<!-- {
  "type": "#page.annotation",
  "description": "The image facet describes properties of an image like width and height",
  "keywords": "image,width,height,item,facet",
  "section": "documentation",
  "tocPath": "Facets/Image"
} -->
