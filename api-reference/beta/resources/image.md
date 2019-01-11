---
author: rgregg
ms.author: rgregg
ms.date: 09/10/2017
title: Image
localization_priority: Normal
ms.openlocfilehash: 2b5e084294c528a83f80b0c49badbf8f1e96ca41
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/11/2019
ms.locfileid: "27889727"
---
# <a name="image-resource-type"></a><span data-ttu-id="d81b7-102">イメージ リソースの種類</span><span class="sxs-lookup"><span data-stu-id="d81b7-102">Image resource type</span></span>

> <span data-ttu-id="d81b7-103">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="d81b7-103">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="d81b7-104">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="d81b7-104">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="d81b7-p102">**イメージ** リソースは、イメージ関連のプロパティを 1 つの構造にグループ化します。[**DriveItem**](driveitem.md) に null 以外の**イメージ** ファセットがある場合は、アイテムはビットマップ イメージを表します。</span><span class="sxs-lookup"><span data-stu-id="d81b7-p102">The **Image** resource groups image-related properties into a single structure. If a [**DriveItem**](driveitem.md) has a non-null **image** facet, the item represents a bitmap image.</span></span>

<span data-ttu-id="d81b7-107">**注:** サービスがイメージの幅と高さを決定できない場合は、**イメージ** リソースが空になる可能性があります。</span><span class="sxs-lookup"><span data-stu-id="d81b7-107">**Note:** If the service is unable to determine the width and height of the image, the **Image** resource may be empty.</span></span>

## <a name="json-representation"></a><span data-ttu-id="d81b7-108">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="d81b7-108">JSON representation</span></span>

<!-- { "blockType": "resource", "@odata.type": "microsoft.graph.image" } -->
```json
{
  "width": 100,
  "height": 200
}
```

## <a name="properties"></a><span data-ttu-id="d81b7-109">プロパティ</span><span class="sxs-lookup"><span data-stu-id="d81b7-109">Properties</span></span>

| <span data-ttu-id="d81b7-110">プロパティ</span><span class="sxs-lookup"><span data-stu-id="d81b7-110">Property</span></span>   | <span data-ttu-id="d81b7-111">種類</span><span class="sxs-lookup"><span data-stu-id="d81b7-111">Type</span></span>  | <span data-ttu-id="d81b7-112">説明</span><span class="sxs-lookup"><span data-stu-id="d81b7-112">Description</span></span>                                |
|:-----------|:------|:-------------------------------------------|
| <span data-ttu-id="d81b7-113">**height**</span><span class="sxs-lookup"><span data-stu-id="d81b7-113">**height**</span></span> | <span data-ttu-id="d81b7-114">Int32</span><span class="sxs-lookup"><span data-stu-id="d81b7-114">Int32</span></span> | <span data-ttu-id="d81b7-p103">省略可能。イメージの高さ (ピクセル単位)。読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="d81b7-p103">Optional. Height of the image, in pixels. Read-only.</span></span> |
| <span data-ttu-id="d81b7-118">**width**</span><span class="sxs-lookup"><span data-stu-id="d81b7-118">**width**</span></span>  | <span data-ttu-id="d81b7-119">Int32</span><span class="sxs-lookup"><span data-stu-id="d81b7-119">Int32</span></span> | <span data-ttu-id="d81b7-p104">省略可能。イメージの幅 (ピクセル単位)。読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="d81b7-p104">Optional. Width of the image, in pixels. Read-only.</span></span>  |

## <a name="remarks"></a><span data-ttu-id="d81b7-123">注釈</span><span class="sxs-lookup"><span data-stu-id="d81b7-123">Remarks</span></span>

<span data-ttu-id="d81b7-124">OneDrive for Business では、このリソースは、ファイル拡張子に基づいてイメージであると予期されるアイテムに対して返されます。</span><span class="sxs-lookup"><span data-stu-id="d81b7-124">In OneDrive for Business, this resource is returned on items that are expected to be images based on file extension.</span></span>

<span data-ttu-id="d81b7-125">DriveItem のファセットの詳細については、「[DriveItem](driveitem.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="d81b7-125">For more information about the facets on a DriveItem, see [DriveItem](driveitem.md).</span></span>


<!-- {
  "type": "#page.annotation",
  "description": "The image facet describes properties of an image like width and height",
  "keywords": "image,width,height,item,facet",
  "section": "documentation",
  "tocPath": "Facets/Image"
} -->
