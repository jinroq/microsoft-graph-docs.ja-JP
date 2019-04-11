---
title: mediaContentRatingGermany リソースの種類
description: まだ文書化されていません
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 111abc1804874dd7345d654eafdb1452c05ebd42
ms.sourcegitcommit: 20fef447f7e658a454a3887ea49746142c22e45c
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/11/2019
ms.locfileid: "31782892"
---
# <a name="mediacontentratinggermany-resource-type"></a><span data-ttu-id="9b11e-103">mediaContentRatingGermany リソースの種類</span><span class="sxs-lookup"><span data-stu-id="9b11e-103">mediaContentRatingGermany resource type</span></span>

> <span data-ttu-id="9b11e-104">**重要:** ベータ版の Microsoft Graph api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="9b11e-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="9b11e-105">**注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="9b11e-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="9b11e-106">まだ文書化されていません</span><span class="sxs-lookup"><span data-stu-id="9b11e-106">Not yet documented</span></span>

## <a name="properties"></a><span data-ttu-id="9b11e-107">プロパティ</span><span class="sxs-lookup"><span data-stu-id="9b11e-107">Properties</span></span>
|<span data-ttu-id="9b11e-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="9b11e-108">Property</span></span>|<span data-ttu-id="9b11e-109">型</span><span class="sxs-lookup"><span data-stu-id="9b11e-109">Type</span></span>|<span data-ttu-id="9b11e-110">説明</span><span class="sxs-lookup"><span data-stu-id="9b11e-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="9b11e-111">movieRating</span><span class="sxs-lookup"><span data-stu-id="9b11e-111">movieRating</span></span>|[<span data-ttu-id="9b11e-112">ratingGermanyMoviesType</span><span class="sxs-lookup"><span data-stu-id="9b11e-112">ratingGermanyMoviesType</span></span>](../resources/intune-deviceconfig-ratinggermanymoviestype.md)|<span data-ttu-id="9b11e-113">ドイツ向けに選択されている映画のレーティング。</span><span class="sxs-lookup"><span data-stu-id="9b11e-113">Movies rating selected for Germany.</span></span> <span data-ttu-id="9b11e-114">可能な値は、`allAllowed`、`allBlocked`、`general`、`agesAbove6`、`agesAbove12`、`agesAbove16`、`adults` です。</span><span class="sxs-lookup"><span data-stu-id="9b11e-114">Possible values are: `allAllowed`, `allBlocked`, `general`, `agesAbove6`, `agesAbove12`, `agesAbove16`, `adults`.</span></span>|
|<span data-ttu-id="9b11e-115">tvRating</span><span class="sxs-lookup"><span data-stu-id="9b11e-115">tvRating</span></span>|[<span data-ttu-id="9b11e-116">ratingGermanyTelevisionType</span><span class="sxs-lookup"><span data-stu-id="9b11e-116">ratingGermanyTelevisionType</span></span>](../resources/intune-deviceconfig-ratinggermanytelevisiontype.md)|<span data-ttu-id="9b11e-117">ドイツ向けに選択されているテレビのレーティング。</span><span class="sxs-lookup"><span data-stu-id="9b11e-117">TV rating selected for Germany.</span></span> <span data-ttu-id="9b11e-118">可能な値は、`allAllowed`、`allBlocked`、`general`、`agesAbove6`、`agesAbove12`、`agesAbove16`、`adults` です。</span><span class="sxs-lookup"><span data-stu-id="9b11e-118">Possible values are: `allAllowed`, `allBlocked`, `general`, `agesAbove6`, `agesAbove12`, `agesAbove16`, `adults`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="9b11e-119">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="9b11e-119">Relationships</span></span>
<span data-ttu-id="9b11e-120">なし</span><span class="sxs-lookup"><span data-stu-id="9b11e-120">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="9b11e-121">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="9b11e-121">JSON Representation</span></span>
<span data-ttu-id="9b11e-122">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="9b11e-122">Here is a JSON representation of the resource.</span></span>
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





