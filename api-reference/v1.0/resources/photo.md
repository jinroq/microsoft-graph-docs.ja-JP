---
author: rgregg
ms.author: rgregg
ms.date: 09/10/2017
title: Photo
ms.openlocfilehash: 391eafd84ab1abd4670c953720ff7097e060bfd3
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27023495"
---
# <a name="photo-resource-type"></a><span data-ttu-id="a6ced-102">写真リソースの種類</span><span class="sxs-lookup"><span data-stu-id="a6ced-102">Photo resource type</span></span>

<span data-ttu-id="a6ced-103">**写真**リソースは、EXIF メタデータなどの写真とカメラのプロパティを [driveItem](driveitem.md) で提供します。</span><span class="sxs-lookup"><span data-stu-id="a6ced-103">The **photo** resource provides photo and camera properties, for example, EXIF metadata, on a [driveItem](driveitem.md).</span></span>

## <a name="json-representation"></a><span data-ttu-id="a6ced-104">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="a6ced-104">JSON representation</span></span>

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

## <a name="properties"></a><span data-ttu-id="a6ced-105">プロパティ</span><span class="sxs-lookup"><span data-stu-id="a6ced-105">Properties</span></span>

| <span data-ttu-id="a6ced-106">プロパティ</span><span class="sxs-lookup"><span data-stu-id="a6ced-106">Property</span></span>                | <span data-ttu-id="a6ced-107">型</span><span class="sxs-lookup"><span data-stu-id="a6ced-107">Type</span></span>           | <span data-ttu-id="a6ced-108">説明</span><span class="sxs-lookup"><span data-stu-id="a6ced-108">Description</span></span>
|:------------------------|:---------------|:----------------------------------
| <span data-ttu-id="a6ced-109">**takenDateTime**</span><span class="sxs-lookup"><span data-stu-id="a6ced-109">**takenDateTime**</span></span>       | <span data-ttu-id="a6ced-110">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="a6ced-110">DateTimeOffset</span></span> | <span data-ttu-id="a6ced-p101">写真の撮影日時を表します。読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="a6ced-p101">Represents the date and time the photo was taken. Read-only.</span></span>
| <span data-ttu-id="a6ced-113">**cameraMake**</span><span class="sxs-lookup"><span data-stu-id="a6ced-113">**cameraMake**</span></span>          | <span data-ttu-id="a6ced-114">String</span><span class="sxs-lookup"><span data-stu-id="a6ced-114">String</span></span>         | <span data-ttu-id="a6ced-p102">カメラの製造元。読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="a6ced-p102">Camera manufacturer. Read-only.</span></span>
| <span data-ttu-id="a6ced-117">**cameraModel**</span><span class="sxs-lookup"><span data-stu-id="a6ced-117">**cameraModel**</span></span>         | <span data-ttu-id="a6ced-118">String</span><span class="sxs-lookup"><span data-stu-id="a6ced-118">String</span></span>         | <span data-ttu-id="a6ced-p103">カメラのモデル。読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="a6ced-p103">Camera model. Read-only.</span></span>
| <span data-ttu-id="a6ced-121">**fNumber**</span><span class="sxs-lookup"><span data-stu-id="a6ced-121">**fNumber**</span></span>             | <span data-ttu-id="a6ced-122">Double</span><span class="sxs-lookup"><span data-stu-id="a6ced-122">Double</span></span>         | <span data-ttu-id="a6ced-p104">カメラの絞り値。読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="a6ced-p104">The F-stop value from the camera. Read-only.</span></span>
| <span data-ttu-id="a6ced-125">**exposureDenominator**</span><span class="sxs-lookup"><span data-stu-id="a6ced-125">**exposureDenominator**</span></span> | <span data-ttu-id="a6ced-126">Double</span><span class="sxs-lookup"><span data-stu-id="a6ced-126">Double</span></span>         | <span data-ttu-id="a6ced-p105">カメラの露出時間の分数の分母。読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="a6ced-p105">The denominator for the exposure time fraction from the camera. Read-only.</span></span>
| <span data-ttu-id="a6ced-129">**exposureNumerator**</span><span class="sxs-lookup"><span data-stu-id="a6ced-129">**exposureNumerator**</span></span>   | <span data-ttu-id="a6ced-130">Double</span><span class="sxs-lookup"><span data-stu-id="a6ced-130">Double</span></span>         | <span data-ttu-id="a6ced-p106">カメラの露出時間の分数の分子。読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="a6ced-p106">The numerator for the exposure time fraction from the camera. Read-only.</span></span>
| <span data-ttu-id="a6ced-133">**focalLength**</span><span class="sxs-lookup"><span data-stu-id="a6ced-133">**focalLength**</span></span>         | <span data-ttu-id="a6ced-134">Double</span><span class="sxs-lookup"><span data-stu-id="a6ced-134">Double</span></span>         | <span data-ttu-id="a6ced-p107">カメラの焦点距離。読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="a6ced-p107">The focal length from the camera. Read-only.</span></span>
| <span data-ttu-id="a6ced-137">**iso**</span><span class="sxs-lookup"><span data-stu-id="a6ced-137">**iso**</span></span>                 | <span data-ttu-id="a6ced-138">Int32</span><span class="sxs-lookup"><span data-stu-id="a6ced-138">Int32</span></span>          | <span data-ttu-id="a6ced-p108">カメラの ISO 値。読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="a6ced-p108">The ISO value from the camera. Read-only.</span></span>

## <a name="remarks"></a><span data-ttu-id="a6ced-141">注釈</span><span class="sxs-lookup"><span data-stu-id="a6ced-141">Remarks</span></span>

<span data-ttu-id="a6ced-142">OneDrive for Business と SharePoint は、**takenDateTime** プロパティのみを返します。</span><span class="sxs-lookup"><span data-stu-id="a6ced-142">OneDrive for Business and SharePoint only return the **takenDateTime** property.</span></span>

<span data-ttu-id="a6ced-143">DriveItem のファセットの詳細については、「[DriveItem](driveitem.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="a6ced-143">For more information about the facets on a DriveItem, see [DriveItem](driveitem.md).</span></span>
<!-- {
  "type": "#page.annotation",
  "description": "The photo facet provides details about the camera and settings on the camera for photos.",
  "keywords": "camera make,camera model, exposure, f-stop, iso",
  "section": "documentation",
  "tocPath": "Facets/Photo"
} -->
