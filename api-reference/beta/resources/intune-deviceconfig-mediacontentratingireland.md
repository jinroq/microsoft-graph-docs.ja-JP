---
title: mediaContentRatingIreland リソースの種類
description: まだ文書化されていません
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: b3efd96cc8ad015989365dff10b1659ef50c4fb7
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/23/2019
ms.locfileid: "29422601"
---
# <a name="mediacontentratingireland-resource-type"></a><span data-ttu-id="bfa59-103">mediaContentRatingIreland リソースの種類</span><span class="sxs-lookup"><span data-stu-id="bfa59-103">mediaContentRatingIreland resource type</span></span>

> <span data-ttu-id="bfa59-104">**重要な:**[Microsoft Graph で/beta のバージョンの Api は予告なしに変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="bfa59-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="bfa59-105">実稼働アプリケーションでこれらの API を使用することは、サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="bfa59-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="bfa59-106">**注:** Intune の Microsoft グラフ API では、テナントの[Intune のアクティブなライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="bfa59-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="bfa59-107">まだ文書化されていません</span><span class="sxs-lookup"><span data-stu-id="bfa59-107">Not yet documented</span></span>

## <a name="properties"></a><span data-ttu-id="bfa59-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="bfa59-108">Properties</span></span>
|<span data-ttu-id="bfa59-109">プロパティ</span><span class="sxs-lookup"><span data-stu-id="bfa59-109">Property</span></span>|<span data-ttu-id="bfa59-110">型</span><span class="sxs-lookup"><span data-stu-id="bfa59-110">Type</span></span>|<span data-ttu-id="bfa59-111">説明</span><span class="sxs-lookup"><span data-stu-id="bfa59-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="bfa59-112">movieRating</span><span class="sxs-lookup"><span data-stu-id="bfa59-112">movieRating</span></span>|[<span data-ttu-id="bfa59-113">ratingIrelandMoviesType</span><span class="sxs-lookup"><span data-stu-id="bfa59-113">ratingIrelandMoviesType</span></span>](../resources/intune-deviceconfig-ratingirelandmoviestype.md)|<span data-ttu-id="bfa59-114">評価のアイルランドの選択したムービーです。</span><span class="sxs-lookup"><span data-stu-id="bfa59-114">Movies rating selected for Ireland.</span></span> <span data-ttu-id="bfa59-115">可能な値は、`allAllowed`、`allBlocked`、`general`、`parentalGuidance`、`agesAbove12`、`agesAbove15`、`agesAbove16`、`adults` です。</span><span class="sxs-lookup"><span data-stu-id="bfa59-115">Possible values are: `allAllowed`, `allBlocked`, `general`, `parentalGuidance`, `agesAbove12`, `agesAbove15`, `agesAbove16`, `adults`.</span></span>|
|<span data-ttu-id="bfa59-116">tvRating</span><span class="sxs-lookup"><span data-stu-id="bfa59-116">tvRating</span></span>|[<span data-ttu-id="bfa59-117">ratingIrelandTelevisionType</span><span class="sxs-lookup"><span data-stu-id="bfa59-117">ratingIrelandTelevisionType</span></span>](../resources/intune-deviceconfig-ratingirelandtelevisiontype.md)|<span data-ttu-id="bfa59-118">テレビの視聴制限はアイルランドのために選択します。</span><span class="sxs-lookup"><span data-stu-id="bfa59-118">TV rating selected for Ireland.</span></span> <span data-ttu-id="bfa59-119">可能な値は、`allAllowed`、`allBlocked`、`general`、`children`、`youngAdults`、`parentalSupervision`、`mature` です。</span><span class="sxs-lookup"><span data-stu-id="bfa59-119">Possible values are: `allAllowed`, `allBlocked`, `general`, `children`, `youngAdults`, `parentalSupervision`, `mature`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="bfa59-120">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="bfa59-120">Relationships</span></span>
<span data-ttu-id="bfa59-121">なし</span><span class="sxs-lookup"><span data-stu-id="bfa59-121">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="bfa59-122">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="bfa59-122">JSON Representation</span></span>
<span data-ttu-id="bfa59-123">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="bfa59-123">Here is a JSON representation of the resource.</span></span>
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




