---
title: outlookGeoCoordinates リソースの種類
description: 物理的な場所に関する地理的な座標と標高、およびそれらの値の精度を表します。
localization_priority: Normal
author: angelgolfer-ms
ms.prod: outlook
doc_type: resourcePageType
ms.openlocfilehash: 6cfa08c15318fdaa58ac71e01a940b621b207f12
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "36035673"
---
# <a name="outlookgeocoordinates-resource-type"></a><span data-ttu-id="e51fd-103">outlookGeoCoordinates リソースの種類</span><span class="sxs-lookup"><span data-stu-id="e51fd-103">outlookGeoCoordinates resource type</span></span>

<span data-ttu-id="e51fd-104">物理的な場所に関する地理的な座標と標高、およびそれらの値の精度を表します。</span><span class="sxs-lookup"><span data-stu-id="e51fd-104">The geographic coordinates, elevation, and their degree of accuracy for a physical location.</span></span>

## <a name="json-representation"></a><span data-ttu-id="e51fd-105">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="e51fd-105">JSON representation</span></span>

<span data-ttu-id="e51fd-106">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="e51fd-106">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.outlookGeoCoordinates"
}-->

```json
{
  "accuracy": 1024.13,
  "altitude": 1024.13,
  "altitudeAccuracy": 1024.13,
  "latitude": 1024.13,
  "longitude": 1024.13
}

```
## <a name="properties"></a><span data-ttu-id="e51fd-107">プロパティ</span><span class="sxs-lookup"><span data-stu-id="e51fd-107">Properties</span></span>
| <span data-ttu-id="e51fd-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="e51fd-108">Property</span></span>     | <span data-ttu-id="e51fd-109">型</span><span class="sxs-lookup"><span data-stu-id="e51fd-109">Type</span></span>   |<span data-ttu-id="e51fd-110">説明</span><span class="sxs-lookup"><span data-stu-id="e51fd-110">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="e51fd-111">accuracy</span><span class="sxs-lookup"><span data-stu-id="e51fd-111">accuracy</span></span>|<span data-ttu-id="e51fd-112">double</span><span class="sxs-lookup"><span data-stu-id="e51fd-112">double</span></span>|<span data-ttu-id="e51fd-113">緯度と経度の精度です。</span><span class="sxs-lookup"><span data-stu-id="e51fd-113">The accuracy of the latitude and longitude.</span></span> <span data-ttu-id="e51fd-114">一例として、緯度と経度の精度が 50 メートル以内となるように、精度をメートル単位で測定することができます。</span><span class="sxs-lookup"><span data-stu-id="e51fd-114">As an example, the accuracy can be measured in meters, such as the latitude and longitude are accurate to within 50 meters.</span></span>|
|<span data-ttu-id="e51fd-115">altitude</span><span class="sxs-lookup"><span data-stu-id="e51fd-115">altitude</span></span>|<span data-ttu-id="e51fd-116">double</span><span class="sxs-lookup"><span data-stu-id="e51fd-116">double</span></span>|<span data-ttu-id="e51fd-117">場所の標高です。</span><span class="sxs-lookup"><span data-stu-id="e51fd-117">The altitude of the location.</span></span>|
|<span data-ttu-id="e51fd-118">altitudeAccuracy</span><span class="sxs-lookup"><span data-stu-id="e51fd-118">altitudeAccuracy</span></span>|<span data-ttu-id="e51fd-119">double</span><span class="sxs-lookup"><span data-stu-id="e51fd-119">double</span></span>|<span data-ttu-id="e51fd-120">標高の精度。</span><span class="sxs-lookup"><span data-stu-id="e51fd-120">The accuracy of the altitude.</span></span>|
|<span data-ttu-id="e51fd-121">latitude</span><span class="sxs-lookup"><span data-stu-id="e51fd-121">latitude</span></span>|<span data-ttu-id="e51fd-122">double</span><span class="sxs-lookup"><span data-stu-id="e51fd-122">double</span></span>|<span data-ttu-id="e51fd-123">場所の緯度です。</span><span class="sxs-lookup"><span data-stu-id="e51fd-123">The latitude of the location.</span></span>|
|<span data-ttu-id="e51fd-124">longitude</span><span class="sxs-lookup"><span data-stu-id="e51fd-124">longitude</span></span>|<span data-ttu-id="e51fd-125">double</span><span class="sxs-lookup"><span data-stu-id="e51fd-125">double</span></span>|<span data-ttu-id="e51fd-126">場所の経度です。</span><span class="sxs-lookup"><span data-stu-id="e51fd-126">The longitude of the location.</span></span>|

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "outlookGeoCoordinates resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
