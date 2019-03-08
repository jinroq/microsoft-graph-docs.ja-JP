---
author: JeremyKelley
ms.author: JeremyKelley
ms.date: 09/10/2017
title: GeoCoordinates
localization_priority: Normal
ms.openlocfilehash: 221037578e055e5bb57987058a190bc3026b3e0c
ms.sourcegitcommit: b877a8dc9aeaf74f975ca495b401ffff001d7699
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 03/08/2019
ms.locfileid: "30482358"
---
# <a name="geocoordinates-resource-type"></a><span data-ttu-id="32bcc-102">GeoCoordinates リソースの種類</span><span class="sxs-lookup"><span data-stu-id="32bcc-102">GeoCoordinates resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="32bcc-p101">**GeoCoordinates** リソースは、ファイル内に含まれるメタデータに基づいて場所の地理座標系と高度を提供します。[**DriveItem**](driveitem.md) に null でない**場所**のファセットがある場合は、アイテムは、それに関連付けられている既知の場所を含むファイルを表します。</span><span class="sxs-lookup"><span data-stu-id="32bcc-p101">The **GeoCoordinates** resource provides geographic coordinates and elevation of a location based on metadata contained within the file. If a [**DriveItem**](driveitem.md) has a non-null **location** facet, the item represents a file with a known location assocaited with it.</span></span>

## <a name="json-representation"></a><span data-ttu-id="32bcc-105">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="32bcc-105">JSON representation</span></span>

<span data-ttu-id="32bcc-106">以下は、リソースの JSON 表記です</span><span class="sxs-lookup"><span data-stu-id="32bcc-106">Here is a JSON representation of the resource</span></span>

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

## <a name="properties"></a><span data-ttu-id="32bcc-107">プロパティ</span><span class="sxs-lookup"><span data-stu-id="32bcc-107">Properties</span></span>

| <span data-ttu-id="32bcc-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="32bcc-108">Property</span></span>  | <span data-ttu-id="32bcc-109">種類</span><span class="sxs-lookup"><span data-stu-id="32bcc-109">Type</span></span>   | <span data-ttu-id="32bcc-110">説明</span><span class="sxs-lookup"><span data-stu-id="32bcc-110">Description</span></span>
|:----------|:-------|:--------------------------------------------------------
| <span data-ttu-id="32bcc-111">altitude</span><span class="sxs-lookup"><span data-stu-id="32bcc-111">altitude</span></span>  | <span data-ttu-id="32bcc-112">倍精度浮動小数点数</span><span class="sxs-lookup"><span data-stu-id="32bcc-112">Double</span></span> | <span data-ttu-id="32bcc-p102">省略可能。アイテムの海抜をフィート単位で表した高度 (高さ)。読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="32bcc-p102">Optional. The altitude (height), in feet,  above sea level for the item. Read-only.</span></span>
| <span data-ttu-id="32bcc-116">latitude</span><span class="sxs-lookup"><span data-stu-id="32bcc-116">latitude</span></span>  | <span data-ttu-id="32bcc-117">倍精度浮動小数点数</span><span class="sxs-lookup"><span data-stu-id="32bcc-117">Double</span></span> | <span data-ttu-id="32bcc-p103">省略可能。アイテムの緯度 (10 進数)。読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="32bcc-p103">Optional. The latitude, in decimal, for the item. Read-only.</span></span>
| <span data-ttu-id="32bcc-121">longitude</span><span class="sxs-lookup"><span data-stu-id="32bcc-121">longitude</span></span> | <span data-ttu-id="32bcc-122">Double</span><span class="sxs-lookup"><span data-stu-id="32bcc-122">Double</span></span> | <span data-ttu-id="32bcc-p104">省略可能。アイテムの経度 (10 進数)。読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="32bcc-p104">Optional. The longitude, in decimal, for the item. Read-only.</span></span>

## <a name="remarks"></a><span data-ttu-id="32bcc-126">注釈</span><span class="sxs-lookup"><span data-stu-id="32bcc-126">Remarks</span></span>

<span data-ttu-id="32bcc-127">DriveItem のファセットの詳細については、「[DriveItem](driveitem.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="32bcc-127">For more information about the facets on a DriveItem, see [DriveItem](driveitem.md).</span></span>

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
