---
title: outlookGeoCoordinates リソースの種類
description: 物理的な場所に関する地理的な座標と標高、およびそれらの値の精度を表します。
localization_priority: Normal
author: angelgolfer-ms
ms.prod: outlook
ms.openlocfilehash: f51f5eeb663a1d1ce55bee083639d244905b2c37
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/12/2019
ms.locfileid: "27973119"
---
# <a name="outlookgeocoordinates-resource-type"></a><span data-ttu-id="7de2e-103">outlookGeoCoordinates リソースの種類</span><span class="sxs-lookup"><span data-stu-id="7de2e-103">outlookGeoCoordinates resource type</span></span>

> <span data-ttu-id="7de2e-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="7de2e-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="7de2e-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="7de2e-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="7de2e-106">物理的な場所に関する地理的な座標と標高、およびそれらの値の精度を表します。</span><span class="sxs-lookup"><span data-stu-id="7de2e-106">The geographic coordinates, elevation, and their degree of accuracy for a physical location.</span></span>

## <a name="json-representation"></a><span data-ttu-id="7de2e-107">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="7de2e-107">JSON representation</span></span>

<span data-ttu-id="7de2e-108">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="7de2e-108">Here is a JSON representation of the resource.</span></span>

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
## <a name="properties"></a><span data-ttu-id="7de2e-109">プロパティ</span><span class="sxs-lookup"><span data-stu-id="7de2e-109">Properties</span></span>
| <span data-ttu-id="7de2e-110">プロパティ</span><span class="sxs-lookup"><span data-stu-id="7de2e-110">Property</span></span>     | <span data-ttu-id="7de2e-111">種類</span><span class="sxs-lookup"><span data-stu-id="7de2e-111">Type</span></span>   |<span data-ttu-id="7de2e-112">説明</span><span class="sxs-lookup"><span data-stu-id="7de2e-112">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="7de2e-113">accuracy</span><span class="sxs-lookup"><span data-stu-id="7de2e-113">accuracy</span></span>|<span data-ttu-id="7de2e-114">double</span><span class="sxs-lookup"><span data-stu-id="7de2e-114">double</span></span>|<span data-ttu-id="7de2e-115">緯度と経度の精度です。</span><span class="sxs-lookup"><span data-stu-id="7de2e-115">The accuracy of the latitude and longitude.</span></span> <span data-ttu-id="7de2e-116">一例として、緯度と経度の精度が 50 メートル以内となるように、精度をメートル単位で測定することができます。</span><span class="sxs-lookup"><span data-stu-id="7de2e-116">As an example, the accuracy can be measured in meters, such as the latitude and longitude are accurate to within 50 meters.</span></span>|
|<span data-ttu-id="7de2e-117">altitude</span><span class="sxs-lookup"><span data-stu-id="7de2e-117">altitude</span></span>|<span data-ttu-id="7de2e-118">double</span><span class="sxs-lookup"><span data-stu-id="7de2e-118">double</span></span>|<span data-ttu-id="7de2e-119">場所の標高です。</span><span class="sxs-lookup"><span data-stu-id="7de2e-119">The altitude of the location.</span></span>|
|<span data-ttu-id="7de2e-120">altitudeAccuracy</span><span class="sxs-lookup"><span data-stu-id="7de2e-120">altitudeAccuracy</span></span>|<span data-ttu-id="7de2e-121">double</span><span class="sxs-lookup"><span data-stu-id="7de2e-121">double</span></span>|<span data-ttu-id="7de2e-122">標高の精度。</span><span class="sxs-lookup"><span data-stu-id="7de2e-122">The accuracy of the altitude.</span></span>|
|<span data-ttu-id="7de2e-123">latitude</span><span class="sxs-lookup"><span data-stu-id="7de2e-123">latitude</span></span>|<span data-ttu-id="7de2e-124">double</span><span class="sxs-lookup"><span data-stu-id="7de2e-124">double</span></span>|<span data-ttu-id="7de2e-125">場所の緯度です。</span><span class="sxs-lookup"><span data-stu-id="7de2e-125">The latitude of the location.</span></span>|
|<span data-ttu-id="7de2e-126">longitude</span><span class="sxs-lookup"><span data-stu-id="7de2e-126">longitude</span></span>|<span data-ttu-id="7de2e-127">double</span><span class="sxs-lookup"><span data-stu-id="7de2e-127">double</span></span>|<span data-ttu-id="7de2e-128">場所の経度です。</span><span class="sxs-lookup"><span data-stu-id="7de2e-128">The longitude of the location.</span></span>|

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "outlookGeoCoordinates resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
