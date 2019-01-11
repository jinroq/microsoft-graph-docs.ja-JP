---
author: rgregg
ms.author: rgregg
ms.date: 09/10/2017
title: Photo
localization_priority: Normal
ms.openlocfilehash: ed891f917ba8018aac349976df0455adfd269fdb
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/11/2019
ms.locfileid: "27869385"
---
# <a name="photo-resource-type"></a><span data-ttu-id="18c1b-102">写真リソースの種類</span><span class="sxs-lookup"><span data-stu-id="18c1b-102">Photo resource type</span></span>

> <span data-ttu-id="18c1b-103">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="18c1b-103">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="18c1b-104">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="18c1b-104">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="18c1b-105">**写真**リソースは、EXIF メタデータなどの写真とカメラのプロパティを [driveItem](driveitem.md) で提供します。</span><span class="sxs-lookup"><span data-stu-id="18c1b-105">The **photo** resource provides photo and camera properties, for example, EXIF metadata, on a [driveItem](driveitem.md).</span></span>

## <a name="json-representation"></a><span data-ttu-id="18c1b-106">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="18c1b-106">JSON representation</span></span>

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

## <a name="properties"></a><span data-ttu-id="18c1b-107">プロパティ</span><span class="sxs-lookup"><span data-stu-id="18c1b-107">Properties</span></span>

| <span data-ttu-id="18c1b-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="18c1b-108">Property</span></span>                | <span data-ttu-id="18c1b-109">種類</span><span class="sxs-lookup"><span data-stu-id="18c1b-109">Type</span></span>           | <span data-ttu-id="18c1b-110">説明</span><span class="sxs-lookup"><span data-stu-id="18c1b-110">Description</span></span>
|:------------------------|:---------------|:----------------------------------
| <span data-ttu-id="18c1b-111">**takenDateTime**</span><span class="sxs-lookup"><span data-stu-id="18c1b-111">**takenDateTime**</span></span>       | <span data-ttu-id="18c1b-112">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="18c1b-112">DateTimeOffset</span></span> | <span data-ttu-id="18c1b-p102">写真の撮影日時を表します。読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="18c1b-p102">Represents the date and time the photo was taken. Read-only.</span></span>
| <span data-ttu-id="18c1b-115">**cameraMake**</span><span class="sxs-lookup"><span data-stu-id="18c1b-115">**cameraMake**</span></span>          | <span data-ttu-id="18c1b-116">String</span><span class="sxs-lookup"><span data-stu-id="18c1b-116">String</span></span>         | <span data-ttu-id="18c1b-p103">カメラの製造元。読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="18c1b-p103">Camera manufacturer. Read-only.</span></span>
| <span data-ttu-id="18c1b-119">**cameraModel**</span><span class="sxs-lookup"><span data-stu-id="18c1b-119">**cameraModel**</span></span>         | <span data-ttu-id="18c1b-120">String</span><span class="sxs-lookup"><span data-stu-id="18c1b-120">String</span></span>         | <span data-ttu-id="18c1b-p104">カメラのモデル。読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="18c1b-p104">Camera model. Read-only.</span></span>
| <span data-ttu-id="18c1b-123">**fNumber**</span><span class="sxs-lookup"><span data-stu-id="18c1b-123">**fNumber**</span></span>             | <span data-ttu-id="18c1b-124">Double</span><span class="sxs-lookup"><span data-stu-id="18c1b-124">Double</span></span>         | <span data-ttu-id="18c1b-p105">カメラの絞り値。読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="18c1b-p105">The F-stop value from the camera. Read-only.</span></span>
| <span data-ttu-id="18c1b-127">**exposureDenominator**</span><span class="sxs-lookup"><span data-stu-id="18c1b-127">**exposureDenominator**</span></span> | <span data-ttu-id="18c1b-128">Double</span><span class="sxs-lookup"><span data-stu-id="18c1b-128">Double</span></span>         | <span data-ttu-id="18c1b-p106">カメラの露出時間の分数の分母。読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="18c1b-p106">The denominator for the exposure time fraction from the camera. Read-only.</span></span>
| <span data-ttu-id="18c1b-131">**exposureNumerator**</span><span class="sxs-lookup"><span data-stu-id="18c1b-131">**exposureNumerator**</span></span>   | <span data-ttu-id="18c1b-132">Double</span><span class="sxs-lookup"><span data-stu-id="18c1b-132">Double</span></span>         | <span data-ttu-id="18c1b-p107">カメラの露出時間の分数の分子。読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="18c1b-p107">The numerator for the exposure time fraction from the camera. Read-only.</span></span>
| <span data-ttu-id="18c1b-135">**focalLength**</span><span class="sxs-lookup"><span data-stu-id="18c1b-135">**focalLength**</span></span>         | <span data-ttu-id="18c1b-136">Double</span><span class="sxs-lookup"><span data-stu-id="18c1b-136">Double</span></span>         | <span data-ttu-id="18c1b-p108">カメラの焦点距離。読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="18c1b-p108">The focal length from the camera. Read-only.</span></span>
| <span data-ttu-id="18c1b-139">**iso**</span><span class="sxs-lookup"><span data-stu-id="18c1b-139">**iso**</span></span>                 | <span data-ttu-id="18c1b-140">Int64</span><span class="sxs-lookup"><span data-stu-id="18c1b-140">Int64</span></span>          | <span data-ttu-id="18c1b-p109">カメラの ISO 値。読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="18c1b-p109">The ISO value from the camera. Read-only.</span></span>

## <a name="remarks"></a><span data-ttu-id="18c1b-143">注釈</span><span class="sxs-lookup"><span data-stu-id="18c1b-143">Remarks</span></span>
<span data-ttu-id="18c1b-144">OneDrive for Business と SharePoint は、**takenDateTime** プロパティのみを返します。</span><span class="sxs-lookup"><span data-stu-id="18c1b-144">OneDrive for Business and SharePoint only return the **takenDateTime** property.</span></span>

<span data-ttu-id="18c1b-145">DriveItem のファセットの詳細については、「[DriveItem](driveitem.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="18c1b-145">For more information about the facets on a DriveItem, see [DriveItem](driveitem.md).</span></span>
<!-- {
  "type": "#page.annotation",
  "description": "The photo facet provides details about the camera and settings on the camera for photos.",
  "keywords": "camera make,camera model, exposure, f-stop, iso",
  "section": "documentation",
  "tocPath": "Facets/Photo"
} -->
