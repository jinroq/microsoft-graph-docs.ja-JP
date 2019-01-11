---
title: mediaContentRatingAustralia リソースの種類
description: まだ文書化されていません
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 0860a17671b2923c2be9b5b469f93d443e808f53
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/11/2019
ms.locfileid: "27891484"
---
# <a name="mediacontentratingaustralia-resource-type"></a><span data-ttu-id="38684-103">mediaContentRatingAustralia リソースの種類</span><span class="sxs-lookup"><span data-stu-id="38684-103">mediaContentRatingAustralia resource type</span></span>

> <span data-ttu-id="38684-104">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="38684-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="38684-105">まだ文書化されていません</span><span class="sxs-lookup"><span data-stu-id="38684-105">Not yet documented</span></span>
## <a name="properties"></a><span data-ttu-id="38684-106">プロパティ</span><span class="sxs-lookup"><span data-stu-id="38684-106">Properties</span></span>
|<span data-ttu-id="38684-107">プロパティ</span><span class="sxs-lookup"><span data-stu-id="38684-107">Property</span></span>|<span data-ttu-id="38684-108">種類</span><span class="sxs-lookup"><span data-stu-id="38684-108">Type</span></span>|<span data-ttu-id="38684-109">説明</span><span class="sxs-lookup"><span data-stu-id="38684-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="38684-110">movieRating</span><span class="sxs-lookup"><span data-stu-id="38684-110">movieRating</span></span>|[<span data-ttu-id="38684-111">ratingAustraliaMoviesType</span><span class="sxs-lookup"><span data-stu-id="38684-111">ratingAustraliaMoviesType</span></span>](../resources/intune-deviceconfig-ratingaustraliamoviestype.md)|<span data-ttu-id="38684-112">評価のオーストラリアの選択したムービーです。</span><span class="sxs-lookup"><span data-stu-id="38684-112">Movies rating selected for Australia.</span></span> <span data-ttu-id="38684-113">可能な値は、`allAllowed`、`allBlocked`、`general`、`parentalGuidance`、`mature`、`agesAbove15`、`agesAbove18` です。</span><span class="sxs-lookup"><span data-stu-id="38684-113">Possible values are: `allAllowed`, `allBlocked`, `general`, `parentalGuidance`, `mature`, `agesAbove15`, `agesAbove18`.</span></span>|
|<span data-ttu-id="38684-114">tvRating</span><span class="sxs-lookup"><span data-stu-id="38684-114">tvRating</span></span>|[<span data-ttu-id="38684-115">ratingAustraliaTelevisionType</span><span class="sxs-lookup"><span data-stu-id="38684-115">ratingAustraliaTelevisionType</span></span>](../resources/intune-deviceconfig-ratingaustraliatelevisiontype.md)|<span data-ttu-id="38684-116">テレビの視聴制限がオーストラリアを選択します。</span><span class="sxs-lookup"><span data-stu-id="38684-116">TV rating selected for Australia.</span></span> <span data-ttu-id="38684-117">可能な値は、`allAllowed`、`allBlocked`、`preschoolers`、`children`、`general`、`parentalGuidance`、`mature`、`agesAbove15`、`agesAbove15AdultViolence` です。</span><span class="sxs-lookup"><span data-stu-id="38684-117">Possible values are: `allAllowed`, `allBlocked`, `preschoolers`, `children`, `general`, `parentalGuidance`, `mature`, `agesAbove15`, `agesAbove15AdultViolence`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="38684-118">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="38684-118">Relationships</span></span>
<span data-ttu-id="38684-119">なし</span><span class="sxs-lookup"><span data-stu-id="38684-119">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="38684-120">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="38684-120">JSON Representation</span></span>
<span data-ttu-id="38684-121">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="38684-121">Here is a JSON representation of the resource.</span></span>
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



