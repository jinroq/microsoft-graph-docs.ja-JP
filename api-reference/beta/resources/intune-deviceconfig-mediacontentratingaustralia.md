---
title: mediaContentRatingAustralia リソースの種類
description: まだ文書化されていません
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 259860387e005f7fe5bfd2d402be5c03ef21149f
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/23/2019
ms.locfileid: "29396638"
---
# <a name="mediacontentratingaustralia-resource-type"></a><span data-ttu-id="3d733-103">mediaContentRatingAustralia リソースの種類</span><span class="sxs-lookup"><span data-stu-id="3d733-103">mediaContentRatingAustralia resource type</span></span>

> <span data-ttu-id="3d733-104">**重要な:**[Microsoft Graph で/beta のバージョンの Api は予告なしに変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="3d733-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="3d733-105">実稼働アプリケーションでこれらの API を使用することは、サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="3d733-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="3d733-106">**注:** Intune の Microsoft グラフ API では、テナントの[Intune のアクティブなライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="3d733-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="3d733-107">まだ文書化されていません</span><span class="sxs-lookup"><span data-stu-id="3d733-107">Not yet documented</span></span>

## <a name="properties"></a><span data-ttu-id="3d733-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="3d733-108">Properties</span></span>
|<span data-ttu-id="3d733-109">プロパティ</span><span class="sxs-lookup"><span data-stu-id="3d733-109">Property</span></span>|<span data-ttu-id="3d733-110">型</span><span class="sxs-lookup"><span data-stu-id="3d733-110">Type</span></span>|<span data-ttu-id="3d733-111">説明</span><span class="sxs-lookup"><span data-stu-id="3d733-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="3d733-112">movieRating</span><span class="sxs-lookup"><span data-stu-id="3d733-112">movieRating</span></span>|[<span data-ttu-id="3d733-113">ratingAustraliaMoviesType</span><span class="sxs-lookup"><span data-stu-id="3d733-113">ratingAustraliaMoviesType</span></span>](../resources/intune-deviceconfig-ratingaustraliamoviestype.md)|<span data-ttu-id="3d733-114">評価のオーストラリアの選択したムービーです。</span><span class="sxs-lookup"><span data-stu-id="3d733-114">Movies rating selected for Australia.</span></span> <span data-ttu-id="3d733-115">可能な値は、`allAllowed`、`allBlocked`、`general`、`parentalGuidance`、`mature`、`agesAbove15`、`agesAbove18` です。</span><span class="sxs-lookup"><span data-stu-id="3d733-115">Possible values are: `allAllowed`, `allBlocked`, `general`, `parentalGuidance`, `mature`, `agesAbove15`, `agesAbove18`.</span></span>|
|<span data-ttu-id="3d733-116">tvRating</span><span class="sxs-lookup"><span data-stu-id="3d733-116">tvRating</span></span>|[<span data-ttu-id="3d733-117">ratingAustraliaTelevisionType</span><span class="sxs-lookup"><span data-stu-id="3d733-117">ratingAustraliaTelevisionType</span></span>](../resources/intune-deviceconfig-ratingaustraliatelevisiontype.md)|<span data-ttu-id="3d733-118">テレビの視聴制限がオーストラリアを選択します。</span><span class="sxs-lookup"><span data-stu-id="3d733-118">TV rating selected for Australia.</span></span> <span data-ttu-id="3d733-119">可能な値は、`allAllowed`、`allBlocked`、`preschoolers`、`children`、`general`、`parentalGuidance`、`mature`、`agesAbove15`、`agesAbove15AdultViolence` です。</span><span class="sxs-lookup"><span data-stu-id="3d733-119">Possible values are: `allAllowed`, `allBlocked`, `preschoolers`, `children`, `general`, `parentalGuidance`, `mature`, `agesAbove15`, `agesAbove15AdultViolence`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="3d733-120">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="3d733-120">Relationships</span></span>
<span data-ttu-id="3d733-121">なし</span><span class="sxs-lookup"><span data-stu-id="3d733-121">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="3d733-122">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="3d733-122">JSON Representation</span></span>
<span data-ttu-id="3d733-123">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="3d733-123">Here is a JSON representation of the resource.</span></span>
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




