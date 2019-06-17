---
title: mediaContentRatingUnitedKingdom リソースの種類
description: まだ文書化されていません
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 0099abaf692a51a4cc2c2ea0630777ab683876d5
ms.sourcegitcommit: 0a62bc5849f27a55d83efce9b3eb01b9711bbe1d
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/14/2019
ms.locfileid: "34986768"
---
# <a name="mediacontentratingunitedkingdom-resource-type"></a><span data-ttu-id="c59c8-103">mediaContentRatingUnitedKingdom リソースの種類</span><span class="sxs-lookup"><span data-stu-id="c59c8-103">mediaContentRatingUnitedKingdom resource type</span></span>

> <span data-ttu-id="c59c8-104">**重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="c59c8-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="c59c8-105">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="c59c8-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="c59c8-106">まだ文書化されていません</span><span class="sxs-lookup"><span data-stu-id="c59c8-106">Not yet documented</span></span>

## <a name="properties"></a><span data-ttu-id="c59c8-107">プロパティ</span><span class="sxs-lookup"><span data-stu-id="c59c8-107">Properties</span></span>
|<span data-ttu-id="c59c8-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="c59c8-108">Property</span></span>|<span data-ttu-id="c59c8-109">型</span><span class="sxs-lookup"><span data-stu-id="c59c8-109">Type</span></span>|<span data-ttu-id="c59c8-110">説明</span><span class="sxs-lookup"><span data-stu-id="c59c8-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c59c8-111">movieRating</span><span class="sxs-lookup"><span data-stu-id="c59c8-111">movieRating</span></span>|[<span data-ttu-id="c59c8-112">ratingUnitedKingdomMoviesType</span><span class="sxs-lookup"><span data-stu-id="c59c8-112">ratingUnitedKingdomMoviesType</span></span>](../resources/intune-deviceconfig-ratingunitedkingdommoviestype.md)|<span data-ttu-id="c59c8-113">英国向けに選択されている映画のレーティング。</span><span class="sxs-lookup"><span data-stu-id="c59c8-113">Movies rating selected for United Kingdom.</span></span> <span data-ttu-id="c59c8-114">可能な値は、`allAllowed`、`allBlocked`、`general`、`universalChildren`、`parentalGuidance`、`agesAbove12Video`、`agesAbove12Cinema`、`agesAbove15`、`adults` です。</span><span class="sxs-lookup"><span data-stu-id="c59c8-114">Possible values are: `allAllowed`, `allBlocked`, `general`, `universalChildren`, `parentalGuidance`, `agesAbove12Video`, `agesAbove12Cinema`, `agesAbove15`, `adults`.</span></span>|
|<span data-ttu-id="c59c8-115">tvRating</span><span class="sxs-lookup"><span data-stu-id="c59c8-115">tvRating</span></span>|[<span data-ttu-id="c59c8-116">ratingUnitedKingdomTelevisionType</span><span class="sxs-lookup"><span data-stu-id="c59c8-116">ratingUnitedKingdomTelevisionType</span></span>](../resources/intune-deviceconfig-ratingunitedkingdomtelevisiontype.md)|<span data-ttu-id="c59c8-117">英国向けに選択されているテレビのレーティング。</span><span class="sxs-lookup"><span data-stu-id="c59c8-117">TV rating selected for United Kingdom.</span></span> <span data-ttu-id="c59c8-118">可能な値は、`allAllowed`、`allBlocked`、`caution` です。</span><span class="sxs-lookup"><span data-stu-id="c59c8-118">Possible values are: `allAllowed`, `allBlocked`, `caution`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="c59c8-119">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="c59c8-119">Relationships</span></span>
<span data-ttu-id="c59c8-120">なし</span><span class="sxs-lookup"><span data-stu-id="c59c8-120">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="c59c8-121">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="c59c8-121">JSON Representation</span></span>
<span data-ttu-id="c59c8-122">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="c59c8-122">Here is a JSON representation of the resource.</span></span>
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





