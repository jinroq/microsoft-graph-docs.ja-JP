---
title: mediaContentRatingJapan リソースの種類
description: まだ文書化されていません
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 3b10d498edd03850a52aa09ba29e352a143a77c5
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 02/21/2019
ms.locfileid: "30163442"
---
# <a name="mediacontentratingjapan-resource-type"></a><span data-ttu-id="d90b4-103">mediaContentRatingJapan リソースの種類</span><span class="sxs-lookup"><span data-stu-id="d90b4-103">mediaContentRatingJapan resource type</span></span>

> <span data-ttu-id="d90b4-104">**重要:** ベータ版の Microsoft Graph api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="d90b4-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="d90b4-105">**注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="d90b4-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="d90b4-106">まだ文書化されていません</span><span class="sxs-lookup"><span data-stu-id="d90b4-106">Not yet documented</span></span>

## <a name="properties"></a><span data-ttu-id="d90b4-107">プロパティ</span><span class="sxs-lookup"><span data-stu-id="d90b4-107">Properties</span></span>
|<span data-ttu-id="d90b4-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="d90b4-108">Property</span></span>|<span data-ttu-id="d90b4-109">型</span><span class="sxs-lookup"><span data-stu-id="d90b4-109">Type</span></span>|<span data-ttu-id="d90b4-110">説明</span><span class="sxs-lookup"><span data-stu-id="d90b4-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d90b4-111">movieRating</span><span class="sxs-lookup"><span data-stu-id="d90b4-111">movieRating</span></span>|[<span data-ttu-id="d90b4-112">ratingJapanMoviesType</span><span class="sxs-lookup"><span data-stu-id="d90b4-112">ratingJapanMoviesType</span></span>](../resources/intune-deviceconfig-ratingjapanmoviestype.md)|<span data-ttu-id="d90b4-113">日本向けに選択されている映画のレーティング。</span><span class="sxs-lookup"><span data-stu-id="d90b4-113">Movies rating selected for Japan.</span></span> <span data-ttu-id="d90b4-114">使用可能な値: `allAllowed`、`allBlocked`、`general`、`parentalGuidance`、`agesAbove15`、`agesAbove18`。</span><span class="sxs-lookup"><span data-stu-id="d90b4-114">Possible values are: `allAllowed`, `allBlocked`, `general`, `parentalGuidance`, `agesAbove15`, `agesAbove18`.</span></span>|
|<span data-ttu-id="d90b4-115">tvRating</span><span class="sxs-lookup"><span data-stu-id="d90b4-115">tvRating</span></span>|[<span data-ttu-id="d90b4-116">ratingJapanTelevisionType</span><span class="sxs-lookup"><span data-stu-id="d90b4-116">ratingJapanTelevisionType</span></span>](../resources/intune-deviceconfig-ratingjapantelevisiontype.md)|<span data-ttu-id="d90b4-117">日本向けに選択されているテレビのレーティング。</span><span class="sxs-lookup"><span data-stu-id="d90b4-117">TV rating selected for Japan.</span></span> <span data-ttu-id="d90b4-118">可能な値は、`allAllowed`、`allBlocked`、`explicitAllowed` です。</span><span class="sxs-lookup"><span data-stu-id="d90b4-118">Possible values are: `allAllowed`, `allBlocked`, `explicitAllowed`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="d90b4-119">関係</span><span class="sxs-lookup"><span data-stu-id="d90b4-119">Relationships</span></span>
<span data-ttu-id="d90b4-120">なし</span><span class="sxs-lookup"><span data-stu-id="d90b4-120">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="d90b4-121">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="d90b4-121">JSON Representation</span></span>
<span data-ttu-id="d90b4-122">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="d90b4-122">Here is a JSON representation of the resource.</span></span>
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




