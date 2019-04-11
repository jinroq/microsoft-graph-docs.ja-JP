---
title: mediaContentRatingNewZealand リソースの種類
description: まだ文書化されていません
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: d1d2b608a285413e8ad4f7049d06982a06878450
ms.sourcegitcommit: 20fef447f7e658a454a3887ea49746142c22e45c
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/11/2019
ms.locfileid: "31807169"
---
# <a name="mediacontentratingnewzealand-resource-type"></a><span data-ttu-id="69df2-103">mediaContentRatingNewZealand リソースの種類</span><span class="sxs-lookup"><span data-stu-id="69df2-103">mediaContentRatingNewZealand resource type</span></span>

> <span data-ttu-id="69df2-104">**重要:** ベータ版の Microsoft Graph api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="69df2-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="69df2-105">**注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="69df2-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="69df2-106">まだ文書化されていません</span><span class="sxs-lookup"><span data-stu-id="69df2-106">Not yet documented</span></span>

## <a name="properties"></a><span data-ttu-id="69df2-107">プロパティ</span><span class="sxs-lookup"><span data-stu-id="69df2-107">Properties</span></span>
|<span data-ttu-id="69df2-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="69df2-108">Property</span></span>|<span data-ttu-id="69df2-109">型</span><span class="sxs-lookup"><span data-stu-id="69df2-109">Type</span></span>|<span data-ttu-id="69df2-110">説明</span><span class="sxs-lookup"><span data-stu-id="69df2-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="69df2-111">movieRating</span><span class="sxs-lookup"><span data-stu-id="69df2-111">movieRating</span></span>|[<span data-ttu-id="69df2-112">ratingNewZealandMoviesType</span><span class="sxs-lookup"><span data-stu-id="69df2-112">ratingNewZealandMoviesType</span></span>](../resources/intune-deviceconfig-ratingnewzealandmoviestype.md)|<span data-ttu-id="69df2-113">ニュージーランドで選択されている映画のレーティング。</span><span class="sxs-lookup"><span data-stu-id="69df2-113">Movies rating selected for New Zealand.</span></span> <span data-ttu-id="69df2-114">使用可能な値は、`allAllowed`、`allBlocked`、`general`、`parentalGuidance`、`mature`、`agesAbove13`、`agesAbove15`、`agesAbove16`、`agesAbove18`、`restricted`、`agesAbove16Restricted` です。</span><span class="sxs-lookup"><span data-stu-id="69df2-114">Possible values are: `allAllowed`, `allBlocked`, `general`, `parentalGuidance`, `mature`, `agesAbove13`, `agesAbove15`, `agesAbove16`, `agesAbove18`, `restricted`, `agesAbove16Restricted`.</span></span>|
|<span data-ttu-id="69df2-115">tvRating</span><span class="sxs-lookup"><span data-stu-id="69df2-115">tvRating</span></span>|[<span data-ttu-id="69df2-116">ratingNewZealandTelevisionType</span><span class="sxs-lookup"><span data-stu-id="69df2-116">ratingNewZealandTelevisionType</span></span>](../resources/intune-deviceconfig-ratingnewzealandtelevisiontype.md)|<span data-ttu-id="69df2-117">ニュージーランド用に選択されているテレビのレーティング。</span><span class="sxs-lookup"><span data-stu-id="69df2-117">TV rating selected for New Zealand.</span></span> <span data-ttu-id="69df2-118">可能な値は、`allAllowed`、`allBlocked`、`general`、`parentalGuidance`、`adults` です。</span><span class="sxs-lookup"><span data-stu-id="69df2-118">Possible values are: `allAllowed`, `allBlocked`, `general`, `parentalGuidance`, `adults`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="69df2-119">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="69df2-119">Relationships</span></span>
<span data-ttu-id="69df2-120">なし</span><span class="sxs-lookup"><span data-stu-id="69df2-120">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="69df2-121">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="69df2-121">JSON Representation</span></span>
<span data-ttu-id="69df2-122">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="69df2-122">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.mediaContentRatingNewZealand"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.mediaContentRatingNewZealand",
  "movieRating": "String",
  "tvRating": "String"
}
```





