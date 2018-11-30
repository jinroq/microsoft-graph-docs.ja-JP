---
title: mediaContentRatingIreland リソースの種類
description: まだ文書化されていません
ms.openlocfilehash: b4348e6f73730d59e6e67b3e102b9ad9caa98add
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27020532"
---
# <a name="mediacontentratingireland-resource-type"></a><span data-ttu-id="31b38-103">mediaContentRatingIreland リソースの種類</span><span class="sxs-lookup"><span data-stu-id="31b38-103">mediaContentRatingIreland resource type</span></span>

> <span data-ttu-id="31b38-104">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="31b38-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="31b38-105">まだ文書化されていません</span><span class="sxs-lookup"><span data-stu-id="31b38-105">Not yet documented</span></span>
## <a name="properties"></a><span data-ttu-id="31b38-106">プロパティ</span><span class="sxs-lookup"><span data-stu-id="31b38-106">Properties</span></span>
|<span data-ttu-id="31b38-107">プロパティ</span><span class="sxs-lookup"><span data-stu-id="31b38-107">Property</span></span>|<span data-ttu-id="31b38-108">型</span><span class="sxs-lookup"><span data-stu-id="31b38-108">Type</span></span>|<span data-ttu-id="31b38-109">説明</span><span class="sxs-lookup"><span data-stu-id="31b38-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="31b38-110">movieRating</span><span class="sxs-lookup"><span data-stu-id="31b38-110">movieRating</span></span>|[<span data-ttu-id="31b38-111">ratingIrelandMoviesType</span><span class="sxs-lookup"><span data-stu-id="31b38-111">ratingIrelandMoviesType</span></span>](../resources/intune-deviceconfig-ratingirelandmoviestype.md)|<span data-ttu-id="31b38-112">評価のアイルランドの選択したムービーです。</span><span class="sxs-lookup"><span data-stu-id="31b38-112">Movies rating selected for Ireland.</span></span> <span data-ttu-id="31b38-113">可能な値は、`allAllowed`、`allBlocked`、`general`、`parentalGuidance`、`agesAbove12`、`agesAbove15`、`agesAbove16`、`adults` です。</span><span class="sxs-lookup"><span data-stu-id="31b38-113">Possible values are: `allAllowed`, `allBlocked`, `general`, `parentalGuidance`, `agesAbove12`, `agesAbove15`, `agesAbove16`, `adults`.</span></span>|
|<span data-ttu-id="31b38-114">tvRating</span><span class="sxs-lookup"><span data-stu-id="31b38-114">tvRating</span></span>|[<span data-ttu-id="31b38-115">ratingIrelandTelevisionType</span><span class="sxs-lookup"><span data-stu-id="31b38-115">ratingIrelandTelevisionType</span></span>](../resources/intune-deviceconfig-ratingirelandtelevisiontype.md)|<span data-ttu-id="31b38-116">テレビの視聴制限はアイルランドのために選択します。</span><span class="sxs-lookup"><span data-stu-id="31b38-116">TV rating selected for Ireland.</span></span> <span data-ttu-id="31b38-117">可能な値は、`allAllowed`、`allBlocked`、`general`、`children`、`youngAdults`、`parentalSupervision`、`mature` です。</span><span class="sxs-lookup"><span data-stu-id="31b38-117">Possible values are: `allAllowed`, `allBlocked`, `general`, `children`, `youngAdults`, `parentalSupervision`, `mature`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="31b38-118">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="31b38-118">Relationships</span></span>
<span data-ttu-id="31b38-119">なし</span><span class="sxs-lookup"><span data-stu-id="31b38-119">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="31b38-120">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="31b38-120">JSON Representation</span></span>
<span data-ttu-id="31b38-121">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="31b38-121">Here is a JSON representation of the resource.</span></span>
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



