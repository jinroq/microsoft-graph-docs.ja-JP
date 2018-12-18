---
title: mediaContentRatingIreland リソースの種類
description: まだ文書化されていません
author: tfitzmac
ms.openlocfilehash: 6ade4ea9d5f2236803a8515b94ebc57f32ce3cd7
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 12/18/2018
ms.locfileid: "27337493"
---
# <a name="mediacontentratingireland-resource-type"></a><span data-ttu-id="20e6d-103">mediaContentRatingIreland リソースの種類</span><span class="sxs-lookup"><span data-stu-id="20e6d-103">mediaContentRatingIreland resource type</span></span>

> <span data-ttu-id="20e6d-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="20e6d-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="20e6d-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="20e6d-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="20e6d-106">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="20e6d-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="20e6d-107">まだ文書化されていません</span><span class="sxs-lookup"><span data-stu-id="20e6d-107">Not yet documented</span></span>
## <a name="properties"></a><span data-ttu-id="20e6d-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="20e6d-108">Properties</span></span>
|<span data-ttu-id="20e6d-109">プロパティ</span><span class="sxs-lookup"><span data-stu-id="20e6d-109">Property</span></span>|<span data-ttu-id="20e6d-110">種類</span><span class="sxs-lookup"><span data-stu-id="20e6d-110">Type</span></span>|<span data-ttu-id="20e6d-111">説明</span><span class="sxs-lookup"><span data-stu-id="20e6d-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="20e6d-112">movieRating</span><span class="sxs-lookup"><span data-stu-id="20e6d-112">movieRating</span></span>|[<span data-ttu-id="20e6d-113">ratingIrelandMoviesType</span><span class="sxs-lookup"><span data-stu-id="20e6d-113">ratingIrelandMoviesType</span></span>](../resources/intune-deviceconfig-ratingirelandmoviestype.md)|<span data-ttu-id="20e6d-114">評価のアイルランドの選択したムービーです。</span><span class="sxs-lookup"><span data-stu-id="20e6d-114">Movies rating selected for Ireland.</span></span> <span data-ttu-id="20e6d-115">可能な値は、`allAllowed`、`allBlocked`、`general`、`parentalGuidance`、`agesAbove12`、`agesAbove15`、`agesAbove16`、`adults` です。</span><span class="sxs-lookup"><span data-stu-id="20e6d-115">Possible values are: `allAllowed`, `allBlocked`, `general`, `parentalGuidance`, `agesAbove12`, `agesAbove15`, `agesAbove16`, `adults`.</span></span>|
|<span data-ttu-id="20e6d-116">tvRating</span><span class="sxs-lookup"><span data-stu-id="20e6d-116">tvRating</span></span>|[<span data-ttu-id="20e6d-117">ratingIrelandTelevisionType</span><span class="sxs-lookup"><span data-stu-id="20e6d-117">ratingIrelandTelevisionType</span></span>](../resources/intune-deviceconfig-ratingirelandtelevisiontype.md)|<span data-ttu-id="20e6d-118">テレビの視聴制限はアイルランドのために選択します。</span><span class="sxs-lookup"><span data-stu-id="20e6d-118">TV rating selected for Ireland.</span></span> <span data-ttu-id="20e6d-119">可能な値は、`allAllowed`、`allBlocked`、`general`、`children`、`youngAdults`、`parentalSupervision`、`mature` です。</span><span class="sxs-lookup"><span data-stu-id="20e6d-119">Possible values are: `allAllowed`, `allBlocked`, `general`, `children`, `youngAdults`, `parentalSupervision`, `mature`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="20e6d-120">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="20e6d-120">Relationships</span></span>
<span data-ttu-id="20e6d-121">なし</span><span class="sxs-lookup"><span data-stu-id="20e6d-121">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="20e6d-122">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="20e6d-122">JSON Representation</span></span>
<span data-ttu-id="20e6d-123">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="20e6d-123">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.mediaContentRatingIreland"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.mediaContentRatingIreland",
  "movieRating": "String",
  "tvRating": "String"
}
```





