---
title: mediaContentRatingUnitedStates リソースの種類
description: まだ文書化されていません
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 60f673e31014eb4da027a58ea29099d9d8aa18e3
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/23/2019
ms.locfileid: "29425835"
---
# <a name="mediacontentratingunitedstates-resource-type"></a><span data-ttu-id="36551-103">mediaContentRatingUnitedStates リソースの種類</span><span class="sxs-lookup"><span data-stu-id="36551-103">mediaContentRatingUnitedStates resource type</span></span>

> <span data-ttu-id="36551-104">**重要な:**[Microsoft Graph で/beta のバージョンの Api は予告なしに変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="36551-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="36551-105">実稼働アプリケーションでこれらの API を使用することは、サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="36551-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="36551-106">**注:** Intune の Microsoft グラフ API では、テナントの[Intune のアクティブなライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="36551-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="36551-107">まだ文書化されていません</span><span class="sxs-lookup"><span data-stu-id="36551-107">Not yet documented</span></span>

## <a name="properties"></a><span data-ttu-id="36551-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="36551-108">Properties</span></span>
|<span data-ttu-id="36551-109">プロパティ</span><span class="sxs-lookup"><span data-stu-id="36551-109">Property</span></span>|<span data-ttu-id="36551-110">型</span><span class="sxs-lookup"><span data-stu-id="36551-110">Type</span></span>|<span data-ttu-id="36551-111">説明</span><span class="sxs-lookup"><span data-stu-id="36551-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="36551-112">movieRating</span><span class="sxs-lookup"><span data-stu-id="36551-112">movieRating</span></span>|[<span data-ttu-id="36551-113">ratingUnitedStatesMoviesType</span><span class="sxs-lookup"><span data-stu-id="36551-113">ratingUnitedStatesMoviesType</span></span>](../resources/intune-deviceconfig-ratingunitedstatesmoviestype.md)|<span data-ttu-id="36551-114">評価の米国の選択したムービーです。</span><span class="sxs-lookup"><span data-stu-id="36551-114">Movies rating selected for United States.</span></span> <span data-ttu-id="36551-115">可能な値は、`allAllowed`、`allBlocked`、`general`、`parentalGuidance`、`parentalGuidance13`、`restricted`、`adults` です。</span><span class="sxs-lookup"><span data-stu-id="36551-115">Possible values are: `allAllowed`, `allBlocked`, `general`, `parentalGuidance`, `parentalGuidance13`, `restricted`, `adults`.</span></span>|
|<span data-ttu-id="36551-116">tvRating</span><span class="sxs-lookup"><span data-stu-id="36551-116">tvRating</span></span>|[<span data-ttu-id="36551-117">ratingUnitedStatesTelevisionType</span><span class="sxs-lookup"><span data-stu-id="36551-117">ratingUnitedStatesTelevisionType</span></span>](../resources/intune-deviceconfig-ratingunitedstatestelevisiontype.md)|<span data-ttu-id="36551-118">テレビの視聴制限はアメリカ合衆国を選択します。</span><span class="sxs-lookup"><span data-stu-id="36551-118">TV rating selected for United States.</span></span> <span data-ttu-id="36551-119">可能な値は、`allAllowed`、`allBlocked`、`childrenAll`、`childrenAbove7`、`general`、`parentalGuidance`、`childrenAbove14`、`adults` です。</span><span class="sxs-lookup"><span data-stu-id="36551-119">Possible values are: `allAllowed`, `allBlocked`, `childrenAll`, `childrenAbove7`, `general`, `parentalGuidance`, `childrenAbove14`, `adults`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="36551-120">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="36551-120">Relationships</span></span>
<span data-ttu-id="36551-121">なし</span><span class="sxs-lookup"><span data-stu-id="36551-121">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="36551-122">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="36551-122">JSON Representation</span></span>
<span data-ttu-id="36551-123">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="36551-123">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.mediaContentRatingUnitedStates"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.mediaContentRatingUnitedStates",
  "movieRating": "String",
  "tvRating": "String"
}
```




