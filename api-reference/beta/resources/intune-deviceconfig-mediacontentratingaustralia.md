---
title: mediaContentRatingAustralia リソースの種類
description: まだ文書化されていません
author: tfitzmac
ms.openlocfilehash: 29501d5e52b922baabd777a8838896230a502631
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 12/18/2018
ms.locfileid: "27317165"
---
# <a name="mediacontentratingaustralia-resource-type"></a><span data-ttu-id="dd922-103">mediaContentRatingAustralia リソースの種類</span><span class="sxs-lookup"><span data-stu-id="dd922-103">mediaContentRatingAustralia resource type</span></span>

> <span data-ttu-id="dd922-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="dd922-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="dd922-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="dd922-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="dd922-106">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="dd922-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="dd922-107">まだ文書化されていません</span><span class="sxs-lookup"><span data-stu-id="dd922-107">Not yet documented</span></span>
## <a name="properties"></a><span data-ttu-id="dd922-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="dd922-108">Properties</span></span>
|<span data-ttu-id="dd922-109">プロパティ</span><span class="sxs-lookup"><span data-stu-id="dd922-109">Property</span></span>|<span data-ttu-id="dd922-110">種類</span><span class="sxs-lookup"><span data-stu-id="dd922-110">Type</span></span>|<span data-ttu-id="dd922-111">説明</span><span class="sxs-lookup"><span data-stu-id="dd922-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="dd922-112">movieRating</span><span class="sxs-lookup"><span data-stu-id="dd922-112">movieRating</span></span>|[<span data-ttu-id="dd922-113">ratingAustraliaMoviesType</span><span class="sxs-lookup"><span data-stu-id="dd922-113">ratingAustraliaMoviesType</span></span>](../resources/intune-deviceconfig-ratingaustraliamoviestype.md)|<span data-ttu-id="dd922-114">評価のオーストラリアの選択したムービーです。</span><span class="sxs-lookup"><span data-stu-id="dd922-114">Movies rating selected for Australia.</span></span> <span data-ttu-id="dd922-115">可能な値は、`allAllowed`、`allBlocked`、`general`、`parentalGuidance`、`mature`、`agesAbove15`、`agesAbove18` です。</span><span class="sxs-lookup"><span data-stu-id="dd922-115">Possible values are: `allAllowed`, `allBlocked`, `general`, `parentalGuidance`, `mature`, `agesAbove15`, `agesAbove18`.</span></span>|
|<span data-ttu-id="dd922-116">tvRating</span><span class="sxs-lookup"><span data-stu-id="dd922-116">tvRating</span></span>|[<span data-ttu-id="dd922-117">ratingAustraliaTelevisionType</span><span class="sxs-lookup"><span data-stu-id="dd922-117">ratingAustraliaTelevisionType</span></span>](../resources/intune-deviceconfig-ratingaustraliatelevisiontype.md)|<span data-ttu-id="dd922-118">テレビの視聴制限がオーストラリアを選択します。</span><span class="sxs-lookup"><span data-stu-id="dd922-118">TV rating selected for Australia.</span></span> <span data-ttu-id="dd922-119">可能な値は、`allAllowed`、`allBlocked`、`preschoolers`、`children`、`general`、`parentalGuidance`、`mature`、`agesAbove15`、`agesAbove15AdultViolence` です。</span><span class="sxs-lookup"><span data-stu-id="dd922-119">Possible values are: `allAllowed`, `allBlocked`, `preschoolers`, `children`, `general`, `parentalGuidance`, `mature`, `agesAbove15`, `agesAbove15AdultViolence`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="dd922-120">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="dd922-120">Relationships</span></span>
<span data-ttu-id="dd922-121">なし</span><span class="sxs-lookup"><span data-stu-id="dd922-121">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="dd922-122">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="dd922-122">JSON Representation</span></span>
<span data-ttu-id="dd922-123">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="dd922-123">Here is a JSON representation of the resource.</span></span>
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





