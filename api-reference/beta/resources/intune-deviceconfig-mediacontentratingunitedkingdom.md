---
title: mediaContentRatingUnitedKingdom リソースの種類
description: まだ文書化されていません
ms.openlocfilehash: 34117db449f65943d0f6e5e0700bbb2c0d19c426
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27066942"
---
# <a name="mediacontentratingunitedkingdom-resource-type"></a><span data-ttu-id="97409-103">mediaContentRatingUnitedKingdom リソースの種類</span><span class="sxs-lookup"><span data-stu-id="97409-103">mediaContentRatingUnitedKingdom resource type</span></span>

> <span data-ttu-id="97409-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="97409-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="97409-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="97409-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="97409-106">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="97409-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="97409-107">まだ文書化されていません</span><span class="sxs-lookup"><span data-stu-id="97409-107">Not yet documented</span></span>
## <a name="properties"></a><span data-ttu-id="97409-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="97409-108">Properties</span></span>
|<span data-ttu-id="97409-109">プロパティ</span><span class="sxs-lookup"><span data-stu-id="97409-109">Property</span></span>|<span data-ttu-id="97409-110">型</span><span class="sxs-lookup"><span data-stu-id="97409-110">Type</span></span>|<span data-ttu-id="97409-111">説明</span><span class="sxs-lookup"><span data-stu-id="97409-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="97409-112">movieRating</span><span class="sxs-lookup"><span data-stu-id="97409-112">movieRating</span></span>|[<span data-ttu-id="97409-113">ratingUnitedKingdomMoviesType</span><span class="sxs-lookup"><span data-stu-id="97409-113">ratingUnitedKingdomMoviesType</span></span>](../resources/intune-deviceconfig-ratingunitedkingdommoviestype.md)|<span data-ttu-id="97409-114">評価の英国を選択したムービーです。</span><span class="sxs-lookup"><span data-stu-id="97409-114">Movies rating selected for United Kingdom.</span></span> <span data-ttu-id="97409-115">可能な値は、`allAllowed`、`allBlocked`、`general`、`universalChildren`、`parentalGuidance`、`agesAbove12Video`、`agesAbove12Cinema`、`agesAbove15`、`adults` です。</span><span class="sxs-lookup"><span data-stu-id="97409-115">Possible values are: `allAllowed`, `allBlocked`, `general`, `universalChildren`, `parentalGuidance`, `agesAbove12Video`, `agesAbove12Cinema`, `agesAbove15`, `adults`.</span></span>|
|<span data-ttu-id="97409-116">tvRating</span><span class="sxs-lookup"><span data-stu-id="97409-116">tvRating</span></span>|[<span data-ttu-id="97409-117">ratingUnitedKingdomTelevisionType</span><span class="sxs-lookup"><span data-stu-id="97409-117">ratingUnitedKingdomTelevisionType</span></span>](../resources/intune-deviceconfig-ratingunitedkingdomtelevisiontype.md)|<span data-ttu-id="97409-118">テレビの視聴制限が英国を選択します。</span><span class="sxs-lookup"><span data-stu-id="97409-118">TV rating selected for United Kingdom.</span></span> <span data-ttu-id="97409-119">可能な値は、`allAllowed`、`allBlocked`、`caution` です。</span><span class="sxs-lookup"><span data-stu-id="97409-119">Possible values are: `allAllowed`, `allBlocked`, `caution`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="97409-120">関係</span><span class="sxs-lookup"><span data-stu-id="97409-120">Relationships</span></span>
<span data-ttu-id="97409-121">なし</span><span class="sxs-lookup"><span data-stu-id="97409-121">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="97409-122">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="97409-122">JSON Representation</span></span>
<span data-ttu-id="97409-123">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="97409-123">Here is a JSON representation of the resource.</span></span>
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





