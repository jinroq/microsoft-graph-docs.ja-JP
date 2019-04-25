---
title: signInLocation リソースの種類
description: サインインが行われた場所から、市区町村、都道府県、および国/地域を提供します。
localization_priority: Normal
ms.openlocfilehash: 49d6dfb07c635ac3754b3e873d75911a43593a73
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32551765"
---
# <a name="signinlocation-resource-type"></a><span data-ttu-id="80ab3-103">signInLocation リソースの種類</span><span class="sxs-lookup"><span data-stu-id="80ab3-103">signInLocation resource type</span></span>
<span data-ttu-id="80ab3-104">サインインが行われた場所から、市区町村、都道府県、および国/地域を提供します。</span><span class="sxs-lookup"><span data-stu-id="80ab3-104">Provides the city, state and country/region from where the sign-in happened.</span></span>



## <a name="properties"></a><span data-ttu-id="80ab3-105">プロパティ</span><span class="sxs-lookup"><span data-stu-id="80ab3-105">Properties</span></span>
| <span data-ttu-id="80ab3-106">プロパティ</span><span class="sxs-lookup"><span data-stu-id="80ab3-106">Property</span></span>     | <span data-ttu-id="80ab3-107">型</span><span class="sxs-lookup"><span data-stu-id="80ab3-107">Type</span></span>   |<span data-ttu-id="80ab3-108">説明</span><span class="sxs-lookup"><span data-stu-id="80ab3-108">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="80ab3-109">city</span><span class="sxs-lookup"><span data-stu-id="80ab3-109">city</span></span>|<span data-ttu-id="80ab3-110">String</span><span class="sxs-lookup"><span data-stu-id="80ab3-110">String</span></span>|<span data-ttu-id="80ab3-111">サインインが発生した都市を提供します。</span><span class="sxs-lookup"><span data-stu-id="80ab3-111">Provides the city where the sign-in originated.</span></span> <span data-ttu-id="80ab3-112">これは、サインインアクティビティの緯度/経度情報を使用して計算されます。</span><span class="sxs-lookup"><span data-stu-id="80ab3-112">This is calculated using latitude/longitude information from the sign-in activity.</span></span>|
|<span data-ttu-id="80ab3-113">countryOrRegion</span><span class="sxs-lookup"><span data-stu-id="80ab3-113">countryOrRegion</span></span>|<span data-ttu-id="80ab3-114">String</span><span class="sxs-lookup"><span data-stu-id="80ab3-114">String</span></span>|<span data-ttu-id="80ab3-115">サインインが発生した国コード情報 (2 文字コード) を提供します。</span><span class="sxs-lookup"><span data-stu-id="80ab3-115">Provides the country code info (2 letter code) where the sign-in originated.</span></span>  <span data-ttu-id="80ab3-116">これは、サインインアクティビティの緯度/経度情報を使用して計算されます。</span><span class="sxs-lookup"><span data-stu-id="80ab3-116">This is calculated using latitude/longitude information from the sign-in activity.</span></span>|
|<span data-ttu-id="80ab3-117">geoCoordinates</span><span class="sxs-lookup"><span data-stu-id="80ab3-117">geoCoordinates</span></span>|[<span data-ttu-id="80ab3-118">geoCoordinates</span><span class="sxs-lookup"><span data-stu-id="80ab3-118">geoCoordinates</span></span>](geocoordinates.md)|<span data-ttu-id="80ab3-119">サインインしたときの緯度、経度、高度を提供します。</span><span class="sxs-lookup"><span data-stu-id="80ab3-119">Provides the latitude, longitude and altitude where the sign-in originated.</span></span>|
|<span data-ttu-id="80ab3-120">state</span><span class="sxs-lookup"><span data-stu-id="80ab3-120">state</span></span>|<span data-ttu-id="80ab3-121">String</span><span class="sxs-lookup"><span data-stu-id="80ab3-121">String</span></span>|<span data-ttu-id="80ab3-122">サインインが開始された状態を提供します。</span><span class="sxs-lookup"><span data-stu-id="80ab3-122">Provides the State where the sign-in originated.</span></span> <span data-ttu-id="80ab3-123">これは、サインインアクティビティの緯度/経度情報を使用して計算されます。</span><span class="sxs-lookup"><span data-stu-id="80ab3-123">This is calculated using latitude/longitude information from the sign-in activity.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="80ab3-124">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="80ab3-124">JSON representation</span></span>

<span data-ttu-id="80ab3-125">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="80ab3-125">Here is a JSON representation of the resource.</span></span>

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
