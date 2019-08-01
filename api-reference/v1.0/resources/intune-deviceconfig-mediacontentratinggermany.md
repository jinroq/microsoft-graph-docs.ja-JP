---
title: mediaContentRatingGermany リソースの種類
description: まだ文書化されていません
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: b4f2eda6b9666d3b23ea48d96f7a7231e189b4f5
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "36028099"
---
# <a name="mediacontentratinggermany-resource-type"></a><span data-ttu-id="d9ee0-103">mediaContentRatingGermany リソースの種類</span><span class="sxs-lookup"><span data-stu-id="d9ee0-103">mediaContentRatingGermany resource type</span></span>

> <span data-ttu-id="d9ee0-104">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="d9ee0-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="d9ee0-105">まだ文書化されていません</span><span class="sxs-lookup"><span data-stu-id="d9ee0-105">Not yet documented</span></span>

## <a name="properties"></a><span data-ttu-id="d9ee0-106">プロパティ</span><span class="sxs-lookup"><span data-stu-id="d9ee0-106">Properties</span></span>
|<span data-ttu-id="d9ee0-107">プロパティ</span><span class="sxs-lookup"><span data-stu-id="d9ee0-107">Property</span></span>|<span data-ttu-id="d9ee0-108">型</span><span class="sxs-lookup"><span data-stu-id="d9ee0-108">Type</span></span>|<span data-ttu-id="d9ee0-109">説明</span><span class="sxs-lookup"><span data-stu-id="d9ee0-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d9ee0-110">movieRating</span><span class="sxs-lookup"><span data-stu-id="d9ee0-110">movieRating</span></span>|[<span data-ttu-id="d9ee0-111">ratingGermanyMoviesType</span><span class="sxs-lookup"><span data-stu-id="d9ee0-111">ratingGermanyMoviesType</span></span>](../resources/intune-deviceconfig-ratinggermanymoviestype.md)|<span data-ttu-id="d9ee0-112">ドイツ向けに選択されている映画のレーティング。</span><span class="sxs-lookup"><span data-stu-id="d9ee0-112">Movies rating selected for Germany.</span></span> <span data-ttu-id="d9ee0-113">可能な値は、`allAllowed`、`allBlocked`、`general`、`agesAbove6`、`agesAbove12`、`agesAbove16`、`adults` です。</span><span class="sxs-lookup"><span data-stu-id="d9ee0-113">Possible values are: `allAllowed`, `allBlocked`, `general`, `agesAbove6`, `agesAbove12`, `agesAbove16`, `adults`.</span></span>|
|<span data-ttu-id="d9ee0-114">tvRating</span><span class="sxs-lookup"><span data-stu-id="d9ee0-114">tvRating</span></span>|[<span data-ttu-id="d9ee0-115">ratingGermanyTelevisionType</span><span class="sxs-lookup"><span data-stu-id="d9ee0-115">ratingGermanyTelevisionType</span></span>](../resources/intune-deviceconfig-ratinggermanytelevisiontype.md)|<span data-ttu-id="d9ee0-116">ドイツ向けに選択されているテレビのレーティング。</span><span class="sxs-lookup"><span data-stu-id="d9ee0-116">TV rating selected for Germany.</span></span> <span data-ttu-id="d9ee0-117">可能な値は、`allAllowed`、`allBlocked`、`general`、`agesAbove6`、`agesAbove12`、`agesAbove16`、`adults` です。</span><span class="sxs-lookup"><span data-stu-id="d9ee0-117">Possible values are: `allAllowed`, `allBlocked`, `general`, `agesAbove6`, `agesAbove12`, `agesAbove16`, `adults`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="d9ee0-118">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="d9ee0-118">Relationships</span></span>
<span data-ttu-id="d9ee0-119">なし</span><span class="sxs-lookup"><span data-stu-id="d9ee0-119">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="d9ee0-120">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="d9ee0-120">JSON Representation</span></span>
<span data-ttu-id="d9ee0-121">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="d9ee0-121">Here is a JSON representation of the resource.</span></span>
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



