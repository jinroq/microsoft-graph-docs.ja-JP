---
title: mediaContentRatingJapan リソースの種類
description: まだ文書化されていません
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 8b1c79e68a530d176445b0395fdb7c4d50996485
ms.sourcegitcommit: 94aaf594c881c02f353c6a417460cdf783a0bfe0
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/11/2019
ms.locfileid: "33950887"
---
# <a name="mediacontentratingjapan-resource-type"></a><span data-ttu-id="7fd2d-103">mediaContentRatingJapan リソースの種類</span><span class="sxs-lookup"><span data-stu-id="7fd2d-103">mediaContentRatingJapan resource type</span></span>

> <span data-ttu-id="7fd2d-104">**重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="7fd2d-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="7fd2d-105">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="7fd2d-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="7fd2d-106">まだ文書化されていません</span><span class="sxs-lookup"><span data-stu-id="7fd2d-106">Not yet documented</span></span>

## <a name="properties"></a><span data-ttu-id="7fd2d-107">プロパティ</span><span class="sxs-lookup"><span data-stu-id="7fd2d-107">Properties</span></span>
|<span data-ttu-id="7fd2d-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="7fd2d-108">Property</span></span>|<span data-ttu-id="7fd2d-109">型</span><span class="sxs-lookup"><span data-stu-id="7fd2d-109">Type</span></span>|<span data-ttu-id="7fd2d-110">説明</span><span class="sxs-lookup"><span data-stu-id="7fd2d-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="7fd2d-111">movieRating</span><span class="sxs-lookup"><span data-stu-id="7fd2d-111">movieRating</span></span>|[<span data-ttu-id="7fd2d-112">ratingJapanMoviesType</span><span class="sxs-lookup"><span data-stu-id="7fd2d-112">ratingJapanMoviesType</span></span>](../resources/intune-deviceconfig-ratingjapanmoviestype.md)|<span data-ttu-id="7fd2d-113">日本向けに選択されている映画のレーティング。</span><span class="sxs-lookup"><span data-stu-id="7fd2d-113">Movies rating selected for Japan.</span></span> <span data-ttu-id="7fd2d-114">使用可能な値: `allAllowed`、`allBlocked`、`general`、`parentalGuidance`、`agesAbove15`、`agesAbove18`。</span><span class="sxs-lookup"><span data-stu-id="7fd2d-114">Possible values are: `allAllowed`, `allBlocked`, `general`, `parentalGuidance`, `agesAbove15`, `agesAbove18`.</span></span>|
|<span data-ttu-id="7fd2d-115">tvRating</span><span class="sxs-lookup"><span data-stu-id="7fd2d-115">tvRating</span></span>|[<span data-ttu-id="7fd2d-116">ratingJapanTelevisionType</span><span class="sxs-lookup"><span data-stu-id="7fd2d-116">ratingJapanTelevisionType</span></span>](../resources/intune-deviceconfig-ratingjapantelevisiontype.md)|<span data-ttu-id="7fd2d-117">日本向けに選択されているテレビのレーティング。</span><span class="sxs-lookup"><span data-stu-id="7fd2d-117">TV rating selected for Japan.</span></span> <span data-ttu-id="7fd2d-118">可能な値は、`allAllowed`、`allBlocked`、`explicitAllowed` です。</span><span class="sxs-lookup"><span data-stu-id="7fd2d-118">Possible values are: `allAllowed`, `allBlocked`, `explicitAllowed`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="7fd2d-119">関係</span><span class="sxs-lookup"><span data-stu-id="7fd2d-119">Relationships</span></span>
<span data-ttu-id="7fd2d-120">なし</span><span class="sxs-lookup"><span data-stu-id="7fd2d-120">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="7fd2d-121">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="7fd2d-121">JSON Representation</span></span>
<span data-ttu-id="7fd2d-122">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="7fd2d-122">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.mediaContentRatingJapan"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.mediaContentRatingJapan",
  "movieRating": "String",
  "tvRating": "String"
}
```




