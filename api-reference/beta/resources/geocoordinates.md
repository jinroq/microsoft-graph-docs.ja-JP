---
author: rgregg
ms.author: rgregg
ms.date: 09/10/2017
title: GeoCoordinates
ms.openlocfilehash: f9110591ee1e3350979aa2c7785cdebb2d4a584c
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27069903"
---
# <a name="geocoordinates-resource-type"></a><span data-ttu-id="4163f-102">GeoCoordinates リソースの種類</span><span class="sxs-lookup"><span data-stu-id="4163f-102">GeoCoordinates resource type</span></span>

> <span data-ttu-id="4163f-103">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="4163f-103">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="4163f-104">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="4163f-104">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="4163f-p102">**GeoCoordinates** リソースは、ファイル内に含まれるメタデータに基づいて場所の地理座標系と高度を提供します。[**DriveItem**](driveitem.md) に null でない**場所**のファセットがある場合は、アイテムは、それに関連付けられている既知の場所を含むファイルを表します。</span><span class="sxs-lookup"><span data-stu-id="4163f-p102">The **GeoCoordinates** resource provides geographic coordinates and elevation of a location based on metadata contained within the file. If a [**DriveItem**](driveitem.md) has a non-null **location** facet, the item represents a file with a known location assocaited with it.</span></span>

## <a name="json-representation"></a><span data-ttu-id="4163f-107">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="4163f-107">JSON representation</span></span>

<span data-ttu-id="4163f-108">以下は、リソースの JSON 表記です</span><span class="sxs-lookup"><span data-stu-id="4163f-108">Here is a JSON representation of the resource</span></span>

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

## <a name="properties"></a><span data-ttu-id="4163f-109">プロパティ</span><span class="sxs-lookup"><span data-stu-id="4163f-109">Properties</span></span>

| <span data-ttu-id="4163f-110">プロパティ</span><span class="sxs-lookup"><span data-stu-id="4163f-110">Property</span></span>  | <span data-ttu-id="4163f-111">型</span><span class="sxs-lookup"><span data-stu-id="4163f-111">Type</span></span>   | <span data-ttu-id="4163f-112">説明</span><span class="sxs-lookup"><span data-stu-id="4163f-112">Description</span></span>
|:----------|:-------|:--------------------------------------------------------
| <span data-ttu-id="4163f-113">altitude</span><span class="sxs-lookup"><span data-stu-id="4163f-113">altitude</span></span>  | <span data-ttu-id="4163f-114">倍精度浮動小数点数</span><span class="sxs-lookup"><span data-stu-id="4163f-114">Double</span></span> | <span data-ttu-id="4163f-p103">省略可能。アイテムの海抜をフィート単位で表した高度 (高さ)。読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="4163f-p103">Optional. The altitude (height), in feet,  above sea level for the item. Read-only.</span></span>
| <span data-ttu-id="4163f-118">latitude</span><span class="sxs-lookup"><span data-stu-id="4163f-118">latitude</span></span>  | <span data-ttu-id="4163f-119">倍精度浮動小数点数</span><span class="sxs-lookup"><span data-stu-id="4163f-119">Double</span></span> | <span data-ttu-id="4163f-p104">省略可能。アイテムの緯度 (10 進数)。読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="4163f-p104">Optional. The latitude, in decimal, for the item. Read-only.</span></span>
| <span data-ttu-id="4163f-123">longitude</span><span class="sxs-lookup"><span data-stu-id="4163f-123">longitude</span></span> | <span data-ttu-id="4163f-124">倍精度浮動小数点数</span><span class="sxs-lookup"><span data-stu-id="4163f-124">Double</span></span> | <span data-ttu-id="4163f-p105">省略可能。アイテムの経度 (10 進数)。読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="4163f-p105">Optional. The longitude, in decimal, for the item. Read-only.</span></span>

## <a name="remarks"></a><span data-ttu-id="4163f-128">注釈</span><span class="sxs-lookup"><span data-stu-id="4163f-128">Remarks</span></span>

<span data-ttu-id="4163f-129">DriveItem のファセットの詳細については、「[DriveItem](driveitem.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="4163f-129">For more information about the facets on a DriveItem, see [DriveItem](driveitem.md).</span></span>

<!-- {
  "type": "#page.annotation",
  "description": "The location facet provides geographic location related properties for an item",
  "keywords": "location,geographic,item,onedrive",
  "section": "documentation",
  "tocPath": "Facets/Location"
} -->
