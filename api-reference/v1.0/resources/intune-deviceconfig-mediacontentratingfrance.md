---
title: mediaContentRatingFrance リソースの種類
description: まだ文書化されていません
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 979a5996b655ba13847e52dc09b083169ff0815a
ms.sourcegitcommit: 873b99d9001d1b2af21836e47f15360b08e10a40
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 02/26/2019
ms.locfileid: "30260229"
---
# <a name="mediacontentratingfrance-resource-type"></a><span data-ttu-id="f83dc-103">mediaContentRatingFrance リソースの種類</span><span class="sxs-lookup"><span data-stu-id="f83dc-103">mediaContentRatingFrance resource type</span></span>

> <span data-ttu-id="f83dc-104">**注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="f83dc-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="f83dc-105">まだ文書化されていません</span><span class="sxs-lookup"><span data-stu-id="f83dc-105">Not yet documented</span></span>

## <a name="properties"></a><span data-ttu-id="f83dc-106">プロパティ</span><span class="sxs-lookup"><span data-stu-id="f83dc-106">Properties</span></span>
|<span data-ttu-id="f83dc-107">プロパティ</span><span class="sxs-lookup"><span data-stu-id="f83dc-107">Property</span></span>|<span data-ttu-id="f83dc-108">型</span><span class="sxs-lookup"><span data-stu-id="f83dc-108">Type</span></span>|<span data-ttu-id="f83dc-109">説明</span><span class="sxs-lookup"><span data-stu-id="f83dc-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f83dc-110">movieRating</span><span class="sxs-lookup"><span data-stu-id="f83dc-110">movieRating</span></span>|[<span data-ttu-id="f83dc-111">ratingFranceMoviesType</span><span class="sxs-lookup"><span data-stu-id="f83dc-111">ratingFranceMoviesType</span></span>](../resources/intune-deviceconfig-ratingfrancemoviestype.md)|<span data-ttu-id="f83dc-112">フランスに対して選択されている映画のレーティング。</span><span class="sxs-lookup"><span data-stu-id="f83dc-112">Movies rating selected for France.</span></span> <span data-ttu-id="f83dc-113">使用可能な値: `allAllowed`、`allBlocked`、`agesAbove10`、`agesAbove12`、`agesAbove16`、`agesAbove18`。</span><span class="sxs-lookup"><span data-stu-id="f83dc-113">Possible values are: `allAllowed`, `allBlocked`, `agesAbove10`, `agesAbove12`, `agesAbove16`, `agesAbove18`.</span></span>|
|<span data-ttu-id="f83dc-114">tvRating</span><span class="sxs-lookup"><span data-stu-id="f83dc-114">tvRating</span></span>|[<span data-ttu-id="f83dc-115">ratingFranceTelevisionType</span><span class="sxs-lookup"><span data-stu-id="f83dc-115">ratingFranceTelevisionType</span></span>](../resources/intune-deviceconfig-ratingfrancetelevisiontype.md)|<span data-ttu-id="f83dc-116">フランスに対して選択されているテレビのレーティング。</span><span class="sxs-lookup"><span data-stu-id="f83dc-116">TV rating selected for France.</span></span> <span data-ttu-id="f83dc-117">使用可能な値: `allAllowed`、`allBlocked`、`agesAbove10`、`agesAbove12`、`agesAbove16`、`agesAbove18`。</span><span class="sxs-lookup"><span data-stu-id="f83dc-117">Possible values are: `allAllowed`, `allBlocked`, `agesAbove10`, `agesAbove12`, `agesAbove16`, `agesAbove18`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="f83dc-118">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="f83dc-118">Relationships</span></span>
<span data-ttu-id="f83dc-119">なし</span><span class="sxs-lookup"><span data-stu-id="f83dc-119">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="f83dc-120">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="f83dc-120">JSON Representation</span></span>
<span data-ttu-id="f83dc-121">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="f83dc-121">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.mediaContentRatingFrance"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.mediaContentRatingFrance",
  "movieRating": "String",
  "tvRating": "String"
}
```



