---
title: mediaContentRatingUnitedKingdom リソースの種類
description: まだ文書化されていません
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 2c91558168922c4b608d62add941b69a5749bc9f
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32554465"
---
# <a name="mediacontentratingunitedkingdom-resource-type"></a><span data-ttu-id="6c2f2-103">mediaContentRatingUnitedKingdom リソースの種類</span><span class="sxs-lookup"><span data-stu-id="6c2f2-103">mediaContentRatingUnitedKingdom resource type</span></span>

> <span data-ttu-id="6c2f2-104">**重要:** ベータ版の Microsoft Graph api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="6c2f2-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="6c2f2-105">**注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="6c2f2-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="6c2f2-106">まだ文書化されていません</span><span class="sxs-lookup"><span data-stu-id="6c2f2-106">Not yet documented</span></span>

## <a name="properties"></a><span data-ttu-id="6c2f2-107">プロパティ</span><span class="sxs-lookup"><span data-stu-id="6c2f2-107">Properties</span></span>
|<span data-ttu-id="6c2f2-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="6c2f2-108">Property</span></span>|<span data-ttu-id="6c2f2-109">型</span><span class="sxs-lookup"><span data-stu-id="6c2f2-109">Type</span></span>|<span data-ttu-id="6c2f2-110">説明</span><span class="sxs-lookup"><span data-stu-id="6c2f2-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="6c2f2-111">movieRating</span><span class="sxs-lookup"><span data-stu-id="6c2f2-111">movieRating</span></span>|[<span data-ttu-id="6c2f2-112">ratingUnitedKingdomMoviesType</span><span class="sxs-lookup"><span data-stu-id="6c2f2-112">ratingUnitedKingdomMoviesType</span></span>](../resources/intune-deviceconfig-ratingunitedkingdommoviestype.md)|<span data-ttu-id="6c2f2-113">英国向けに選択されている映画のレーティング。</span><span class="sxs-lookup"><span data-stu-id="6c2f2-113">Movies rating selected for United Kingdom.</span></span> <span data-ttu-id="6c2f2-114">可能な値は、`allAllowed`、`allBlocked`、`general`、`universalChildren`、`parentalGuidance`、`agesAbove12Video`、`agesAbove12Cinema`、`agesAbove15`、`adults` です。</span><span class="sxs-lookup"><span data-stu-id="6c2f2-114">Possible values are: `allAllowed`, `allBlocked`, `general`, `universalChildren`, `parentalGuidance`, `agesAbove12Video`, `agesAbove12Cinema`, `agesAbove15`, `adults`.</span></span>|
|<span data-ttu-id="6c2f2-115">tvRating</span><span class="sxs-lookup"><span data-stu-id="6c2f2-115">tvRating</span></span>|[<span data-ttu-id="6c2f2-116">ratingUnitedKingdomTelevisionType</span><span class="sxs-lookup"><span data-stu-id="6c2f2-116">ratingUnitedKingdomTelevisionType</span></span>](../resources/intune-deviceconfig-ratingunitedkingdomtelevisiontype.md)|<span data-ttu-id="6c2f2-117">英国向けに選択されているテレビのレーティング。</span><span class="sxs-lookup"><span data-stu-id="6c2f2-117">TV rating selected for United Kingdom.</span></span> <span data-ttu-id="6c2f2-118">可能な値は、`allAllowed`、`allBlocked`、`caution` です。</span><span class="sxs-lookup"><span data-stu-id="6c2f2-118">Possible values are: `allAllowed`, `allBlocked`, `caution`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="6c2f2-119">関係</span><span class="sxs-lookup"><span data-stu-id="6c2f2-119">Relationships</span></span>
<span data-ttu-id="6c2f2-120">なし</span><span class="sxs-lookup"><span data-stu-id="6c2f2-120">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="6c2f2-121">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="6c2f2-121">JSON Representation</span></span>
<span data-ttu-id="6c2f2-122">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="6c2f2-122">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.mediaContentRatingUnitedKingdom"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.mediaContentRatingUnitedKingdom",
  "movieRating": "String",
  "tvRating": "String"
}
```





