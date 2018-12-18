---
title: mediaContentRatingIreland リソースの種類
description: まだ文書化されていません
author: tfitzmac
ms.openlocfilehash: 68d5e0e9454fadde550988f46c1104733a9de013
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 12/18/2018
ms.locfileid: "27359473"
---
# <a name="mediacontentratingireland-resource-type"></a><span data-ttu-id="1d989-103">mediaContentRatingIreland リソースの種類</span><span class="sxs-lookup"><span data-stu-id="1d989-103">mediaContentRatingIreland resource type</span></span>

> <span data-ttu-id="1d989-104">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="1d989-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="1d989-105">まだ文書化されていません</span><span class="sxs-lookup"><span data-stu-id="1d989-105">Not yet documented</span></span>
## <a name="properties"></a><span data-ttu-id="1d989-106">プロパティ</span><span class="sxs-lookup"><span data-stu-id="1d989-106">Properties</span></span>
|<span data-ttu-id="1d989-107">プロパティ</span><span class="sxs-lookup"><span data-stu-id="1d989-107">Property</span></span>|<span data-ttu-id="1d989-108">種類</span><span class="sxs-lookup"><span data-stu-id="1d989-108">Type</span></span>|<span data-ttu-id="1d989-109">説明</span><span class="sxs-lookup"><span data-stu-id="1d989-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="1d989-110">movieRating</span><span class="sxs-lookup"><span data-stu-id="1d989-110">movieRating</span></span>|[<span data-ttu-id="1d989-111">ratingIrelandMoviesType</span><span class="sxs-lookup"><span data-stu-id="1d989-111">ratingIrelandMoviesType</span></span>](../resources/intune-deviceconfig-ratingirelandmoviestype.md)|<span data-ttu-id="1d989-112">評価のアイルランドの選択したムービーです。</span><span class="sxs-lookup"><span data-stu-id="1d989-112">Movies rating selected for Ireland.</span></span> <span data-ttu-id="1d989-113">可能な値は、`allAllowed`、`allBlocked`、`general`、`parentalGuidance`、`agesAbove12`、`agesAbove15`、`agesAbove16`、`adults` です。</span><span class="sxs-lookup"><span data-stu-id="1d989-113">Possible values are: `allAllowed`, `allBlocked`, `general`, `parentalGuidance`, `agesAbove12`, `agesAbove15`, `agesAbove16`, `adults`.</span></span>|
|<span data-ttu-id="1d989-114">tvRating</span><span class="sxs-lookup"><span data-stu-id="1d989-114">tvRating</span></span>|[<span data-ttu-id="1d989-115">ratingIrelandTelevisionType</span><span class="sxs-lookup"><span data-stu-id="1d989-115">ratingIrelandTelevisionType</span></span>](../resources/intune-deviceconfig-ratingirelandtelevisiontype.md)|<span data-ttu-id="1d989-116">テレビの視聴制限はアイルランドのために選択します。</span><span class="sxs-lookup"><span data-stu-id="1d989-116">TV rating selected for Ireland.</span></span> <span data-ttu-id="1d989-117">可能な値は、`allAllowed`、`allBlocked`、`general`、`children`、`youngAdults`、`parentalSupervision`、`mature` です。</span><span class="sxs-lookup"><span data-stu-id="1d989-117">Possible values are: `allAllowed`, `allBlocked`, `general`, `children`, `youngAdults`, `parentalSupervision`, `mature`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="1d989-118">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="1d989-118">Relationships</span></span>
<span data-ttu-id="1d989-119">なし</span><span class="sxs-lookup"><span data-stu-id="1d989-119">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="1d989-120">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="1d989-120">JSON Representation</span></span>
<span data-ttu-id="1d989-121">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="1d989-121">Here is a JSON representation of the resource.</span></span>
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



