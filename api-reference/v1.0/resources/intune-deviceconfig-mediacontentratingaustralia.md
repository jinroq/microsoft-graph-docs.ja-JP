---
title: mediaContentRatingAustralia リソースの種類
description: まだ文書化されていません
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 0a9e3035585794216440522233f23a8061ddafee
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "36031431"
---
# <a name="mediacontentratingaustralia-resource-type"></a><span data-ttu-id="c0a6a-103">mediaContentRatingAustralia リソースの種類</span><span class="sxs-lookup"><span data-stu-id="c0a6a-103">mediaContentRatingAustralia resource type</span></span>

> <span data-ttu-id="c0a6a-104">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="c0a6a-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="c0a6a-105">まだ文書化されていません</span><span class="sxs-lookup"><span data-stu-id="c0a6a-105">Not yet documented</span></span>

## <a name="properties"></a><span data-ttu-id="c0a6a-106">プロパティ</span><span class="sxs-lookup"><span data-stu-id="c0a6a-106">Properties</span></span>
|<span data-ttu-id="c0a6a-107">プロパティ</span><span class="sxs-lookup"><span data-stu-id="c0a6a-107">Property</span></span>|<span data-ttu-id="c0a6a-108">型</span><span class="sxs-lookup"><span data-stu-id="c0a6a-108">Type</span></span>|<span data-ttu-id="c0a6a-109">説明</span><span class="sxs-lookup"><span data-stu-id="c0a6a-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c0a6a-110">movieRating</span><span class="sxs-lookup"><span data-stu-id="c0a6a-110">movieRating</span></span>|[<span data-ttu-id="c0a6a-111">ratingAustraliaMoviesType</span><span class="sxs-lookup"><span data-stu-id="c0a6a-111">ratingAustraliaMoviesType</span></span>](../resources/intune-deviceconfig-ratingaustraliamoviestype.md)|<span data-ttu-id="c0a6a-112">オーストラリア向けに選択されている映画のレーティング。</span><span class="sxs-lookup"><span data-stu-id="c0a6a-112">Movies rating selected for Australia.</span></span> <span data-ttu-id="c0a6a-113">可能な値は、`allAllowed`、`allBlocked`、`general`、`parentalGuidance`、`mature`、`agesAbove15`、`agesAbove18` です。</span><span class="sxs-lookup"><span data-stu-id="c0a6a-113">Possible values are: `allAllowed`, `allBlocked`, `general`, `parentalGuidance`, `mature`, `agesAbove15`, `agesAbove18`.</span></span>|
|<span data-ttu-id="c0a6a-114">tvRating</span><span class="sxs-lookup"><span data-stu-id="c0a6a-114">tvRating</span></span>|[<span data-ttu-id="c0a6a-115">ratingAustraliaTelevisionType</span><span class="sxs-lookup"><span data-stu-id="c0a6a-115">ratingAustraliaTelevisionType</span></span>](../resources/intune-deviceconfig-ratingaustraliatelevisiontype.md)|<span data-ttu-id="c0a6a-116">オーストラリア向けに選択されているテレビのレーティング。</span><span class="sxs-lookup"><span data-stu-id="c0a6a-116">TV rating selected for Australia.</span></span> <span data-ttu-id="c0a6a-117">可能な値は、`allAllowed`、`allBlocked`、`preschoolers`、`children`、`general`、`parentalGuidance`、`mature`、`agesAbove15`、`agesAbove15AdultViolence` です。</span><span class="sxs-lookup"><span data-stu-id="c0a6a-117">Possible values are: `allAllowed`, `allBlocked`, `preschoolers`, `children`, `general`, `parentalGuidance`, `mature`, `agesAbove15`, `agesAbove15AdultViolence`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="c0a6a-118">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="c0a6a-118">Relationships</span></span>
<span data-ttu-id="c0a6a-119">なし</span><span class="sxs-lookup"><span data-stu-id="c0a6a-119">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="c0a6a-120">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="c0a6a-120">JSON Representation</span></span>
<span data-ttu-id="c0a6a-121">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="c0a6a-121">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.mediaContentRatingAustralia"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.mediaContentRatingAustralia",
  "movieRating": "String",
  "tvRating": "String"
}
```



