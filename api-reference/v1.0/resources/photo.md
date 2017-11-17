---
author: rgregg
ms.author: rgregg
ms.date: 09/10/2017
title: Photo
ms.openlocfilehash: a4284caa7c20e266d87e22e9b3d729e17bc88abf
ms.sourcegitcommit: 7aea7a97e36e6d146214de3a90fdbc71628aadba
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 09/28/2017
---
# <a name="photo-resource-type"></a><span data-ttu-id="6edee-102">Photo リソース型</span><span class="sxs-lookup"><span data-stu-id="6edee-102">Photo resource type</span></span>

<span data-ttu-id="6edee-103">**写真**リソースは、EXIF メタデータなどの写真とカメラのプロパティを [driveItem](driveitem.md) で提供します。</span><span class="sxs-lookup"><span data-stu-id="6edee-103">The **photo** resource provides photo and camera properties, for example, EXIF metadata, on a [driveItem](driveitem.md).</span></span>

## <a name="json-representation"></a><span data-ttu-id="6edee-104">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="6edee-104">JSON representation</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [  ],
  "@odata.type": "microsoft.graph.photo"
}-->
```json
{
  "cameraMake": "string",
  "cameraModel": "string",
  "exposureDenominator": 1000.0,
  "exposureNumerator": 1.0,
  "fNumber": 1.8,
  "focalLength": 22.5,
  "iso": 100,
  "takenDateTime": "String (timestamp)"
}
```

## <a name="properties"></a><span data-ttu-id="6edee-105">プロパティ</span><span class="sxs-lookup"><span data-stu-id="6edee-105">Properties</span></span>

| <span data-ttu-id="6edee-106">プロパティ</span><span class="sxs-lookup"><span data-stu-id="6edee-106">Property</span></span>                | <span data-ttu-id="6edee-107">型</span><span class="sxs-lookup"><span data-stu-id="6edee-107">Type</span></span>           | <span data-ttu-id="6edee-108">説明</span><span class="sxs-lookup"><span data-stu-id="6edee-108">Description</span></span>
|:------------------------|:---------------|:----------------------------------
| <span data-ttu-id="6edee-109">**takenDateTime**</span><span class="sxs-lookup"><span data-stu-id="6edee-109">**takenDateTime**</span></span>       | <span data-ttu-id="6edee-110">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="6edee-110">DateTimeOffset</span></span> | <span data-ttu-id="6edee-p101">写真の撮影日時を表します。読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="6edee-p101">Represents the date and time the photo was taken. Read-only.</span></span>
| <span data-ttu-id="6edee-113">**cameraMake**</span><span class="sxs-lookup"><span data-stu-id="6edee-113">**cameraMake**</span></span>          | <span data-ttu-id="6edee-114">String</span><span class="sxs-lookup"><span data-stu-id="6edee-114">String</span></span>         | <span data-ttu-id="6edee-p102">カメラの製造元。読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="6edee-p102">Camera manufacturer. Read-only.</span></span>
| <span data-ttu-id="6edee-117">**cameraModel**</span><span class="sxs-lookup"><span data-stu-id="6edee-117">**cameraModel**</span></span>         | <span data-ttu-id="6edee-118">String</span><span class="sxs-lookup"><span data-stu-id="6edee-118">String</span></span>         | <span data-ttu-id="6edee-p103">カメラのモデル。読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="6edee-p103">Camera model. Read-only.</span></span>
| <span data-ttu-id="6edee-121">**fNumber**</span><span class="sxs-lookup"><span data-stu-id="6edee-121">**fNumber**</span></span>             | <span data-ttu-id="6edee-122">Double</span><span class="sxs-lookup"><span data-stu-id="6edee-122">Double</span></span>         | <span data-ttu-id="6edee-p104">カメラの絞り値。読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="6edee-p104">The F-stop value from the camera. Read-only.</span></span>
| <span data-ttu-id="6edee-125">**exposureDenominator**</span><span class="sxs-lookup"><span data-stu-id="6edee-125">**exposureDenominator**</span></span> | <span data-ttu-id="6edee-126">Double</span><span class="sxs-lookup"><span data-stu-id="6edee-126">Double</span></span>         | <span data-ttu-id="6edee-p105">カメラの露出時間の分数の分母。読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="6edee-p105">The denominator for the exposure time fraction from the camera. Read-only.</span></span>
| <span data-ttu-id="6edee-129">**exposureNumerator**</span><span class="sxs-lookup"><span data-stu-id="6edee-129">**exposureNumerator**</span></span>   | <span data-ttu-id="6edee-130">Double</span><span class="sxs-lookup"><span data-stu-id="6edee-130">Double</span></span>         | <span data-ttu-id="6edee-p106">カメラの露出時間の分数の分子。読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="6edee-p106">The numerator for the exposure time fraction from the camera. Read-only.</span></span>
| <span data-ttu-id="6edee-133">**focalLength**</span><span class="sxs-lookup"><span data-stu-id="6edee-133">**focalLength**</span></span>         | <span data-ttu-id="6edee-134">Double</span><span class="sxs-lookup"><span data-stu-id="6edee-134">Double</span></span>         | <span data-ttu-id="6edee-p107">カメラの焦点距離。読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="6edee-p107">The focal length from the camera. Read-only.</span></span>
| <span data-ttu-id="6edee-137">**iso**</span><span class="sxs-lookup"><span data-stu-id="6edee-137">**iso**</span></span>                 | <span data-ttu-id="6edee-138">Int64</span><span class="sxs-lookup"><span data-stu-id="6edee-138">Int64</span></span>          | <span data-ttu-id="6edee-p108">カメラの ISO 値。読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="6edee-p108">The ISO value from the camera. Read-only.</span></span>

## <a name="remarks"></a><span data-ttu-id="6edee-141">注釈</span><span class="sxs-lookup"><span data-stu-id="6edee-141">Remarks</span></span>
<span data-ttu-id="6edee-142">OneDrive for Business と SharePoint は、**takenDateTime** プロパティのみを返します。</span><span class="sxs-lookup"><span data-stu-id="6edee-142">OneDrive for Business and SharePoint only return the **takenDateTime** property.</span></span>

<span data-ttu-id="6edee-143">DriveItem のファセットの詳細については、「[DriveItem](driveitem.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="6edee-143">For more information about the facets on a DriveItem, see [DriveItem](driveitem.md).</span></span>
<!-- {
  "type": "#page.annotation",
  "description": "The photo facet provides details about the camera and settings on the camera for photos.",
  "keywords": "camera make,camera model, exposure, f-stop, iso",
  "section": "documentation",
  "tocPath": "Facets/Photo"
} -->
