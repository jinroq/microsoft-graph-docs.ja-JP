---
title: mediaContentRatingAustralia リソースの種類
description: まだ文書化されていません
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 5703da7bcc21cc84b0f133e9a6b653e1b22031c3
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32572774"
---
# <a name="mediacontentratingaustralia-resource-type"></a><span data-ttu-id="92d10-103">mediaContentRatingAustralia リソースの種類</span><span class="sxs-lookup"><span data-stu-id="92d10-103">mediaContentRatingAustralia resource type</span></span>

> <span data-ttu-id="92d10-104">**重要:** ベータ版の Microsoft Graph api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="92d10-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="92d10-105">**注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="92d10-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="92d10-106">まだ文書化されていません</span><span class="sxs-lookup"><span data-stu-id="92d10-106">Not yet documented</span></span>

## <a name="properties"></a><span data-ttu-id="92d10-107">プロパティ</span><span class="sxs-lookup"><span data-stu-id="92d10-107">Properties</span></span>
|<span data-ttu-id="92d10-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="92d10-108">Property</span></span>|<span data-ttu-id="92d10-109">型</span><span class="sxs-lookup"><span data-stu-id="92d10-109">Type</span></span>|<span data-ttu-id="92d10-110">説明</span><span class="sxs-lookup"><span data-stu-id="92d10-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="92d10-111">movieRating</span><span class="sxs-lookup"><span data-stu-id="92d10-111">movieRating</span></span>|[<span data-ttu-id="92d10-112">ratingAustraliaMoviesType</span><span class="sxs-lookup"><span data-stu-id="92d10-112">ratingAustraliaMoviesType</span></span>](../resources/intune-deviceconfig-ratingaustraliamoviestype.md)|<span data-ttu-id="92d10-113">オーストラリア向けに選択されている映画のレーティング。</span><span class="sxs-lookup"><span data-stu-id="92d10-113">Movies rating selected for Australia.</span></span> <span data-ttu-id="92d10-114">可能な値は、`allAllowed`、`allBlocked`、`general`、`parentalGuidance`、`mature`、`agesAbove15`、`agesAbove18` です。</span><span class="sxs-lookup"><span data-stu-id="92d10-114">Possible values are: `allAllowed`, `allBlocked`, `general`, `parentalGuidance`, `mature`, `agesAbove15`, `agesAbove18`.</span></span>|
|<span data-ttu-id="92d10-115">tvRating</span><span class="sxs-lookup"><span data-stu-id="92d10-115">tvRating</span></span>|[<span data-ttu-id="92d10-116">ratingAustraliaTelevisionType</span><span class="sxs-lookup"><span data-stu-id="92d10-116">ratingAustraliaTelevisionType</span></span>](../resources/intune-deviceconfig-ratingaustraliatelevisiontype.md)|<span data-ttu-id="92d10-117">オーストラリア向けに選択されているテレビのレーティング。</span><span class="sxs-lookup"><span data-stu-id="92d10-117">TV rating selected for Australia.</span></span> <span data-ttu-id="92d10-118">可能な値は、`allAllowed`、`allBlocked`、`preschoolers`、`children`、`general`、`parentalGuidance`、`mature`、`agesAbove15`、`agesAbove15AdultViolence` です。</span><span class="sxs-lookup"><span data-stu-id="92d10-118">Possible values are: `allAllowed`, `allBlocked`, `preschoolers`, `children`, `general`, `parentalGuidance`, `mature`, `agesAbove15`, `agesAbove15AdultViolence`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="92d10-119">関係</span><span class="sxs-lookup"><span data-stu-id="92d10-119">Relationships</span></span>
<span data-ttu-id="92d10-120">なし</span><span class="sxs-lookup"><span data-stu-id="92d10-120">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="92d10-121">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="92d10-121">JSON Representation</span></span>
<span data-ttu-id="92d10-122">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="92d10-122">Here is a JSON representation of the resource.</span></span>
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





