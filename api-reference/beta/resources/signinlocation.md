---
title: signInLocation リソースの種類
description: 市、州、および記号の発生場所からの国を提供します。
ms.openlocfilehash: a3d4f6ca5ec18e70960f45a3da1bb06d51ee1e65
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27070574"
---
# <a name="signinlocation-resource-type"></a><span data-ttu-id="ecd6c-103">signInLocation リソースの種類</span><span class="sxs-lookup"><span data-stu-id="ecd6c-103">signInLocation resource type</span></span>
<span data-ttu-id="ecd6c-104">市、州、および記号の発生場所からの国を提供します。</span><span class="sxs-lookup"><span data-stu-id="ecd6c-104">Provides the city, state and country/region from where the sign-in happened.</span></span>



## <a name="properties"></a><span data-ttu-id="ecd6c-105">プロパティ</span><span class="sxs-lookup"><span data-stu-id="ecd6c-105">Properties</span></span>
| <span data-ttu-id="ecd6c-106">プロパティ</span><span class="sxs-lookup"><span data-stu-id="ecd6c-106">Property</span></span>     | <span data-ttu-id="ecd6c-107">型</span><span class="sxs-lookup"><span data-stu-id="ecd6c-107">Type</span></span>   |<span data-ttu-id="ecd6c-108">説明</span><span class="sxs-lookup"><span data-stu-id="ecd6c-108">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="ecd6c-109">city</span><span class="sxs-lookup"><span data-stu-id="ecd6c-109">city</span></span>|<span data-ttu-id="ecd6c-110">String</span><span class="sxs-lookup"><span data-stu-id="ecd6c-110">String</span></span>|<span data-ttu-id="ecd6c-111">サインインが発生した場所の市区町村を提供します。</span><span class="sxs-lookup"><span data-stu-id="ecd6c-111">Provides the city where the sign-in originated.</span></span> <span data-ttu-id="ecd6c-112">これは、サインインの活動からの緯度/経度情報を使用して計算されます。</span><span class="sxs-lookup"><span data-stu-id="ecd6c-112">This is calculated using latitude/longitude information from the sign-in activity.</span></span>|
|<span data-ttu-id="ecd6c-113">countryOrRegion</span><span class="sxs-lookup"><span data-stu-id="ecd6c-113">countryOrRegion</span></span>|<span data-ttu-id="ecd6c-114">String</span><span class="sxs-lookup"><span data-stu-id="ecd6c-114">String</span></span>|<span data-ttu-id="ecd6c-115">サインインが発生した場所 (2 文字のコード) の国コード情報を提供します。</span><span class="sxs-lookup"><span data-stu-id="ecd6c-115">Provides the country code info (2 letter code) where the sign-in originated.</span></span>  <span data-ttu-id="ecd6c-116">これは、サインインの活動からの緯度/経度情報を使用して計算されます。</span><span class="sxs-lookup"><span data-stu-id="ecd6c-116">This is calculated using latitude/longitude information from the sign-in activity.</span></span>|
|<span data-ttu-id="ecd6c-117">geoCoordinates</span><span class="sxs-lookup"><span data-stu-id="ecd6c-117">geoCoordinates</span></span>|[<span data-ttu-id="ecd6c-118">geoCoordinates</span><span class="sxs-lookup"><span data-stu-id="ecd6c-118">geoCoordinates</span></span>](geocoordinates.md)|<span data-ttu-id="ecd6c-119">緯度、経度および高度の記号には、発生した場所を提供します。</span><span class="sxs-lookup"><span data-stu-id="ecd6c-119">Provides the latitude, longitude and altitude where the sign-in originated.</span></span>|
|<span data-ttu-id="ecd6c-120">state</span><span class="sxs-lookup"><span data-stu-id="ecd6c-120">state</span></span>|<span data-ttu-id="ecd6c-121">String</span><span class="sxs-lookup"><span data-stu-id="ecd6c-121">String</span></span>|<span data-ttu-id="ecd6c-122">サインインが発生した場所の状態を提供します。</span><span class="sxs-lookup"><span data-stu-id="ecd6c-122">Provides the State where the sign-in originated.</span></span> <span data-ttu-id="ecd6c-123">これは、サインインの活動からの緯度/経度情報を使用して計算されます。</span><span class="sxs-lookup"><span data-stu-id="ecd6c-123">This is calculated using latitude/longitude information from the sign-in activity.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="ecd6c-124">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="ecd6c-124">JSON representation</span></span>

<span data-ttu-id="ecd6c-125">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="ecd6c-125">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.signInLocation"
}-->

```json
{
  "city": "String",
  "countryOrRegion": "String",
  "geoCoordinates": {"@odata.type": "microsoft.graph.geoCoordinates"},
  "state": "String"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "signInLocation resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->