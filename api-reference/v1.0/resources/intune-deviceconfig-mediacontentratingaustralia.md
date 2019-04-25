---
title: mediaContentRatingAustralia リソースの種類
description: まだ文書化されていません
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 37e42c3629e73d8dc629ba754583f8023c168b30
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32572375"
---
# <a name="mediacontentratingaustralia-resource-type"></a><span data-ttu-id="d30f7-103">mediaContentRatingAustralia リソースの種類</span><span class="sxs-lookup"><span data-stu-id="d30f7-103">mediaContentRatingAustralia resource type</span></span>

> <span data-ttu-id="d30f7-104">**注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="d30f7-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="d30f7-105">まだ文書化されていません</span><span class="sxs-lookup"><span data-stu-id="d30f7-105">Not yet documented</span></span>

## <a name="properties"></a><span data-ttu-id="d30f7-106">プロパティ</span><span class="sxs-lookup"><span data-stu-id="d30f7-106">Properties</span></span>
|<span data-ttu-id="d30f7-107">プロパティ</span><span class="sxs-lookup"><span data-stu-id="d30f7-107">Property</span></span>|<span data-ttu-id="d30f7-108">型</span><span class="sxs-lookup"><span data-stu-id="d30f7-108">Type</span></span>|<span data-ttu-id="d30f7-109">説明</span><span class="sxs-lookup"><span data-stu-id="d30f7-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d30f7-110">movieRating</span><span class="sxs-lookup"><span data-stu-id="d30f7-110">movieRating</span></span>|[<span data-ttu-id="d30f7-111">ratingAustraliaMoviesType</span><span class="sxs-lookup"><span data-stu-id="d30f7-111">ratingAustraliaMoviesType</span></span>](../resources/intune-deviceconfig-ratingaustraliamoviestype.md)|<span data-ttu-id="d30f7-112">オーストラリア向けに選択されている映画のレーティング。</span><span class="sxs-lookup"><span data-stu-id="d30f7-112">Movies rating selected for Australia.</span></span> <span data-ttu-id="d30f7-113">可能な値は、`allAllowed`、`allBlocked`、`general`、`parentalGuidance`、`mature`、`agesAbove15`、`agesAbove18` です。</span><span class="sxs-lookup"><span data-stu-id="d30f7-113">Possible values are: `allAllowed`, `allBlocked`, `general`, `parentalGuidance`, `mature`, `agesAbove15`, `agesAbove18`.</span></span>|
|<span data-ttu-id="d30f7-114">tvRating</span><span class="sxs-lookup"><span data-stu-id="d30f7-114">tvRating</span></span>|[<span data-ttu-id="d30f7-115">ratingAustraliaTelevisionType</span><span class="sxs-lookup"><span data-stu-id="d30f7-115">ratingAustraliaTelevisionType</span></span>](../resources/intune-deviceconfig-ratingaustraliatelevisiontype.md)|<span data-ttu-id="d30f7-116">オーストラリア向けに選択されているテレビのレーティング。</span><span class="sxs-lookup"><span data-stu-id="d30f7-116">TV rating selected for Australia.</span></span> <span data-ttu-id="d30f7-117">可能な値は、`allAllowed`、`allBlocked`、`preschoolers`、`children`、`general`、`parentalGuidance`、`mature`、`agesAbove15`、`agesAbove15AdultViolence` です。</span><span class="sxs-lookup"><span data-stu-id="d30f7-117">Possible values are: `allAllowed`, `allBlocked`, `preschoolers`, `children`, `general`, `parentalGuidance`, `mature`, `agesAbove15`, `agesAbove15AdultViolence`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="d30f7-118">関係</span><span class="sxs-lookup"><span data-stu-id="d30f7-118">Relationships</span></span>
<span data-ttu-id="d30f7-119">なし</span><span class="sxs-lookup"><span data-stu-id="d30f7-119">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="d30f7-120">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="d30f7-120">JSON Representation</span></span>
<span data-ttu-id="d30f7-121">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="d30f7-121">Here is a JSON representation of the resource.</span></span>
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



