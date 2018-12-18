---
title: mediaContentRatingUnitedKingdom リソースの種類
description: まだ文書化されていません
author: tfitzmac
ms.openlocfilehash: 0fcd17f27d999f933ce6824f8a49018013341c7b
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 12/18/2018
ms.locfileid: "27315534"
---
# <a name="mediacontentratingunitedkingdom-resource-type"></a><span data-ttu-id="339ab-103">mediaContentRatingUnitedKingdom リソースの種類</span><span class="sxs-lookup"><span data-stu-id="339ab-103">mediaContentRatingUnitedKingdom resource type</span></span>

> <span data-ttu-id="339ab-104">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="339ab-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="339ab-105">まだ文書化されていません</span><span class="sxs-lookup"><span data-stu-id="339ab-105">Not yet documented</span></span>
## <a name="properties"></a><span data-ttu-id="339ab-106">プロパティ</span><span class="sxs-lookup"><span data-stu-id="339ab-106">Properties</span></span>
|<span data-ttu-id="339ab-107">プロパティ</span><span class="sxs-lookup"><span data-stu-id="339ab-107">Property</span></span>|<span data-ttu-id="339ab-108">種類</span><span class="sxs-lookup"><span data-stu-id="339ab-108">Type</span></span>|<span data-ttu-id="339ab-109">説明</span><span class="sxs-lookup"><span data-stu-id="339ab-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="339ab-110">movieRating</span><span class="sxs-lookup"><span data-stu-id="339ab-110">movieRating</span></span>|[<span data-ttu-id="339ab-111">ratingUnitedKingdomMoviesType</span><span class="sxs-lookup"><span data-stu-id="339ab-111">ratingUnitedKingdomMoviesType</span></span>](../resources/intune-deviceconfig-ratingunitedkingdommoviestype.md)|<span data-ttu-id="339ab-112">評価の英国を選択したムービーです。</span><span class="sxs-lookup"><span data-stu-id="339ab-112">Movies rating selected for United Kingdom.</span></span> <span data-ttu-id="339ab-113">可能な値は、`allAllowed`、`allBlocked`、`general`、`universalChildren`、`parentalGuidance`、`agesAbove12Video`、`agesAbove12Cinema`、`agesAbove15`、`adults` です。</span><span class="sxs-lookup"><span data-stu-id="339ab-113">Possible values are: `allAllowed`, `allBlocked`, `general`, `universalChildren`, `parentalGuidance`, `agesAbove12Video`, `agesAbove12Cinema`, `agesAbove15`, `adults`.</span></span>|
|<span data-ttu-id="339ab-114">tvRating</span><span class="sxs-lookup"><span data-stu-id="339ab-114">tvRating</span></span>|[<span data-ttu-id="339ab-115">ratingUnitedKingdomTelevisionType</span><span class="sxs-lookup"><span data-stu-id="339ab-115">ratingUnitedKingdomTelevisionType</span></span>](../resources/intune-deviceconfig-ratingunitedkingdomtelevisiontype.md)|<span data-ttu-id="339ab-116">テレビの視聴制限が英国を選択します。</span><span class="sxs-lookup"><span data-stu-id="339ab-116">TV rating selected for United Kingdom.</span></span> <span data-ttu-id="339ab-117">可能な値は、`allAllowed`、`allBlocked`、`caution` です。</span><span class="sxs-lookup"><span data-stu-id="339ab-117">Possible values are: `allAllowed`, `allBlocked`, `caution`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="339ab-118">関係</span><span class="sxs-lookup"><span data-stu-id="339ab-118">Relationships</span></span>
<span data-ttu-id="339ab-119">なし</span><span class="sxs-lookup"><span data-stu-id="339ab-119">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="339ab-120">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="339ab-120">JSON Representation</span></span>
<span data-ttu-id="339ab-121">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="339ab-121">Here is a JSON representation of the resource.</span></span>
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



