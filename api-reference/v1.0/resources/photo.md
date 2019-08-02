---
author: JeremyKelley
ms.author: JeremyKelley
ms.date: 09/10/2017
title: 写真
localization_priority: Normal
description: 写真リソースは、EXIF メタデータなどの写真とカメラのプロパティを driveItem で提供します。
ms.prod: ''
doc_type: resourcePageType
ms.openlocfilehash: c86190768c10b04bb55f59104368089cf7c77b18
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "36035500"
---
# <a name="photo-resource-type"></a><span data-ttu-id="a3d68-103">写真リソースの種類</span><span class="sxs-lookup"><span data-stu-id="a3d68-103">Photo resource type</span></span>

<span data-ttu-id="a3d68-104">**写真**リソースは、EXIF メタデータなどの写真とカメラのプロパティを [driveItem](driveitem.md) で提供します。</span><span class="sxs-lookup"><span data-stu-id="a3d68-104">The **photo** resource provides photo and camera properties, for example, EXIF metadata, on a [driveItem](driveitem.md).</span></span>

## <a name="json-representation"></a><span data-ttu-id="a3d68-105">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="a3d68-105">JSON representation</span></span>

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

## <a name="properties"></a><span data-ttu-id="a3d68-106">プロパティ</span><span class="sxs-lookup"><span data-stu-id="a3d68-106">Properties</span></span>

| <span data-ttu-id="a3d68-107">プロパティ</span><span class="sxs-lookup"><span data-stu-id="a3d68-107">Property</span></span>                | <span data-ttu-id="a3d68-108">型</span><span class="sxs-lookup"><span data-stu-id="a3d68-108">Type</span></span>           | <span data-ttu-id="a3d68-109">説明</span><span class="sxs-lookup"><span data-stu-id="a3d68-109">Description</span></span>
|:------------------------|:---------------|:----------------------------------
| <span data-ttu-id="a3d68-110">**takenDateTime**</span><span class="sxs-lookup"><span data-stu-id="a3d68-110">**takenDateTime**</span></span>       | <span data-ttu-id="a3d68-111">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="a3d68-111">DateTimeOffset</span></span> | <span data-ttu-id="a3d68-p101">写真の撮影日時を表します。読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="a3d68-p101">Represents the date and time the photo was taken. Read-only.</span></span>
| <span data-ttu-id="a3d68-114">**cameraMake**</span><span class="sxs-lookup"><span data-stu-id="a3d68-114">**cameraMake**</span></span>          | <span data-ttu-id="a3d68-115">String</span><span class="sxs-lookup"><span data-stu-id="a3d68-115">String</span></span>         | <span data-ttu-id="a3d68-p102">カメラの製造元。読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="a3d68-p102">Camera manufacturer. Read-only.</span></span>
| <span data-ttu-id="a3d68-118">**cameraModel**</span><span class="sxs-lookup"><span data-stu-id="a3d68-118">**cameraModel**</span></span>         | <span data-ttu-id="a3d68-119">String</span><span class="sxs-lookup"><span data-stu-id="a3d68-119">String</span></span>         | <span data-ttu-id="a3d68-p103">カメラのモデル。読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="a3d68-p103">Camera model. Read-only.</span></span>
| <span data-ttu-id="a3d68-122">**fNumber**</span><span class="sxs-lookup"><span data-stu-id="a3d68-122">**fNumber**</span></span>             | <span data-ttu-id="a3d68-123">2 行分</span><span class="sxs-lookup"><span data-stu-id="a3d68-123">Double</span></span>         | <span data-ttu-id="a3d68-p104">カメラの絞り値。読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="a3d68-p104">The F-stop value from the camera. Read-only.</span></span>
| <span data-ttu-id="a3d68-126">**exposureDenominator**</span><span class="sxs-lookup"><span data-stu-id="a3d68-126">**exposureDenominator**</span></span> | <span data-ttu-id="a3d68-127">2 行分</span><span class="sxs-lookup"><span data-stu-id="a3d68-127">Double</span></span>         | <span data-ttu-id="a3d68-p105">カメラの露出時間の分数の分母。読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="a3d68-p105">The denominator for the exposure time fraction from the camera. Read-only.</span></span>
| <span data-ttu-id="a3d68-130">**exposureNumerator**</span><span class="sxs-lookup"><span data-stu-id="a3d68-130">**exposureNumerator**</span></span>   | <span data-ttu-id="a3d68-131">Double</span><span class="sxs-lookup"><span data-stu-id="a3d68-131">Double</span></span>         | <span data-ttu-id="a3d68-p106">カメラの露出時間の分数の分子。読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="a3d68-p106">The numerator for the exposure time fraction from the camera. Read-only.</span></span>
| <span data-ttu-id="a3d68-134">**focalLength**</span><span class="sxs-lookup"><span data-stu-id="a3d68-134">**focalLength**</span></span>         | <span data-ttu-id="a3d68-135">倍精度浮動小数点数</span><span class="sxs-lookup"><span data-stu-id="a3d68-135">Double</span></span>         | <span data-ttu-id="a3d68-p107">カメラの焦点距離。読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="a3d68-p107">The focal length from the camera. Read-only.</span></span>
| <span data-ttu-id="a3d68-138">**iso**</span><span class="sxs-lookup"><span data-stu-id="a3d68-138">**iso**</span></span>                 | <span data-ttu-id="a3d68-139">Int32</span><span class="sxs-lookup"><span data-stu-id="a3d68-139">Int32</span></span>          | <span data-ttu-id="a3d68-p108">カメラの ISO 値。読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="a3d68-p108">The ISO value from the camera. Read-only.</span></span>

## <a name="remarks"></a><span data-ttu-id="a3d68-142">注釈</span><span class="sxs-lookup"><span data-stu-id="a3d68-142">Remarks</span></span>

<span data-ttu-id="a3d68-143">OneDrive for Business と SharePoint は、**takenDateTime** プロパティのみを返します。</span><span class="sxs-lookup"><span data-stu-id="a3d68-143">OneDrive for Business and SharePoint only return the **takenDateTime** property.</span></span>

<span data-ttu-id="a3d68-144">DriveItem のファセットの詳細については、「[DriveItem](driveitem.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="a3d68-144">For more information about the facets on a DriveItem, see [DriveItem](driveitem.md).</span></span>
<!-- {
  "type": "#page.annotation",
  "description": "The photo facet provides details about the camera and settings on the camera for photos.",
  "keywords": "camera make,camera model, exposure, f-stop, iso",
  "section": "documentation",
  "tocPath": "Facets/Photo"
} -->
