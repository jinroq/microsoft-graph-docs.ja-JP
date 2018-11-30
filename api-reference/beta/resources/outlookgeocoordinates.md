---
title: outlookGeoCoordinates リソースの種類
description: 物理的な場所に関する地理的な座標と標高、およびそれらの値の精度を表します。
ms.openlocfilehash: 9de60c218f6fc54ed2be12b2987126195e5eb140
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27068643"
---
# <a name="outlookgeocoordinates-resource-type"></a><span data-ttu-id="cb9a0-103">outlookGeoCoordinates リソースの種類</span><span class="sxs-lookup"><span data-stu-id="cb9a0-103">outlookGeoCoordinates resource type</span></span>

> <span data-ttu-id="cb9a0-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="cb9a0-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="cb9a0-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="cb9a0-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="cb9a0-106">物理的な場所に関する地理的な座標と標高、およびそれらの値の精度を表します。</span><span class="sxs-lookup"><span data-stu-id="cb9a0-106">The geographic coordinates, elevation, and their degree of accuracy for a physical location.</span></span>

## <a name="json-representation"></a><span data-ttu-id="cb9a0-107">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="cb9a0-107">JSON representation</span></span>

<span data-ttu-id="cb9a0-108">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="cb9a0-108">Here is a JSON representation of the resource.</span></span>

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
## <a name="properties"></a><span data-ttu-id="cb9a0-109">プロパティ</span><span class="sxs-lookup"><span data-stu-id="cb9a0-109">Properties</span></span>
| <span data-ttu-id="cb9a0-110">プロパティ</span><span class="sxs-lookup"><span data-stu-id="cb9a0-110">Property</span></span>     | <span data-ttu-id="cb9a0-111">型</span><span class="sxs-lookup"><span data-stu-id="cb9a0-111">Type</span></span>   |<span data-ttu-id="cb9a0-112">説明</span><span class="sxs-lookup"><span data-stu-id="cb9a0-112">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="cb9a0-113">accuracy</span><span class="sxs-lookup"><span data-stu-id="cb9a0-113">accuracy</span></span>|<span data-ttu-id="cb9a0-114">double</span><span class="sxs-lookup"><span data-stu-id="cb9a0-114">double</span></span>|<span data-ttu-id="cb9a0-115">緯度と経度の精度です。</span><span class="sxs-lookup"><span data-stu-id="cb9a0-115">The accuracy of the latitude and longitude.</span></span> <span data-ttu-id="cb9a0-116">一例として、緯度と経度の精度が 50 メートル以内となるように、精度をメートル単位で測定することができます。</span><span class="sxs-lookup"><span data-stu-id="cb9a0-116">As an example, the accuracy can be measured in meters, such as the latitude and longitude are accurate to within 50 meters.</span></span>|
|<span data-ttu-id="cb9a0-117">altitude</span><span class="sxs-lookup"><span data-stu-id="cb9a0-117">altitude</span></span>|<span data-ttu-id="cb9a0-118">double</span><span class="sxs-lookup"><span data-stu-id="cb9a0-118">double</span></span>|<span data-ttu-id="cb9a0-119">場所の標高です。</span><span class="sxs-lookup"><span data-stu-id="cb9a0-119">The altitude of the location.</span></span>|
|<span data-ttu-id="cb9a0-120">altitudeAccuracy</span><span class="sxs-lookup"><span data-stu-id="cb9a0-120">altitudeAccuracy</span></span>|<span data-ttu-id="cb9a0-121">double</span><span class="sxs-lookup"><span data-stu-id="cb9a0-121">double</span></span>|<span data-ttu-id="cb9a0-122">標高の精度。</span><span class="sxs-lookup"><span data-stu-id="cb9a0-122">The accuracy of the altitude.</span></span>|
|<span data-ttu-id="cb9a0-123">latitude</span><span class="sxs-lookup"><span data-stu-id="cb9a0-123">latitude</span></span>|<span data-ttu-id="cb9a0-124">double</span><span class="sxs-lookup"><span data-stu-id="cb9a0-124">double</span></span>|<span data-ttu-id="cb9a0-125">場所の緯度です。</span><span class="sxs-lookup"><span data-stu-id="cb9a0-125">The latitude of the location.</span></span>|
|<span data-ttu-id="cb9a0-126">longitude</span><span class="sxs-lookup"><span data-stu-id="cb9a0-126">longitude</span></span>|<span data-ttu-id="cb9a0-127">double</span><span class="sxs-lookup"><span data-stu-id="cb9a0-127">double</span></span>|<span data-ttu-id="cb9a0-128">場所の経度です。</span><span class="sxs-lookup"><span data-stu-id="cb9a0-128">The longitude of the location.</span></span>|

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "outlookGeoCoordinates resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->