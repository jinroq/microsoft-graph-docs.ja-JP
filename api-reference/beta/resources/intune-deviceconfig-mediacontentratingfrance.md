---
title: mediaContentRatingFrance リソースの種類
description: まだ文書化されていません
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 9e3d270bfb876f33afdd1944f070aaefe58fe569
ms.sourcegitcommit: 20fef447f7e658a454a3887ea49746142c22e45c
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/11/2019
ms.locfileid: "31786785"
---
# <a name="mediacontentratingfrance-resource-type"></a><span data-ttu-id="8a2af-103">mediaContentRatingFrance リソースの種類</span><span class="sxs-lookup"><span data-stu-id="8a2af-103">mediaContentRatingFrance resource type</span></span>

> <span data-ttu-id="8a2af-104">**重要:** ベータ版の Microsoft Graph api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="8a2af-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="8a2af-105">**注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="8a2af-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="8a2af-106">まだ文書化されていません</span><span class="sxs-lookup"><span data-stu-id="8a2af-106">Not yet documented</span></span>

## <a name="properties"></a><span data-ttu-id="8a2af-107">プロパティ</span><span class="sxs-lookup"><span data-stu-id="8a2af-107">Properties</span></span>
|<span data-ttu-id="8a2af-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="8a2af-108">Property</span></span>|<span data-ttu-id="8a2af-109">型</span><span class="sxs-lookup"><span data-stu-id="8a2af-109">Type</span></span>|<span data-ttu-id="8a2af-110">説明</span><span class="sxs-lookup"><span data-stu-id="8a2af-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="8a2af-111">movieRating</span><span class="sxs-lookup"><span data-stu-id="8a2af-111">movieRating</span></span>|[<span data-ttu-id="8a2af-112">ratingFranceMoviesType</span><span class="sxs-lookup"><span data-stu-id="8a2af-112">ratingFranceMoviesType</span></span>](../resources/intune-deviceconfig-ratingfrancemoviestype.md)|<span data-ttu-id="8a2af-113">フランスに対して選択されている映画のレーティング。</span><span class="sxs-lookup"><span data-stu-id="8a2af-113">Movies rating selected for France.</span></span> <span data-ttu-id="8a2af-114">可能な値は `allAllowed`、`allBlocked`、`agesAbove10`、`agesAbove12`、`agesAbove16`、`agesAbove18` です。</span><span class="sxs-lookup"><span data-stu-id="8a2af-114">Possible values are: `allAllowed`, `allBlocked`, `agesAbove10`, `agesAbove12`, `agesAbove16`, `agesAbove18`.</span></span>|
|<span data-ttu-id="8a2af-115">tvRating</span><span class="sxs-lookup"><span data-stu-id="8a2af-115">tvRating</span></span>|[<span data-ttu-id="8a2af-116">ratingFranceTelevisionType</span><span class="sxs-lookup"><span data-stu-id="8a2af-116">ratingFranceTelevisionType</span></span>](../resources/intune-deviceconfig-ratingfrancetelevisiontype.md)|<span data-ttu-id="8a2af-117">フランスに対して選択されているテレビのレーティング。</span><span class="sxs-lookup"><span data-stu-id="8a2af-117">TV rating selected for France.</span></span> <span data-ttu-id="8a2af-118">可能な値は `allAllowed`、`allBlocked`、`agesAbove10`、`agesAbove12`、`agesAbove16`、`agesAbove18` です。</span><span class="sxs-lookup"><span data-stu-id="8a2af-118">Possible values are: `allAllowed`, `allBlocked`, `agesAbove10`, `agesAbove12`, `agesAbove16`, `agesAbove18`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="8a2af-119">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="8a2af-119">Relationships</span></span>
<span data-ttu-id="8a2af-120">なし</span><span class="sxs-lookup"><span data-stu-id="8a2af-120">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="8a2af-121">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="8a2af-121">JSON Representation</span></span>
<span data-ttu-id="8a2af-122">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="8a2af-122">Here is a JSON representation of the resource.</span></span>
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





