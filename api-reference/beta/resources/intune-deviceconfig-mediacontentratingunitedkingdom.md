---
title: mediaContentRatingUnitedKingdom リソースの種類
description: まだ文書化されていません
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 7d21ac4650072c4523f9e120d5d73ad393686635
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/23/2019
ms.locfileid: "29408076"
---
# <a name="mediacontentratingunitedkingdom-resource-type"></a><span data-ttu-id="0517e-103">mediaContentRatingUnitedKingdom リソースの種類</span><span class="sxs-lookup"><span data-stu-id="0517e-103">mediaContentRatingUnitedKingdom resource type</span></span>

> <span data-ttu-id="0517e-104">**重要な:**[Microsoft Graph で/beta のバージョンの Api は予告なしに変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="0517e-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="0517e-105">実稼働アプリケーションでこれらの API を使用することは、サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="0517e-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="0517e-106">**注:** Intune の Microsoft グラフ API では、テナントの[Intune のアクティブなライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="0517e-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="0517e-107">まだ文書化されていません</span><span class="sxs-lookup"><span data-stu-id="0517e-107">Not yet documented</span></span>

## <a name="properties"></a><span data-ttu-id="0517e-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="0517e-108">Properties</span></span>
|<span data-ttu-id="0517e-109">プロパティ</span><span class="sxs-lookup"><span data-stu-id="0517e-109">Property</span></span>|<span data-ttu-id="0517e-110">型</span><span class="sxs-lookup"><span data-stu-id="0517e-110">Type</span></span>|<span data-ttu-id="0517e-111">説明</span><span class="sxs-lookup"><span data-stu-id="0517e-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="0517e-112">movieRating</span><span class="sxs-lookup"><span data-stu-id="0517e-112">movieRating</span></span>|[<span data-ttu-id="0517e-113">ratingUnitedKingdomMoviesType</span><span class="sxs-lookup"><span data-stu-id="0517e-113">ratingUnitedKingdomMoviesType</span></span>](../resources/intune-deviceconfig-ratingunitedkingdommoviestype.md)|<span data-ttu-id="0517e-114">評価の英国を選択したムービーです。</span><span class="sxs-lookup"><span data-stu-id="0517e-114">Movies rating selected for United Kingdom.</span></span> <span data-ttu-id="0517e-115">可能な値は、`allAllowed`、`allBlocked`、`general`、`universalChildren`、`parentalGuidance`、`agesAbove12Video`、`agesAbove12Cinema`、`agesAbove15`、`adults` です。</span><span class="sxs-lookup"><span data-stu-id="0517e-115">Possible values are: `allAllowed`, `allBlocked`, `general`, `universalChildren`, `parentalGuidance`, `agesAbove12Video`, `agesAbove12Cinema`, `agesAbove15`, `adults`.</span></span>|
|<span data-ttu-id="0517e-116">tvRating</span><span class="sxs-lookup"><span data-stu-id="0517e-116">tvRating</span></span>|[<span data-ttu-id="0517e-117">ratingUnitedKingdomTelevisionType</span><span class="sxs-lookup"><span data-stu-id="0517e-117">ratingUnitedKingdomTelevisionType</span></span>](../resources/intune-deviceconfig-ratingunitedkingdomtelevisiontype.md)|<span data-ttu-id="0517e-118">テレビの視聴制限が英国を選択します。</span><span class="sxs-lookup"><span data-stu-id="0517e-118">TV rating selected for United Kingdom.</span></span> <span data-ttu-id="0517e-119">可能な値は、`allAllowed`、`allBlocked`、`caution` です。</span><span class="sxs-lookup"><span data-stu-id="0517e-119">Possible values are: `allAllowed`, `allBlocked`, `caution`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="0517e-120">関係</span><span class="sxs-lookup"><span data-stu-id="0517e-120">Relationships</span></span>
<span data-ttu-id="0517e-121">なし</span><span class="sxs-lookup"><span data-stu-id="0517e-121">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="0517e-122">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="0517e-122">JSON Representation</span></span>
<span data-ttu-id="0517e-123">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="0517e-123">Here is a JSON representation of the resource.</span></span>
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




