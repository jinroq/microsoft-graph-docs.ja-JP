---
title: outlookGeoCoordinates リソースの種類
description: 物理的な場所に関する地理的な座標と標高、およびそれらの値の精度を表します。
localization_priority: Normal
author: angelgolfer-ms
ms.prod: outlook
ms.openlocfilehash: 7ca63aa3df6a597aaacb81fbeacf275ac87064f1
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/24/2019
ms.locfileid: "29511836"
---
# <a name="outlookgeocoordinates-resource-type"></a><span data-ttu-id="3cd6b-103">outlookGeoCoordinates リソースの種類</span><span class="sxs-lookup"><span data-stu-id="3cd6b-103">outlookGeoCoordinates resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="3cd6b-104">物理的な場所に関する地理的な座標と標高、およびそれらの値の精度を表します。</span><span class="sxs-lookup"><span data-stu-id="3cd6b-104">The geographic coordinates, elevation, and their degree of accuracy for a physical location.</span></span>

## <a name="json-representation"></a><span data-ttu-id="3cd6b-105">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="3cd6b-105">JSON representation</span></span>

<span data-ttu-id="3cd6b-106">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="3cd6b-106">Here is a JSON representation of the resource.</span></span>

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
## <a name="properties"></a><span data-ttu-id="3cd6b-107">プロパティ</span><span class="sxs-lookup"><span data-stu-id="3cd6b-107">Properties</span></span>
| <span data-ttu-id="3cd6b-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="3cd6b-108">Property</span></span>     | <span data-ttu-id="3cd6b-109">型</span><span class="sxs-lookup"><span data-stu-id="3cd6b-109">Type</span></span>   |<span data-ttu-id="3cd6b-110">説明</span><span class="sxs-lookup"><span data-stu-id="3cd6b-110">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="3cd6b-111">accuracy</span><span class="sxs-lookup"><span data-stu-id="3cd6b-111">accuracy</span></span>|<span data-ttu-id="3cd6b-112">double</span><span class="sxs-lookup"><span data-stu-id="3cd6b-112">double</span></span>|<span data-ttu-id="3cd6b-113">緯度と経度の精度です。</span><span class="sxs-lookup"><span data-stu-id="3cd6b-113">The accuracy of the latitude and longitude.</span></span> <span data-ttu-id="3cd6b-114">一例として、緯度と経度の精度が 50 メートル以内となるように、精度をメートル単位で測定することができます。</span><span class="sxs-lookup"><span data-stu-id="3cd6b-114">As an example, the accuracy can be measured in meters, such as the latitude and longitude are accurate to within 50 meters.</span></span>|
|<span data-ttu-id="3cd6b-115">altitude</span><span class="sxs-lookup"><span data-stu-id="3cd6b-115">altitude</span></span>|<span data-ttu-id="3cd6b-116">double</span><span class="sxs-lookup"><span data-stu-id="3cd6b-116">double</span></span>|<span data-ttu-id="3cd6b-117">場所の標高です。</span><span class="sxs-lookup"><span data-stu-id="3cd6b-117">The altitude of the location.</span></span>|
|<span data-ttu-id="3cd6b-118">altitudeAccuracy</span><span class="sxs-lookup"><span data-stu-id="3cd6b-118">altitudeAccuracy</span></span>|<span data-ttu-id="3cd6b-119">double</span><span class="sxs-lookup"><span data-stu-id="3cd6b-119">double</span></span>|<span data-ttu-id="3cd6b-120">標高の精度。</span><span class="sxs-lookup"><span data-stu-id="3cd6b-120">The accuracy of the altitude.</span></span>|
|<span data-ttu-id="3cd6b-121">latitude</span><span class="sxs-lookup"><span data-stu-id="3cd6b-121">latitude</span></span>|<span data-ttu-id="3cd6b-122">double</span><span class="sxs-lookup"><span data-stu-id="3cd6b-122">double</span></span>|<span data-ttu-id="3cd6b-123">場所の緯度です。</span><span class="sxs-lookup"><span data-stu-id="3cd6b-123">The latitude of the location.</span></span>|
|<span data-ttu-id="3cd6b-124">longitude</span><span class="sxs-lookup"><span data-stu-id="3cd6b-124">longitude</span></span>|<span data-ttu-id="3cd6b-125">double</span><span class="sxs-lookup"><span data-stu-id="3cd6b-125">double</span></span>|<span data-ttu-id="3cd6b-126">場所の経度です。</span><span class="sxs-lookup"><span data-stu-id="3cd6b-126">The longitude of the location.</span></span>|

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "outlookGeoCoordinates resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/outlookgeocoordinates.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
