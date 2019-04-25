---
title: mediaContentRatingIreland リソースの種類
description: まだ文書化されていません
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 153164010b6beda5d38779f67ffcd0654a1c986a
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32572361"
---
# <a name="mediacontentratingireland-resource-type"></a><span data-ttu-id="2085b-103">mediaContentRatingIreland リソースの種類</span><span class="sxs-lookup"><span data-stu-id="2085b-103">mediaContentRatingIreland resource type</span></span>

> <span data-ttu-id="2085b-104">**注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="2085b-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="2085b-105">まだ文書化されていません</span><span class="sxs-lookup"><span data-stu-id="2085b-105">Not yet documented</span></span>

## <a name="properties"></a><span data-ttu-id="2085b-106">プロパティ</span><span class="sxs-lookup"><span data-stu-id="2085b-106">Properties</span></span>
|<span data-ttu-id="2085b-107">プロパティ</span><span class="sxs-lookup"><span data-stu-id="2085b-107">Property</span></span>|<span data-ttu-id="2085b-108">型</span><span class="sxs-lookup"><span data-stu-id="2085b-108">Type</span></span>|<span data-ttu-id="2085b-109">説明</span><span class="sxs-lookup"><span data-stu-id="2085b-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="2085b-110">movieRating</span><span class="sxs-lookup"><span data-stu-id="2085b-110">movieRating</span></span>|[<span data-ttu-id="2085b-111">ratingIrelandMoviesType</span><span class="sxs-lookup"><span data-stu-id="2085b-111">ratingIrelandMoviesType</span></span>](../resources/intune-deviceconfig-ratingirelandmoviestype.md)|<span data-ttu-id="2085b-112">アイルランド向けに選択されている映画のレーティング。</span><span class="sxs-lookup"><span data-stu-id="2085b-112">Movies rating selected for Ireland.</span></span> <span data-ttu-id="2085b-113">可能な値は、`allAllowed`、`allBlocked`、`general`、`parentalGuidance`、`agesAbove12`、`agesAbove15`、`agesAbove16`、`adults` です。</span><span class="sxs-lookup"><span data-stu-id="2085b-113">Possible values are: `allAllowed`, `allBlocked`, `general`, `parentalGuidance`, `agesAbove12`, `agesAbove15`, `agesAbove16`, `adults`.</span></span>|
|<span data-ttu-id="2085b-114">tvRating</span><span class="sxs-lookup"><span data-stu-id="2085b-114">tvRating</span></span>|[<span data-ttu-id="2085b-115">ratingIrelandTelevisionType</span><span class="sxs-lookup"><span data-stu-id="2085b-115">ratingIrelandTelevisionType</span></span>](../resources/intune-deviceconfig-ratingirelandtelevisiontype.md)|<span data-ttu-id="2085b-116">アイルランド向けに選択されているテレビのレーティング。</span><span class="sxs-lookup"><span data-stu-id="2085b-116">TV rating selected for Ireland.</span></span> <span data-ttu-id="2085b-117">可能な値は、`allAllowed`、`allBlocked`、`general`、`children`、`youngAdults`、`parentalSupervision`、`mature` です。</span><span class="sxs-lookup"><span data-stu-id="2085b-117">Possible values are: `allAllowed`, `allBlocked`, `general`, `children`, `youngAdults`, `parentalSupervision`, `mature`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="2085b-118">関係</span><span class="sxs-lookup"><span data-stu-id="2085b-118">Relationships</span></span>
<span data-ttu-id="2085b-119">なし</span><span class="sxs-lookup"><span data-stu-id="2085b-119">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="2085b-120">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="2085b-120">JSON Representation</span></span>
<span data-ttu-id="2085b-121">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="2085b-121">Here is a JSON representation of the resource.</span></span>
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



