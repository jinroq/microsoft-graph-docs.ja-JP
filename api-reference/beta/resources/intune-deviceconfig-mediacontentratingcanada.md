---
title: mediaContentRatingCanada リソースの種類
description: まだ文書化されていません
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 38f3bac4e8410a3c63bd07319888ab0a5fc7df19
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 02/21/2019
ms.locfileid: "30146348"
---
# <a name="mediacontentratingcanada-resource-type"></a><span data-ttu-id="bbe77-103">mediaContentRatingCanada リソースの種類</span><span class="sxs-lookup"><span data-stu-id="bbe77-103">mediaContentRatingCanada resource type</span></span>

> <span data-ttu-id="bbe77-104">**重要:** ベータ版の Microsoft Graph api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="bbe77-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="bbe77-105">**注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="bbe77-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="bbe77-106">まだ文書化されていません</span><span class="sxs-lookup"><span data-stu-id="bbe77-106">Not yet documented</span></span>

## <a name="properties"></a><span data-ttu-id="bbe77-107">プロパティ</span><span class="sxs-lookup"><span data-stu-id="bbe77-107">Properties</span></span>
|<span data-ttu-id="bbe77-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="bbe77-108">Property</span></span>|<span data-ttu-id="bbe77-109">型</span><span class="sxs-lookup"><span data-stu-id="bbe77-109">Type</span></span>|<span data-ttu-id="bbe77-110">説明</span><span class="sxs-lookup"><span data-stu-id="bbe77-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="bbe77-111">movieRating</span><span class="sxs-lookup"><span data-stu-id="bbe77-111">movieRating</span></span>|[<span data-ttu-id="bbe77-112">ratingCanadaMoviesType</span><span class="sxs-lookup"><span data-stu-id="bbe77-112">ratingCanadaMoviesType</span></span>](../resources/intune-deviceconfig-ratingcanadamoviestype.md)|<span data-ttu-id="bbe77-113">カナダ向けに選択されている映画のレーティング。</span><span class="sxs-lookup"><span data-stu-id="bbe77-113">Movies rating selected for Canada.</span></span> <span data-ttu-id="bbe77-114">可能な値は、`allAllowed`、`allBlocked`、`general`、`parentalGuidance`、`agesAbove14`、`agesAbove18`、`restricted` です。</span><span class="sxs-lookup"><span data-stu-id="bbe77-114">Possible values are: `allAllowed`, `allBlocked`, `general`, `parentalGuidance`, `agesAbove14`, `agesAbove18`, `restricted`.</span></span>|
|<span data-ttu-id="bbe77-115">tvRating</span><span class="sxs-lookup"><span data-stu-id="bbe77-115">tvRating</span></span>|[<span data-ttu-id="bbe77-116">ratingCanadaTelevisionType</span><span class="sxs-lookup"><span data-stu-id="bbe77-116">ratingCanadaTelevisionType</span></span>](../resources/intune-deviceconfig-ratingcanadatelevisiontype.md)|<span data-ttu-id="bbe77-117">カナダ向けに選択されているテレビのレーティング。</span><span class="sxs-lookup"><span data-stu-id="bbe77-117">TV rating selected for Canada.</span></span> <span data-ttu-id="bbe77-118">可能な値は、`allAllowed`、`allBlocked`、`children`、`childrenAbove8`、`general`、`parentalGuidance`、`agesAbove14`、`agesAbove18` です。</span><span class="sxs-lookup"><span data-stu-id="bbe77-118">Possible values are: `allAllowed`, `allBlocked`, `children`, `childrenAbove8`, `general`, `parentalGuidance`, `agesAbove14`, `agesAbove18`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="bbe77-119">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="bbe77-119">Relationships</span></span>
<span data-ttu-id="bbe77-120">なし</span><span class="sxs-lookup"><span data-stu-id="bbe77-120">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="bbe77-121">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="bbe77-121">JSON Representation</span></span>
<span data-ttu-id="bbe77-122">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="bbe77-122">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.mediaContentRatingCanada"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.mediaContentRatingCanada",
  "movieRating": "String",
  "tvRating": "String"
}
```




