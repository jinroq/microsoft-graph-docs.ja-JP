---
title: mediaContentRatingUnitedKingdom リソースの種類
description: まだ文書化されていません
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 947fd12d8219215b0828ef1c05d2d8b36f970f16
ms.sourcegitcommit: 873b99d9001d1b2af21836e47f15360b08e10a40
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 02/26/2019
ms.locfileid: "30252456"
---
# <a name="mediacontentratingunitedkingdom-resource-type"></a><span data-ttu-id="9322b-103">mediaContentRatingUnitedKingdom リソースの種類</span><span class="sxs-lookup"><span data-stu-id="9322b-103">mediaContentRatingUnitedKingdom resource type</span></span>

> <span data-ttu-id="9322b-104">**注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="9322b-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="9322b-105">まだ文書化されていません</span><span class="sxs-lookup"><span data-stu-id="9322b-105">Not yet documented</span></span>

## <a name="properties"></a><span data-ttu-id="9322b-106">プロパティ</span><span class="sxs-lookup"><span data-stu-id="9322b-106">Properties</span></span>
|<span data-ttu-id="9322b-107">プロパティ</span><span class="sxs-lookup"><span data-stu-id="9322b-107">Property</span></span>|<span data-ttu-id="9322b-108">型</span><span class="sxs-lookup"><span data-stu-id="9322b-108">Type</span></span>|<span data-ttu-id="9322b-109">説明</span><span class="sxs-lookup"><span data-stu-id="9322b-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="9322b-110">movieRating</span><span class="sxs-lookup"><span data-stu-id="9322b-110">movieRating</span></span>|[<span data-ttu-id="9322b-111">ratingUnitedKingdomMoviesType</span><span class="sxs-lookup"><span data-stu-id="9322b-111">ratingUnitedKingdomMoviesType</span></span>](../resources/intune-deviceconfig-ratingunitedkingdommoviestype.md)|<span data-ttu-id="9322b-112">英国向けに選択されている映画のレーティング。</span><span class="sxs-lookup"><span data-stu-id="9322b-112">Movies rating selected for United Kingdom.</span></span> <span data-ttu-id="9322b-113">可能な値は、`allAllowed`、`allBlocked`、`general`、`universalChildren`、`parentalGuidance`、`agesAbove12Video`、`agesAbove12Cinema`、`agesAbove15`、`adults` です。</span><span class="sxs-lookup"><span data-stu-id="9322b-113">Possible values are: `allAllowed`, `allBlocked`, `general`, `universalChildren`, `parentalGuidance`, `agesAbove12Video`, `agesAbove12Cinema`, `agesAbove15`, `adults`.</span></span>|
|<span data-ttu-id="9322b-114">tvRating</span><span class="sxs-lookup"><span data-stu-id="9322b-114">tvRating</span></span>|[<span data-ttu-id="9322b-115">ratingUnitedKingdomTelevisionType</span><span class="sxs-lookup"><span data-stu-id="9322b-115">ratingUnitedKingdomTelevisionType</span></span>](../resources/intune-deviceconfig-ratingunitedkingdomtelevisiontype.md)|<span data-ttu-id="9322b-116">英国向けに選択されているテレビのレーティング。</span><span class="sxs-lookup"><span data-stu-id="9322b-116">TV rating selected for United Kingdom.</span></span> <span data-ttu-id="9322b-117">可能な値は、`allAllowed`、`allBlocked`、`caution` です。</span><span class="sxs-lookup"><span data-stu-id="9322b-117">Possible values are: `allAllowed`, `allBlocked`, `caution`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="9322b-118">関係</span><span class="sxs-lookup"><span data-stu-id="9322b-118">Relationships</span></span>
<span data-ttu-id="9322b-119">なし</span><span class="sxs-lookup"><span data-stu-id="9322b-119">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="9322b-120">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="9322b-120">JSON Representation</span></span>
<span data-ttu-id="9322b-121">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="9322b-121">Here is a JSON representation of the resource.</span></span>
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



