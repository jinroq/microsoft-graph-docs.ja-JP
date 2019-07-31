---
author: JeremyKelley
description: GeoCoordinates リソースは、ファイルに含まれているメタデータに基づいて、場所の地理的な座標と仰角を提供します。
ms.date: 09/10/2017
title: GeoCoordinates
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
ms.openlocfilehash: 98f9c09c4604311c0cc741028565be860eb996ef
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "35971950"
---
# <a name="geocoordinates-resource-type"></a><span data-ttu-id="d13f2-103">GeoCoordinates リソースの種類</span><span class="sxs-lookup"><span data-stu-id="d13f2-103">GeoCoordinates resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="d13f2-p101">**GeoCoordinates** リソースは、ファイル内に含まれるメタデータに基づいて場所の地理座標系と高度を提供します。[**DriveItem**](driveitem.md) に null でない**場所**のファセットがある場合は、アイテムは、それに関連付けられている既知の場所を含むファイルを表します。</span><span class="sxs-lookup"><span data-stu-id="d13f2-p101">The **GeoCoordinates** resource provides geographic coordinates and elevation of a location based on metadata contained within the file. If a [**DriveItem**](driveitem.md) has a non-null **location** facet, the item represents a file with a known location assocaited with it.</span></span>

## <a name="json-representation"></a><span data-ttu-id="d13f2-106">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="d13f2-106">JSON representation</span></span>

<span data-ttu-id="d13f2-107">以下は、リソースの JSON 表記です</span><span class="sxs-lookup"><span data-stu-id="d13f2-107">Here is a JSON representation of the resource</span></span>

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

## <a name="properties"></a><span data-ttu-id="d13f2-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="d13f2-108">Properties</span></span>

| <span data-ttu-id="d13f2-109">プロパティ</span><span class="sxs-lookup"><span data-stu-id="d13f2-109">Property</span></span>  | <span data-ttu-id="d13f2-110">型</span><span class="sxs-lookup"><span data-stu-id="d13f2-110">Type</span></span>   | <span data-ttu-id="d13f2-111">説明</span><span class="sxs-lookup"><span data-stu-id="d13f2-111">Description</span></span>
|:----------|:-------|:--------------------------------------------------------
| <span data-ttu-id="d13f2-112">altitude</span><span class="sxs-lookup"><span data-stu-id="d13f2-112">altitude</span></span>  | <span data-ttu-id="d13f2-113">2 行分</span><span class="sxs-lookup"><span data-stu-id="d13f2-113">Double</span></span> | <span data-ttu-id="d13f2-p102">省略可能。アイテムの海抜をフィート単位で表した高度 (高さ)。読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="d13f2-p102">Optional. The altitude (height), in feet,  above sea level for the item. Read-only.</span></span>
| <span data-ttu-id="d13f2-117">latitude</span><span class="sxs-lookup"><span data-stu-id="d13f2-117">latitude</span></span>  | <span data-ttu-id="d13f2-118">2 行分</span><span class="sxs-lookup"><span data-stu-id="d13f2-118">Double</span></span> | <span data-ttu-id="d13f2-p103">省略可能。アイテムの緯度 (10 進数)。読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="d13f2-p103">Optional. The latitude, in decimal, for the item. Read-only.</span></span>
| <span data-ttu-id="d13f2-122">longitude</span><span class="sxs-lookup"><span data-stu-id="d13f2-122">longitude</span></span> | <span data-ttu-id="d13f2-123">Double</span><span class="sxs-lookup"><span data-stu-id="d13f2-123">Double</span></span> | <span data-ttu-id="d13f2-p104">省略可能。アイテムの経度 (10 進数)。読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="d13f2-p104">Optional. The longitude, in decimal, for the item. Read-only.</span></span>

## <a name="remarks"></a><span data-ttu-id="d13f2-127">注釈</span><span class="sxs-lookup"><span data-stu-id="d13f2-127">Remarks</span></span>

<span data-ttu-id="d13f2-128">DriveItem のファセットの詳細については、「[DriveItem](driveitem.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="d13f2-128">For more information about the facets on a DriveItem, see [DriveItem](driveitem.md).</span></span>

<!--
{
  "type": "#page.annotation",
  "description": "The location facet provides geographic location related properties for an item",
  "keywords": "location,geographic,item,onedrive",
  "section": "documentation",
  "tocPath": "Facets/Location",
  "suppressions": []
}
-->
