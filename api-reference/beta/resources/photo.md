---
author: JeremyKelley
ms.author: JeremyKelley
ms.date: 09/10/2017
title: 写真
localization_priority: Normal
ms.openlocfilehash: f55236489d71c88f8d000b3462e64e82b8c08e56
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/26/2019
ms.locfileid: "33344909"
---
# <a name="photo-resource-type"></a><span data-ttu-id="f122e-102">写真リソースの種類</span><span class="sxs-lookup"><span data-stu-id="f122e-102">Photo resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="f122e-103">**写真**リソースは、EXIF メタデータなどの写真とカメラのプロパティを [driveItem](driveitem.md) で提供します。</span><span class="sxs-lookup"><span data-stu-id="f122e-103">The **photo** resource provides photo and camera properties, for example, EXIF metadata, on a [driveItem](driveitem.md).</span></span>

## <a name="json-representation"></a><span data-ttu-id="f122e-104">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="f122e-104">JSON representation</span></span>

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

## <a name="properties"></a><span data-ttu-id="f122e-105">プロパティ</span><span class="sxs-lookup"><span data-stu-id="f122e-105">Properties</span></span>

| <span data-ttu-id="f122e-106">プロパティ</span><span class="sxs-lookup"><span data-stu-id="f122e-106">Property</span></span>                | <span data-ttu-id="f122e-107">型</span><span class="sxs-lookup"><span data-stu-id="f122e-107">Type</span></span>           | <span data-ttu-id="f122e-108">説明</span><span class="sxs-lookup"><span data-stu-id="f122e-108">Description</span></span>
|:------------------------|:---------------|:----------------------------------
| <span data-ttu-id="f122e-109">**takenDateTime**</span><span class="sxs-lookup"><span data-stu-id="f122e-109">**takenDateTime**</span></span>       | <span data-ttu-id="f122e-110">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="f122e-110">DateTimeOffset</span></span> | <span data-ttu-id="f122e-p101">写真の撮影日時を表します。読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="f122e-p101">Represents the date and time the photo was taken. Read-only.</span></span>
| <span data-ttu-id="f122e-113">**cameraMake**</span><span class="sxs-lookup"><span data-stu-id="f122e-113">**cameraMake**</span></span>          | <span data-ttu-id="f122e-114">String</span><span class="sxs-lookup"><span data-stu-id="f122e-114">String</span></span>         | <span data-ttu-id="f122e-p102">カメラの製造元。読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="f122e-p102">Camera manufacturer. Read-only.</span></span>
| <span data-ttu-id="f122e-117">**cameraModel**</span><span class="sxs-lookup"><span data-stu-id="f122e-117">**cameraModel**</span></span>         | <span data-ttu-id="f122e-118">String</span><span class="sxs-lookup"><span data-stu-id="f122e-118">String</span></span>         | <span data-ttu-id="f122e-p103">カメラのモデル。読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="f122e-p103">Camera model. Read-only.</span></span>
| <span data-ttu-id="f122e-121">**fNumber**</span><span class="sxs-lookup"><span data-stu-id="f122e-121">**fNumber**</span></span>             | <span data-ttu-id="f122e-122">2 行分</span><span class="sxs-lookup"><span data-stu-id="f122e-122">Double</span></span>         | <span data-ttu-id="f122e-p104">カメラの絞り値。読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="f122e-p104">The F-stop value from the camera. Read-only.</span></span>
| <span data-ttu-id="f122e-125">**exposureDenominator**</span><span class="sxs-lookup"><span data-stu-id="f122e-125">**exposureDenominator**</span></span> | <span data-ttu-id="f122e-126">2 行分</span><span class="sxs-lookup"><span data-stu-id="f122e-126">Double</span></span>         | <span data-ttu-id="f122e-p105">カメラの露出時間の分数の分母。読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="f122e-p105">The denominator for the exposure time fraction from the camera. Read-only.</span></span>
| <span data-ttu-id="f122e-129">**exposureNumerator**</span><span class="sxs-lookup"><span data-stu-id="f122e-129">**exposureNumerator**</span></span>   | <span data-ttu-id="f122e-130">Double</span><span class="sxs-lookup"><span data-stu-id="f122e-130">Double</span></span>         | <span data-ttu-id="f122e-p106">カメラの露出時間の分数の分子。読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="f122e-p106">The numerator for the exposure time fraction from the camera. Read-only.</span></span>
| <span data-ttu-id="f122e-133">**focalLength**</span><span class="sxs-lookup"><span data-stu-id="f122e-133">**focalLength**</span></span>         | <span data-ttu-id="f122e-134">倍精度浮動小数点数</span><span class="sxs-lookup"><span data-stu-id="f122e-134">Double</span></span>         | <span data-ttu-id="f122e-p107">カメラの焦点距離。読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="f122e-p107">The focal length from the camera. Read-only.</span></span>
| <span data-ttu-id="f122e-137">**iso**</span><span class="sxs-lookup"><span data-stu-id="f122e-137">**iso**</span></span>                 | <span data-ttu-id="f122e-138">Int64</span><span class="sxs-lookup"><span data-stu-id="f122e-138">Int64</span></span>          | <span data-ttu-id="f122e-p108">カメラの ISO 値。読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="f122e-p108">The ISO value from the camera. Read-only.</span></span>

## <a name="remarks"></a><span data-ttu-id="f122e-141">注釈</span><span class="sxs-lookup"><span data-stu-id="f122e-141">Remarks</span></span>
<span data-ttu-id="f122e-142">OneDrive for Business と SharePoint は、**takenDateTime** プロパティのみを返します。</span><span class="sxs-lookup"><span data-stu-id="f122e-142">OneDrive for Business and SharePoint only return the **takenDateTime** property.</span></span>

<span data-ttu-id="f122e-143">DriveItem のファセットの詳細については、「[DriveItem](driveitem.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="f122e-143">For more information about the facets on a DriveItem, see [DriveItem](driveitem.md).</span></span>
<!--
{
  "type": "#page.annotation",
  "description": "The photo facet provides details about the camera and settings on the camera for photos.",
  "keywords": "camera make,camera model, exposure, f-stop, iso",
  "section": "documentation",
  "tocPath": "Facets/Photo",
  "suppressions": []
}
-->
