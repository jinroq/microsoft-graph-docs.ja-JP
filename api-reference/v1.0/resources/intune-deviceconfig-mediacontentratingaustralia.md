---
title: mediaContentRatingAustralia リソースの種類
description: まだ文書化されていません
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 5f3f12cc233c1accfad05ccec92d412c75426d1a
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/12/2019
ms.locfileid: "27952847"
---
# <a name="mediacontentratingaustralia-resource-type"></a><span data-ttu-id="b7a12-103">mediaContentRatingAustralia リソースの種類</span><span class="sxs-lookup"><span data-stu-id="b7a12-103">mediaContentRatingAustralia resource type</span></span>

> <span data-ttu-id="b7a12-104">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="b7a12-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="b7a12-105">まだ文書化されていません</span><span class="sxs-lookup"><span data-stu-id="b7a12-105">Not yet documented</span></span>
## <a name="properties"></a><span data-ttu-id="b7a12-106">プロパティ</span><span class="sxs-lookup"><span data-stu-id="b7a12-106">Properties</span></span>
|<span data-ttu-id="b7a12-107">プロパティ</span><span class="sxs-lookup"><span data-stu-id="b7a12-107">Property</span></span>|<span data-ttu-id="b7a12-108">型</span><span class="sxs-lookup"><span data-stu-id="b7a12-108">Type</span></span>|<span data-ttu-id="b7a12-109">説明</span><span class="sxs-lookup"><span data-stu-id="b7a12-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b7a12-110">movieRating</span><span class="sxs-lookup"><span data-stu-id="b7a12-110">movieRating</span></span>|[<span data-ttu-id="b7a12-111">ratingAustraliaMoviesType</span><span class="sxs-lookup"><span data-stu-id="b7a12-111">ratingAustraliaMoviesType</span></span>](../resources/intune-deviceconfig-ratingaustraliamoviestype.md)|<span data-ttu-id="b7a12-112">評価のオーストラリアの選択したムービーです。</span><span class="sxs-lookup"><span data-stu-id="b7a12-112">Movies rating selected for Australia.</span></span> <span data-ttu-id="b7a12-113">可能な値は、`allAllowed`、`allBlocked`、`general`、`parentalGuidance`、`mature`、`agesAbove15`、`agesAbove18` です。</span><span class="sxs-lookup"><span data-stu-id="b7a12-113">Possible values are: `allAllowed`, `allBlocked`, `general`, `parentalGuidance`, `mature`, `agesAbove15`, `agesAbove18`.</span></span>|
|<span data-ttu-id="b7a12-114">tvRating</span><span class="sxs-lookup"><span data-stu-id="b7a12-114">tvRating</span></span>|[<span data-ttu-id="b7a12-115">ratingAustraliaTelevisionType</span><span class="sxs-lookup"><span data-stu-id="b7a12-115">ratingAustraliaTelevisionType</span></span>](../resources/intune-deviceconfig-ratingaustraliatelevisiontype.md)|<span data-ttu-id="b7a12-116">テレビの視聴制限がオーストラリアを選択します。</span><span class="sxs-lookup"><span data-stu-id="b7a12-116">TV rating selected for Australia.</span></span> <span data-ttu-id="b7a12-117">可能な値は、`allAllowed`、`allBlocked`、`preschoolers`、`children`、`general`、`parentalGuidance`、`mature`、`agesAbove15`、`agesAbove15AdultViolence` です。</span><span class="sxs-lookup"><span data-stu-id="b7a12-117">Possible values are: `allAllowed`, `allBlocked`, `preschoolers`, `children`, `general`, `parentalGuidance`, `mature`, `agesAbove15`, `agesAbove15AdultViolence`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="b7a12-118">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="b7a12-118">Relationships</span></span>
<span data-ttu-id="b7a12-119">なし</span><span class="sxs-lookup"><span data-stu-id="b7a12-119">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="b7a12-120">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="b7a12-120">JSON Representation</span></span>
<span data-ttu-id="b7a12-121">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="b7a12-121">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.mediaContentRatingAustralia"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.mediaContentRatingAustralia",
  "movieRating": "String",
  "tvRating": "String"
}
```



