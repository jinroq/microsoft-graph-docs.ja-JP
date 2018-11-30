---
title: mediaContentRatingJapan リソースの種類
description: まだ文書化されていません
ms.openlocfilehash: 15e905355133545db2cdf0864fcbba7e9c226183
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27021589"
---
# <a name="mediacontentratingjapan-resource-type"></a><span data-ttu-id="e68d7-103">mediaContentRatingJapan リソースの種類</span><span class="sxs-lookup"><span data-stu-id="e68d7-103">mediaContentRatingJapan resource type</span></span>

> <span data-ttu-id="e68d7-104">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="e68d7-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="e68d7-105">まだ文書化されていません</span><span class="sxs-lookup"><span data-stu-id="e68d7-105">Not yet documented</span></span>
## <a name="properties"></a><span data-ttu-id="e68d7-106">プロパティ</span><span class="sxs-lookup"><span data-stu-id="e68d7-106">Properties</span></span>
|<span data-ttu-id="e68d7-107">プロパティ</span><span class="sxs-lookup"><span data-stu-id="e68d7-107">Property</span></span>|<span data-ttu-id="e68d7-108">型</span><span class="sxs-lookup"><span data-stu-id="e68d7-108">Type</span></span>|<span data-ttu-id="e68d7-109">説明</span><span class="sxs-lookup"><span data-stu-id="e68d7-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e68d7-110">movieRating</span><span class="sxs-lookup"><span data-stu-id="e68d7-110">movieRating</span></span>|[<span data-ttu-id="e68d7-111">ratingJapanMoviesType</span><span class="sxs-lookup"><span data-stu-id="e68d7-111">ratingJapanMoviesType</span></span>](../resources/intune-deviceconfig-ratingjapanmoviestype.md)|<span data-ttu-id="e68d7-112">評価日本の選択したムービーです。</span><span class="sxs-lookup"><span data-stu-id="e68d7-112">Movies rating selected for Japan.</span></span> <span data-ttu-id="e68d7-113">使用可能な値: `allAllowed`、`allBlocked`、`general`、`parentalGuidance`、`agesAbove15`、`agesAbove18`。</span><span class="sxs-lookup"><span data-stu-id="e68d7-113">Possible values are: `allAllowed`, `allBlocked`, `general`, `parentalGuidance`, `agesAbove15`, `agesAbove18`.</span></span>|
|<span data-ttu-id="e68d7-114">tvRating</span><span class="sxs-lookup"><span data-stu-id="e68d7-114">tvRating</span></span>|[<span data-ttu-id="e68d7-115">ratingJapanTelevisionType</span><span class="sxs-lookup"><span data-stu-id="e68d7-115">ratingJapanTelevisionType</span></span>](../resources/intune-deviceconfig-ratingjapantelevisiontype.md)|<span data-ttu-id="e68d7-116">テレビの視聴制限が日本用に選択します。</span><span class="sxs-lookup"><span data-stu-id="e68d7-116">TV rating selected for Japan.</span></span> <span data-ttu-id="e68d7-117">可能な値は、`allAllowed`、`allBlocked`、`explicitAllowed` です。</span><span class="sxs-lookup"><span data-stu-id="e68d7-117">Possible values are: `allAllowed`, `allBlocked`, `explicitAllowed`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="e68d7-118">関係</span><span class="sxs-lookup"><span data-stu-id="e68d7-118">Relationships</span></span>
<span data-ttu-id="e68d7-119">なし</span><span class="sxs-lookup"><span data-stu-id="e68d7-119">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="e68d7-120">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="e68d7-120">JSON Representation</span></span>
<span data-ttu-id="e68d7-121">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="e68d7-121">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.mediaContentRatingJapan"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.mediaContentRatingJapan",
  "movieRating": "String",
  "tvRating": "String"
}
```



