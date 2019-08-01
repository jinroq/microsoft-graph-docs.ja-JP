---
title: mediaContentRatingIreland リソースの種類
description: まだ文書化されていません
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 9a36d4e56d4d101c5cdf0ba198a6b3ea17d11bd1
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "36028071"
---
# <a name="mediacontentratingireland-resource-type"></a><span data-ttu-id="1a5b1-103">mediaContentRatingIreland リソースの種類</span><span class="sxs-lookup"><span data-stu-id="1a5b1-103">mediaContentRatingIreland resource type</span></span>

> <span data-ttu-id="1a5b1-104">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="1a5b1-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="1a5b1-105">まだ文書化されていません</span><span class="sxs-lookup"><span data-stu-id="1a5b1-105">Not yet documented</span></span>

## <a name="properties"></a><span data-ttu-id="1a5b1-106">プロパティ</span><span class="sxs-lookup"><span data-stu-id="1a5b1-106">Properties</span></span>
|<span data-ttu-id="1a5b1-107">プロパティ</span><span class="sxs-lookup"><span data-stu-id="1a5b1-107">Property</span></span>|<span data-ttu-id="1a5b1-108">型</span><span class="sxs-lookup"><span data-stu-id="1a5b1-108">Type</span></span>|<span data-ttu-id="1a5b1-109">説明</span><span class="sxs-lookup"><span data-stu-id="1a5b1-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="1a5b1-110">movieRating</span><span class="sxs-lookup"><span data-stu-id="1a5b1-110">movieRating</span></span>|[<span data-ttu-id="1a5b1-111">ratingIrelandMoviesType</span><span class="sxs-lookup"><span data-stu-id="1a5b1-111">ratingIrelandMoviesType</span></span>](../resources/intune-deviceconfig-ratingirelandmoviestype.md)|<span data-ttu-id="1a5b1-112">アイルランド向けに選択されている映画のレーティング。</span><span class="sxs-lookup"><span data-stu-id="1a5b1-112">Movies rating selected for Ireland.</span></span> <span data-ttu-id="1a5b1-113">可能な値は、`allAllowed`、`allBlocked`、`general`、`parentalGuidance`、`agesAbove12`、`agesAbove15`、`agesAbove16`、`adults` です。</span><span class="sxs-lookup"><span data-stu-id="1a5b1-113">Possible values are: `allAllowed`, `allBlocked`, `general`, `parentalGuidance`, `agesAbove12`, `agesAbove15`, `agesAbove16`, `adults`.</span></span>|
|<span data-ttu-id="1a5b1-114">tvRating</span><span class="sxs-lookup"><span data-stu-id="1a5b1-114">tvRating</span></span>|[<span data-ttu-id="1a5b1-115">ratingIrelandTelevisionType</span><span class="sxs-lookup"><span data-stu-id="1a5b1-115">ratingIrelandTelevisionType</span></span>](../resources/intune-deviceconfig-ratingirelandtelevisiontype.md)|<span data-ttu-id="1a5b1-116">アイルランド向けに選択されているテレビのレーティング。</span><span class="sxs-lookup"><span data-stu-id="1a5b1-116">TV rating selected for Ireland.</span></span> <span data-ttu-id="1a5b1-117">可能な値は、`allAllowed`、`allBlocked`、`general`、`children`、`youngAdults`、`parentalSupervision`、`mature` です。</span><span class="sxs-lookup"><span data-stu-id="1a5b1-117">Possible values are: `allAllowed`, `allBlocked`, `general`, `children`, `youngAdults`, `parentalSupervision`, `mature`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="1a5b1-118">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="1a5b1-118">Relationships</span></span>
<span data-ttu-id="1a5b1-119">なし</span><span class="sxs-lookup"><span data-stu-id="1a5b1-119">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="1a5b1-120">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="1a5b1-120">JSON Representation</span></span>
<span data-ttu-id="1a5b1-121">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="1a5b1-121">Here is a JSON representation of the resource.</span></span>
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



