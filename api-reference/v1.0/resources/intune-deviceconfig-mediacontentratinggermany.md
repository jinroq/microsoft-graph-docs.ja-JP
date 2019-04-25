---
title: mediaContentRatingGermany リソースの種類
description: まだ文書化されていません
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 7e3c59bf110c55492db49a81a557cef0b421e328
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32572382"
---
# <a name="mediacontentratinggermany-resource-type"></a><span data-ttu-id="d1f0b-103">mediaContentRatingGermany リソースの種類</span><span class="sxs-lookup"><span data-stu-id="d1f0b-103">mediaContentRatingGermany resource type</span></span>

> <span data-ttu-id="d1f0b-104">**注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="d1f0b-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="d1f0b-105">まだ文書化されていません</span><span class="sxs-lookup"><span data-stu-id="d1f0b-105">Not yet documented</span></span>

## <a name="properties"></a><span data-ttu-id="d1f0b-106">プロパティ</span><span class="sxs-lookup"><span data-stu-id="d1f0b-106">Properties</span></span>
|<span data-ttu-id="d1f0b-107">プロパティ</span><span class="sxs-lookup"><span data-stu-id="d1f0b-107">Property</span></span>|<span data-ttu-id="d1f0b-108">型</span><span class="sxs-lookup"><span data-stu-id="d1f0b-108">Type</span></span>|<span data-ttu-id="d1f0b-109">説明</span><span class="sxs-lookup"><span data-stu-id="d1f0b-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d1f0b-110">movieRating</span><span class="sxs-lookup"><span data-stu-id="d1f0b-110">movieRating</span></span>|[<span data-ttu-id="d1f0b-111">ratingGermanyMoviesType</span><span class="sxs-lookup"><span data-stu-id="d1f0b-111">ratingGermanyMoviesType</span></span>](../resources/intune-deviceconfig-ratinggermanymoviestype.md)|<span data-ttu-id="d1f0b-112">ドイツ向けに選択されている映画のレーティング。</span><span class="sxs-lookup"><span data-stu-id="d1f0b-112">Movies rating selected for Germany.</span></span> <span data-ttu-id="d1f0b-113">可能な値は、`allAllowed`、`allBlocked`、`general`、`agesAbove6`、`agesAbove12`、`agesAbove16`、`adults` です。</span><span class="sxs-lookup"><span data-stu-id="d1f0b-113">Possible values are: `allAllowed`, `allBlocked`, `general`, `agesAbove6`, `agesAbove12`, `agesAbove16`, `adults`.</span></span>|
|<span data-ttu-id="d1f0b-114">tvRating</span><span class="sxs-lookup"><span data-stu-id="d1f0b-114">tvRating</span></span>|[<span data-ttu-id="d1f0b-115">ratingGermanyTelevisionType</span><span class="sxs-lookup"><span data-stu-id="d1f0b-115">ratingGermanyTelevisionType</span></span>](../resources/intune-deviceconfig-ratinggermanytelevisiontype.md)|<span data-ttu-id="d1f0b-116">ドイツ向けに選択されているテレビのレーティング。</span><span class="sxs-lookup"><span data-stu-id="d1f0b-116">TV rating selected for Germany.</span></span> <span data-ttu-id="d1f0b-117">可能な値は、`allAllowed`、`allBlocked`、`general`、`agesAbove6`、`agesAbove12`、`agesAbove16`、`adults` です。</span><span class="sxs-lookup"><span data-stu-id="d1f0b-117">Possible values are: `allAllowed`, `allBlocked`, `general`, `agesAbove6`, `agesAbove12`, `agesAbove16`, `adults`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="d1f0b-118">関係</span><span class="sxs-lookup"><span data-stu-id="d1f0b-118">Relationships</span></span>
<span data-ttu-id="d1f0b-119">なし</span><span class="sxs-lookup"><span data-stu-id="d1f0b-119">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="d1f0b-120">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="d1f0b-120">JSON Representation</span></span>
<span data-ttu-id="d1f0b-121">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="d1f0b-121">Here is a JSON representation of the resource.</span></span>
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



