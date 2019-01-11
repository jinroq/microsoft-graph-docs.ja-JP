---
title: mediaContentRatingUnitedKingdom リソースの種類
description: まだ文書化されていません
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 48cf2b491b8dc2cb9ad5234c8285d82a64350aac
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/11/2019
ms.locfileid: "27829212"
---
# <a name="mediacontentratingunitedkingdom-resource-type"></a><span data-ttu-id="80442-103">mediaContentRatingUnitedKingdom リソースの種類</span><span class="sxs-lookup"><span data-stu-id="80442-103">mediaContentRatingUnitedKingdom resource type</span></span>

> <span data-ttu-id="80442-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="80442-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="80442-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="80442-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="80442-106">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="80442-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="80442-107">まだ文書化されていません</span><span class="sxs-lookup"><span data-stu-id="80442-107">Not yet documented</span></span>
## <a name="properties"></a><span data-ttu-id="80442-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="80442-108">Properties</span></span>
|<span data-ttu-id="80442-109">プロパティ</span><span class="sxs-lookup"><span data-stu-id="80442-109">Property</span></span>|<span data-ttu-id="80442-110">種類</span><span class="sxs-lookup"><span data-stu-id="80442-110">Type</span></span>|<span data-ttu-id="80442-111">説明</span><span class="sxs-lookup"><span data-stu-id="80442-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="80442-112">movieRating</span><span class="sxs-lookup"><span data-stu-id="80442-112">movieRating</span></span>|[<span data-ttu-id="80442-113">ratingUnitedKingdomMoviesType</span><span class="sxs-lookup"><span data-stu-id="80442-113">ratingUnitedKingdomMoviesType</span></span>](../resources/intune-deviceconfig-ratingunitedkingdommoviestype.md)|<span data-ttu-id="80442-114">評価の英国を選択したムービーです。</span><span class="sxs-lookup"><span data-stu-id="80442-114">Movies rating selected for United Kingdom.</span></span> <span data-ttu-id="80442-115">可能な値は、`allAllowed`、`allBlocked`、`general`、`universalChildren`、`parentalGuidance`、`agesAbove12Video`、`agesAbove12Cinema`、`agesAbove15`、`adults` です。</span><span class="sxs-lookup"><span data-stu-id="80442-115">Possible values are: `allAllowed`, `allBlocked`, `general`, `universalChildren`, `parentalGuidance`, `agesAbove12Video`, `agesAbove12Cinema`, `agesAbove15`, `adults`.</span></span>|
|<span data-ttu-id="80442-116">tvRating</span><span class="sxs-lookup"><span data-stu-id="80442-116">tvRating</span></span>|[<span data-ttu-id="80442-117">ratingUnitedKingdomTelevisionType</span><span class="sxs-lookup"><span data-stu-id="80442-117">ratingUnitedKingdomTelevisionType</span></span>](../resources/intune-deviceconfig-ratingunitedkingdomtelevisiontype.md)|<span data-ttu-id="80442-118">テレビの視聴制限が英国を選択します。</span><span class="sxs-lookup"><span data-stu-id="80442-118">TV rating selected for United Kingdom.</span></span> <span data-ttu-id="80442-119">可能な値は、`allAllowed`、`allBlocked`、`caution` です。</span><span class="sxs-lookup"><span data-stu-id="80442-119">Possible values are: `allAllowed`, `allBlocked`, `caution`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="80442-120">関係</span><span class="sxs-lookup"><span data-stu-id="80442-120">Relationships</span></span>
<span data-ttu-id="80442-121">なし</span><span class="sxs-lookup"><span data-stu-id="80442-121">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="80442-122">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="80442-122">JSON Representation</span></span>
<span data-ttu-id="80442-123">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="80442-123">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.mediaContentRatingUnitedKingdom"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.mediaContentRatingUnitedKingdom",
  "movieRating": "String",
  "tvRating": "String"
}
```





