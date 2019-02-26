---
title: mediaContentRatingGermany リソースの種類
description: まだ文書化されていません
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 7e3c59bf110c55492db49a81a557cef0b421e328
ms.sourcegitcommit: 873b99d9001d1b2af21836e47f15360b08e10a40
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 02/26/2019
ms.locfileid: "30260355"
---
# <a name="mediacontentratinggermany-resource-type"></a><span data-ttu-id="80e84-103">mediaContentRatingGermany リソースの種類</span><span class="sxs-lookup"><span data-stu-id="80e84-103">mediaContentRatingGermany resource type</span></span>

> <span data-ttu-id="80e84-104">**注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="80e84-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="80e84-105">まだ文書化されていません</span><span class="sxs-lookup"><span data-stu-id="80e84-105">Not yet documented</span></span>

## <a name="properties"></a><span data-ttu-id="80e84-106">プロパティ</span><span class="sxs-lookup"><span data-stu-id="80e84-106">Properties</span></span>
|<span data-ttu-id="80e84-107">プロパティ</span><span class="sxs-lookup"><span data-stu-id="80e84-107">Property</span></span>|<span data-ttu-id="80e84-108">型</span><span class="sxs-lookup"><span data-stu-id="80e84-108">Type</span></span>|<span data-ttu-id="80e84-109">説明</span><span class="sxs-lookup"><span data-stu-id="80e84-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="80e84-110">movieRating</span><span class="sxs-lookup"><span data-stu-id="80e84-110">movieRating</span></span>|[<span data-ttu-id="80e84-111">ratingGermanyMoviesType</span><span class="sxs-lookup"><span data-stu-id="80e84-111">ratingGermanyMoviesType</span></span>](../resources/intune-deviceconfig-ratinggermanymoviestype.md)|<span data-ttu-id="80e84-112">ドイツ向けに選択されている映画のレーティング。</span><span class="sxs-lookup"><span data-stu-id="80e84-112">Movies rating selected for Germany.</span></span> <span data-ttu-id="80e84-113">可能な値は、`allAllowed`、`allBlocked`、`general`、`agesAbove6`、`agesAbove12`、`agesAbove16`、`adults` です。</span><span class="sxs-lookup"><span data-stu-id="80e84-113">Possible values are: `allAllowed`, `allBlocked`, `general`, `agesAbove6`, `agesAbove12`, `agesAbove16`, `adults`.</span></span>|
|<span data-ttu-id="80e84-114">tvRating</span><span class="sxs-lookup"><span data-stu-id="80e84-114">tvRating</span></span>|[<span data-ttu-id="80e84-115">ratingGermanyTelevisionType</span><span class="sxs-lookup"><span data-stu-id="80e84-115">ratingGermanyTelevisionType</span></span>](../resources/intune-deviceconfig-ratinggermanytelevisiontype.md)|<span data-ttu-id="80e84-116">ドイツ向けに選択されているテレビのレーティング。</span><span class="sxs-lookup"><span data-stu-id="80e84-116">TV rating selected for Germany.</span></span> <span data-ttu-id="80e84-117">可能な値は、`allAllowed`、`allBlocked`、`general`、`agesAbove6`、`agesAbove12`、`agesAbove16`、`adults` です。</span><span class="sxs-lookup"><span data-stu-id="80e84-117">Possible values are: `allAllowed`, `allBlocked`, `general`, `agesAbove6`, `agesAbove12`, `agesAbove16`, `adults`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="80e84-118">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="80e84-118">Relationships</span></span>
<span data-ttu-id="80e84-119">なし</span><span class="sxs-lookup"><span data-stu-id="80e84-119">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="80e84-120">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="80e84-120">JSON Representation</span></span>
<span data-ttu-id="80e84-121">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="80e84-121">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.mediaContentRatingGermany"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.mediaContentRatingGermany",
  "movieRating": "String",
  "tvRating": "String"
}
```



