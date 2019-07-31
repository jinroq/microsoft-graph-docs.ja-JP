---
author: JeremyKelley
description: 写真リソースは、EXIF メタデータなどの写真とカメラのプロパティを driveItem で提供します。
ms.date: 09/10/2017
title: 写真
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
ms.openlocfilehash: 6713e66b5ca14cfa6605b9e67d4bec152a321f33
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "36009224"
---
# <a name="photo-resource-type"></a><span data-ttu-id="ec902-103">写真リソースの種類</span><span class="sxs-lookup"><span data-stu-id="ec902-103">Photo resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="ec902-104">**写真**リソースは、EXIF メタデータなどの写真とカメラのプロパティを [driveItem](driveitem.md) で提供します。</span><span class="sxs-lookup"><span data-stu-id="ec902-104">The **photo** resource provides photo and camera properties, for example, EXIF metadata, on a [driveItem](driveitem.md).</span></span>

## <a name="json-representation"></a><span data-ttu-id="ec902-105">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="ec902-105">JSON representation</span></span>

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

## <a name="properties"></a><span data-ttu-id="ec902-106">プロパティ</span><span class="sxs-lookup"><span data-stu-id="ec902-106">Properties</span></span>

| <span data-ttu-id="ec902-107">プロパティ</span><span class="sxs-lookup"><span data-stu-id="ec902-107">Property</span></span>                | <span data-ttu-id="ec902-108">型</span><span class="sxs-lookup"><span data-stu-id="ec902-108">Type</span></span>           | <span data-ttu-id="ec902-109">説明</span><span class="sxs-lookup"><span data-stu-id="ec902-109">Description</span></span>
|:------------------------|:---------------|:----------------------------------
| <span data-ttu-id="ec902-110">**takenDateTime**</span><span class="sxs-lookup"><span data-stu-id="ec902-110">**takenDateTime**</span></span>       | <span data-ttu-id="ec902-111">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="ec902-111">DateTimeOffset</span></span> | <span data-ttu-id="ec902-p101">写真の撮影日時を表します。読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="ec902-p101">Represents the date and time the photo was taken. Read-only.</span></span>
| <span data-ttu-id="ec902-114">**cameraMake**</span><span class="sxs-lookup"><span data-stu-id="ec902-114">**cameraMake**</span></span>          | <span data-ttu-id="ec902-115">String</span><span class="sxs-lookup"><span data-stu-id="ec902-115">String</span></span>         | <span data-ttu-id="ec902-p102">カメラの製造元。読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="ec902-p102">Camera manufacturer. Read-only.</span></span>
| <span data-ttu-id="ec902-118">**cameraModel**</span><span class="sxs-lookup"><span data-stu-id="ec902-118">**cameraModel**</span></span>         | <span data-ttu-id="ec902-119">String</span><span class="sxs-lookup"><span data-stu-id="ec902-119">String</span></span>         | <span data-ttu-id="ec902-p103">カメラのモデル。読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="ec902-p103">Camera model. Read-only.</span></span>
| <span data-ttu-id="ec902-122">**fNumber**</span><span class="sxs-lookup"><span data-stu-id="ec902-122">**fNumber**</span></span>             | <span data-ttu-id="ec902-123">2 行分</span><span class="sxs-lookup"><span data-stu-id="ec902-123">Double</span></span>         | <span data-ttu-id="ec902-p104">カメラの絞り値。読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="ec902-p104">The F-stop value from the camera. Read-only.</span></span>
| <span data-ttu-id="ec902-126">**exposureDenominator**</span><span class="sxs-lookup"><span data-stu-id="ec902-126">**exposureDenominator**</span></span> | <span data-ttu-id="ec902-127">2 行分</span><span class="sxs-lookup"><span data-stu-id="ec902-127">Double</span></span>         | <span data-ttu-id="ec902-p105">カメラの露出時間の分数の分母。読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="ec902-p105">The denominator for the exposure time fraction from the camera. Read-only.</span></span>
| <span data-ttu-id="ec902-130">**exposureNumerator**</span><span class="sxs-lookup"><span data-stu-id="ec902-130">**exposureNumerator**</span></span>   | <span data-ttu-id="ec902-131">Double</span><span class="sxs-lookup"><span data-stu-id="ec902-131">Double</span></span>         | <span data-ttu-id="ec902-p106">カメラの露出時間の分数の分子。読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="ec902-p106">The numerator for the exposure time fraction from the camera. Read-only.</span></span>
| <span data-ttu-id="ec902-134">**focalLength**</span><span class="sxs-lookup"><span data-stu-id="ec902-134">**focalLength**</span></span>         | <span data-ttu-id="ec902-135">倍精度浮動小数点数</span><span class="sxs-lookup"><span data-stu-id="ec902-135">Double</span></span>         | <span data-ttu-id="ec902-p107">カメラの焦点距離。読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="ec902-p107">The focal length from the camera. Read-only.</span></span>
| <span data-ttu-id="ec902-138">**iso**</span><span class="sxs-lookup"><span data-stu-id="ec902-138">**iso**</span></span>                 | <span data-ttu-id="ec902-139">Int64</span><span class="sxs-lookup"><span data-stu-id="ec902-139">Int64</span></span>          | <span data-ttu-id="ec902-p108">カメラの ISO 値。読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="ec902-p108">The ISO value from the camera. Read-only.</span></span>

## <a name="remarks"></a><span data-ttu-id="ec902-142">注釈</span><span class="sxs-lookup"><span data-stu-id="ec902-142">Remarks</span></span>
<span data-ttu-id="ec902-143">OneDrive for Business と SharePoint は、**takenDateTime** プロパティのみを返します。</span><span class="sxs-lookup"><span data-stu-id="ec902-143">OneDrive for Business and SharePoint only return the **takenDateTime** property.</span></span>

<span data-ttu-id="ec902-144">DriveItem のファセットの詳細については、「[DriveItem](driveitem.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="ec902-144">For more information about the facets on a DriveItem, see [DriveItem](driveitem.md).</span></span>
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
