---
title: mediaContentRatingIreland リソースの種類
description: まだ文書化されていません
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: f497922920ab6826bf11ad0ed78234d2c180f7a7
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "36000808"
---
# <a name="mediacontentratingireland-resource-type"></a><span data-ttu-id="82c21-103">mediaContentRatingIreland リソースの種類</span><span class="sxs-lookup"><span data-stu-id="82c21-103">mediaContentRatingIreland resource type</span></span>

> <span data-ttu-id="82c21-104">**重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="82c21-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="82c21-105">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="82c21-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="82c21-106">まだ文書化されていません</span><span class="sxs-lookup"><span data-stu-id="82c21-106">Not yet documented</span></span>

## <a name="properties"></a><span data-ttu-id="82c21-107">プロパティ</span><span class="sxs-lookup"><span data-stu-id="82c21-107">Properties</span></span>
|<span data-ttu-id="82c21-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="82c21-108">Property</span></span>|<span data-ttu-id="82c21-109">型</span><span class="sxs-lookup"><span data-stu-id="82c21-109">Type</span></span>|<span data-ttu-id="82c21-110">説明</span><span class="sxs-lookup"><span data-stu-id="82c21-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="82c21-111">movieRating</span><span class="sxs-lookup"><span data-stu-id="82c21-111">movieRating</span></span>|[<span data-ttu-id="82c21-112">ratingIrelandMoviesType</span><span class="sxs-lookup"><span data-stu-id="82c21-112">ratingIrelandMoviesType</span></span>](../resources/intune-deviceconfig-ratingirelandmoviestype.md)|<span data-ttu-id="82c21-113">アイルランド向けに選択されている映画のレーティング。</span><span class="sxs-lookup"><span data-stu-id="82c21-113">Movies rating selected for Ireland.</span></span> <span data-ttu-id="82c21-114">可能な値は、`allAllowed`、`allBlocked`、`general`、`parentalGuidance`、`agesAbove12`、`agesAbove15`、`agesAbove16`、`adults` です。</span><span class="sxs-lookup"><span data-stu-id="82c21-114">Possible values are: `allAllowed`, `allBlocked`, `general`, `parentalGuidance`, `agesAbove12`, `agesAbove15`, `agesAbove16`, `adults`.</span></span>|
|<span data-ttu-id="82c21-115">tvRating</span><span class="sxs-lookup"><span data-stu-id="82c21-115">tvRating</span></span>|[<span data-ttu-id="82c21-116">ratingIrelandTelevisionType</span><span class="sxs-lookup"><span data-stu-id="82c21-116">ratingIrelandTelevisionType</span></span>](../resources/intune-deviceconfig-ratingirelandtelevisiontype.md)|<span data-ttu-id="82c21-117">アイルランド向けに選択されているテレビのレーティング。</span><span class="sxs-lookup"><span data-stu-id="82c21-117">TV rating selected for Ireland.</span></span> <span data-ttu-id="82c21-118">可能な値は、`allAllowed`、`allBlocked`、`general`、`children`、`youngAdults`、`parentalSupervision`、`mature` です。</span><span class="sxs-lookup"><span data-stu-id="82c21-118">Possible values are: `allAllowed`, `allBlocked`, `general`, `children`, `youngAdults`, `parentalSupervision`, `mature`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="82c21-119">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="82c21-119">Relationships</span></span>
<span data-ttu-id="82c21-120">なし</span><span class="sxs-lookup"><span data-stu-id="82c21-120">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="82c21-121">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="82c21-121">JSON Representation</span></span>
<span data-ttu-id="82c21-122">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="82c21-122">Here is a JSON representation of the resource.</span></span>
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





