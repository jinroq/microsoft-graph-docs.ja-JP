---
author: rgregg
ms.author: rgregg
ms.date: 09/10/2017
title: GeoCoordinates
localization_priority: Normal
ms.openlocfilehash: 45df506820ee242b53630c9d44ed390216bae141
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/24/2019
ms.locfileid: "29525074"
---
# <a name="geocoordinates-resource-type"></a><span data-ttu-id="0017b-102">GeoCoordinates リソースの種類</span><span class="sxs-lookup"><span data-stu-id="0017b-102">GeoCoordinates resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="0017b-p101">**GeoCoordinates** リソースは、ファイル内に含まれるメタデータに基づいて場所の地理座標系と高度を提供します。[**DriveItem**](driveitem.md) に null でない**場所**のファセットがある場合は、アイテムは、それに関連付けられている既知の場所を含むファイルを表します。</span><span class="sxs-lookup"><span data-stu-id="0017b-p101">The **GeoCoordinates** resource provides geographic coordinates and elevation of a location based on metadata contained within the file. If a [**DriveItem**](driveitem.md) has a non-null **location** facet, the item represents a file with a known location assocaited with it.</span></span>

## <a name="json-representation"></a><span data-ttu-id="0017b-105">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="0017b-105">JSON representation</span></span>

<span data-ttu-id="0017b-106">以下は、リソースの JSON 表記です</span><span class="sxs-lookup"><span data-stu-id="0017b-106">Here is a JSON representation of the resource</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.geoCoordinates"
}-->

```json
{
  "altitude": 1024.13,
  "latitude": 26.13246,
  "longitude": 24.34616
}
```

## <a name="properties"></a><span data-ttu-id="0017b-107">プロパティ</span><span class="sxs-lookup"><span data-stu-id="0017b-107">Properties</span></span>

| <span data-ttu-id="0017b-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="0017b-108">Property</span></span>  | <span data-ttu-id="0017b-109">型</span><span class="sxs-lookup"><span data-stu-id="0017b-109">Type</span></span>   | <span data-ttu-id="0017b-110">説明</span><span class="sxs-lookup"><span data-stu-id="0017b-110">Description</span></span>
|:----------|:-------|:--------------------------------------------------------
| <span data-ttu-id="0017b-111">altitude</span><span class="sxs-lookup"><span data-stu-id="0017b-111">altitude</span></span>  | <span data-ttu-id="0017b-112">Double</span><span class="sxs-lookup"><span data-stu-id="0017b-112">Double</span></span> | <span data-ttu-id="0017b-p102">省略可能。アイテムの海抜をフィート単位で表した高度 (高さ)。読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="0017b-p102">Optional. The altitude (height), in feet,  above sea level for the item. Read-only.</span></span>
| <span data-ttu-id="0017b-116">latitude</span><span class="sxs-lookup"><span data-stu-id="0017b-116">latitude</span></span>  | <span data-ttu-id="0017b-117">Double</span><span class="sxs-lookup"><span data-stu-id="0017b-117">Double</span></span> | <span data-ttu-id="0017b-p103">省略可能。アイテムの緯度 (10 進数)。読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="0017b-p103">Optional. The latitude, in decimal, for the item. Read-only.</span></span>
| <span data-ttu-id="0017b-121">longitude</span><span class="sxs-lookup"><span data-stu-id="0017b-121">longitude</span></span> | <span data-ttu-id="0017b-122">Double</span><span class="sxs-lookup"><span data-stu-id="0017b-122">Double</span></span> | <span data-ttu-id="0017b-p104">省略可能。アイテムの経度 (10 進数)。読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="0017b-p104">Optional. The longitude, in decimal, for the item. Read-only.</span></span>

## <a name="remarks"></a><span data-ttu-id="0017b-126">注釈</span><span class="sxs-lookup"><span data-stu-id="0017b-126">Remarks</span></span>

<span data-ttu-id="0017b-127">DriveItem のファセットの詳細については、「[DriveItem](driveitem.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="0017b-127">For more information about the facets on a DriveItem, see [DriveItem](driveitem.md).</span></span>

<!--
{
  "type": "#page.annotation",
  "description": "The location facet provides geographic location related properties for an item",
  "keywords": "location,geographic,item,onedrive",
  "section": "documentation",
  "tocPath": "Facets/Location",
  "suppressions": [
    "Error: /api-reference/beta/resources/geocoordinates.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
