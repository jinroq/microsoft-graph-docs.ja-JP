---
title: mediaContentRatingCanada リソースの種類
description: まだ文書化されていません
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 292dc926a626a2aca96312133eb6c9a850db39af
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/23/2019
ms.locfileid: "29398052"
---
# <a name="mediacontentratingcanada-resource-type"></a><span data-ttu-id="4347d-103">mediaContentRatingCanada リソースの種類</span><span class="sxs-lookup"><span data-stu-id="4347d-103">mediaContentRatingCanada resource type</span></span>

> <span data-ttu-id="4347d-104">**重要な:**[Microsoft Graph で/beta のバージョンの Api は予告なしに変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="4347d-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="4347d-105">実稼働アプリケーションでこれらの API を使用することは、サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="4347d-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="4347d-106">**注:** Intune の Microsoft グラフ API では、テナントの[Intune のアクティブなライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="4347d-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="4347d-107">まだ文書化されていません</span><span class="sxs-lookup"><span data-stu-id="4347d-107">Not yet documented</span></span>

## <a name="properties"></a><span data-ttu-id="4347d-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="4347d-108">Properties</span></span>
|<span data-ttu-id="4347d-109">プロパティ</span><span class="sxs-lookup"><span data-stu-id="4347d-109">Property</span></span>|<span data-ttu-id="4347d-110">型</span><span class="sxs-lookup"><span data-stu-id="4347d-110">Type</span></span>|<span data-ttu-id="4347d-111">説明</span><span class="sxs-lookup"><span data-stu-id="4347d-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="4347d-112">movieRating</span><span class="sxs-lookup"><span data-stu-id="4347d-112">movieRating</span></span>|[<span data-ttu-id="4347d-113">ratingCanadaMoviesType</span><span class="sxs-lookup"><span data-stu-id="4347d-113">ratingCanadaMoviesType</span></span>](../resources/intune-deviceconfig-ratingcanadamoviestype.md)|<span data-ttu-id="4347d-114">評価のカナダの選択したムービーです。</span><span class="sxs-lookup"><span data-stu-id="4347d-114">Movies rating selected for Canada.</span></span> <span data-ttu-id="4347d-115">可能な値は、`allAllowed`、`allBlocked`、`general`、`parentalGuidance`、`agesAbove14`、`agesAbove18`、`restricted` です。</span><span class="sxs-lookup"><span data-stu-id="4347d-115">Possible values are: `allAllowed`, `allBlocked`, `general`, `parentalGuidance`, `agesAbove14`, `agesAbove18`, `restricted`.</span></span>|
|<span data-ttu-id="4347d-116">tvRating</span><span class="sxs-lookup"><span data-stu-id="4347d-116">tvRating</span></span>|[<span data-ttu-id="4347d-117">ratingCanadaTelevisionType</span><span class="sxs-lookup"><span data-stu-id="4347d-117">ratingCanadaTelevisionType</span></span>](../resources/intune-deviceconfig-ratingcanadatelevisiontype.md)|<span data-ttu-id="4347d-118">テレビの視聴制限がカナダを選択します。</span><span class="sxs-lookup"><span data-stu-id="4347d-118">TV rating selected for Canada.</span></span> <span data-ttu-id="4347d-119">可能な値は、`allAllowed`、`allBlocked`、`children`、`childrenAbove8`、`general`、`parentalGuidance`、`agesAbove14`、`agesAbove18` です。</span><span class="sxs-lookup"><span data-stu-id="4347d-119">Possible values are: `allAllowed`, `allBlocked`, `children`, `childrenAbove8`, `general`, `parentalGuidance`, `agesAbove14`, `agesAbove18`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="4347d-120">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="4347d-120">Relationships</span></span>
<span data-ttu-id="4347d-121">なし</span><span class="sxs-lookup"><span data-stu-id="4347d-121">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="4347d-122">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="4347d-122">JSON Representation</span></span>
<span data-ttu-id="4347d-123">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="4347d-123">Here is a JSON representation of the resource.</span></span>
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




