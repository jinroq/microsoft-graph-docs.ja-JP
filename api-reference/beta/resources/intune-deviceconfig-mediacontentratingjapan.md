---
title: mediaContentRatingJapan リソースの種類
description: まだ文書化されていません
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 1c129fb2853025758fc71aff381efe500d38ec8f
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/23/2019
ms.locfileid: "29394839"
---
# <a name="mediacontentratingjapan-resource-type"></a><span data-ttu-id="8740a-103">mediaContentRatingJapan リソースの種類</span><span class="sxs-lookup"><span data-stu-id="8740a-103">mediaContentRatingJapan resource type</span></span>

> <span data-ttu-id="8740a-104">**重要な:**[Microsoft Graph で/beta のバージョンの Api は予告なしに変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="8740a-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="8740a-105">実稼働アプリケーションでこれらの API を使用することは、サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="8740a-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="8740a-106">**注:** Intune の Microsoft グラフ API では、テナントの[Intune のアクティブなライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="8740a-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="8740a-107">まだ文書化されていません</span><span class="sxs-lookup"><span data-stu-id="8740a-107">Not yet documented</span></span>

## <a name="properties"></a><span data-ttu-id="8740a-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="8740a-108">Properties</span></span>
|<span data-ttu-id="8740a-109">プロパティ</span><span class="sxs-lookup"><span data-stu-id="8740a-109">Property</span></span>|<span data-ttu-id="8740a-110">型</span><span class="sxs-lookup"><span data-stu-id="8740a-110">Type</span></span>|<span data-ttu-id="8740a-111">説明</span><span class="sxs-lookup"><span data-stu-id="8740a-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="8740a-112">movieRating</span><span class="sxs-lookup"><span data-stu-id="8740a-112">movieRating</span></span>|[<span data-ttu-id="8740a-113">ratingJapanMoviesType</span><span class="sxs-lookup"><span data-stu-id="8740a-113">ratingJapanMoviesType</span></span>](../resources/intune-deviceconfig-ratingjapanmoviestype.md)|<span data-ttu-id="8740a-114">評価日本の選択したムービーです。</span><span class="sxs-lookup"><span data-stu-id="8740a-114">Movies rating selected for Japan.</span></span> <span data-ttu-id="8740a-115">使用可能な値: `allAllowed`、`allBlocked`、`general`、`parentalGuidance`、`agesAbove15`、`agesAbove18`。</span><span class="sxs-lookup"><span data-stu-id="8740a-115">Possible values are: `allAllowed`, `allBlocked`, `general`, `parentalGuidance`, `agesAbove15`, `agesAbove18`.</span></span>|
|<span data-ttu-id="8740a-116">tvRating</span><span class="sxs-lookup"><span data-stu-id="8740a-116">tvRating</span></span>|[<span data-ttu-id="8740a-117">ratingJapanTelevisionType</span><span class="sxs-lookup"><span data-stu-id="8740a-117">ratingJapanTelevisionType</span></span>](../resources/intune-deviceconfig-ratingjapantelevisiontype.md)|<span data-ttu-id="8740a-118">テレビの視聴制限が日本用に選択します。</span><span class="sxs-lookup"><span data-stu-id="8740a-118">TV rating selected for Japan.</span></span> <span data-ttu-id="8740a-119">可能な値は、`allAllowed`、`allBlocked`、`explicitAllowed` です。</span><span class="sxs-lookup"><span data-stu-id="8740a-119">Possible values are: `allAllowed`, `allBlocked`, `explicitAllowed`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="8740a-120">関係</span><span class="sxs-lookup"><span data-stu-id="8740a-120">Relationships</span></span>
<span data-ttu-id="8740a-121">なし</span><span class="sxs-lookup"><span data-stu-id="8740a-121">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="8740a-122">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="8740a-122">JSON Representation</span></span>
<span data-ttu-id="8740a-123">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="8740a-123">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.mediaContentRatingJapan"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.mediaContentRatingJapan",
  "movieRating": "String",
  "tvRating": "String"
}
```




