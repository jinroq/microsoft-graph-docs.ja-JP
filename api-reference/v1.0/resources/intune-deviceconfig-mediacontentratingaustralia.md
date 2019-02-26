---
title: mediaContentRatingAustralia リソースの種類
description: まだ文書化されていません
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 37e42c3629e73d8dc629ba754583f8023c168b30
ms.sourcegitcommit: 873b99d9001d1b2af21836e47f15360b08e10a40
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 02/26/2019
ms.locfileid: "30259116"
---
# <a name="mediacontentratingaustralia-resource-type"></a><span data-ttu-id="6effc-103">mediaContentRatingAustralia リソースの種類</span><span class="sxs-lookup"><span data-stu-id="6effc-103">mediaContentRatingAustralia resource type</span></span>

> <span data-ttu-id="6effc-104">**注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="6effc-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="6effc-105">まだ文書化されていません</span><span class="sxs-lookup"><span data-stu-id="6effc-105">Not yet documented</span></span>

## <a name="properties"></a><span data-ttu-id="6effc-106">プロパティ</span><span class="sxs-lookup"><span data-stu-id="6effc-106">Properties</span></span>
|<span data-ttu-id="6effc-107">プロパティ</span><span class="sxs-lookup"><span data-stu-id="6effc-107">Property</span></span>|<span data-ttu-id="6effc-108">型</span><span class="sxs-lookup"><span data-stu-id="6effc-108">Type</span></span>|<span data-ttu-id="6effc-109">説明</span><span class="sxs-lookup"><span data-stu-id="6effc-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="6effc-110">movieRating</span><span class="sxs-lookup"><span data-stu-id="6effc-110">movieRating</span></span>|[<span data-ttu-id="6effc-111">ratingAustraliaMoviesType</span><span class="sxs-lookup"><span data-stu-id="6effc-111">ratingAustraliaMoviesType</span></span>](../resources/intune-deviceconfig-ratingaustraliamoviestype.md)|<span data-ttu-id="6effc-112">オーストラリア向けに選択されている映画のレーティング。</span><span class="sxs-lookup"><span data-stu-id="6effc-112">Movies rating selected for Australia.</span></span> <span data-ttu-id="6effc-113">可能な値は、`allAllowed`、`allBlocked`、`general`、`parentalGuidance`、`mature`、`agesAbove15`、`agesAbove18` です。</span><span class="sxs-lookup"><span data-stu-id="6effc-113">Possible values are: `allAllowed`, `allBlocked`, `general`, `parentalGuidance`, `mature`, `agesAbove15`, `agesAbove18`.</span></span>|
|<span data-ttu-id="6effc-114">tvRating</span><span class="sxs-lookup"><span data-stu-id="6effc-114">tvRating</span></span>|[<span data-ttu-id="6effc-115">ratingAustraliaTelevisionType</span><span class="sxs-lookup"><span data-stu-id="6effc-115">ratingAustraliaTelevisionType</span></span>](../resources/intune-deviceconfig-ratingaustraliatelevisiontype.md)|<span data-ttu-id="6effc-116">オーストラリア向けに選択されているテレビのレーティング。</span><span class="sxs-lookup"><span data-stu-id="6effc-116">TV rating selected for Australia.</span></span> <span data-ttu-id="6effc-117">可能な値は、`allAllowed`、`allBlocked`、`preschoolers`、`children`、`general`、`parentalGuidance`、`mature`、`agesAbove15`、`agesAbove15AdultViolence` です。</span><span class="sxs-lookup"><span data-stu-id="6effc-117">Possible values are: `allAllowed`, `allBlocked`, `preschoolers`, `children`, `general`, `parentalGuidance`, `mature`, `agesAbove15`, `agesAbove15AdultViolence`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="6effc-118">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="6effc-118">Relationships</span></span>
<span data-ttu-id="6effc-119">なし</span><span class="sxs-lookup"><span data-stu-id="6effc-119">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="6effc-120">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="6effc-120">JSON Representation</span></span>
<span data-ttu-id="6effc-121">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="6effc-121">Here is a JSON representation of the resource.</span></span>
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



