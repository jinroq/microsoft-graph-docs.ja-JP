---
title: mediaContentRatingNewZealand リソースの種類
description: まだ文書化されていません
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: adfc34cf65104f0bf370a4e1ba22cfcb78bf250b
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/23/2019
ms.locfileid: "29403449"
---
# <a name="mediacontentratingnewzealand-resource-type"></a><span data-ttu-id="adf56-103">mediaContentRatingNewZealand リソースの種類</span><span class="sxs-lookup"><span data-stu-id="adf56-103">mediaContentRatingNewZealand resource type</span></span>

> <span data-ttu-id="adf56-104">**重要な:**[Microsoft Graph で/beta のバージョンの Api は予告なしに変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="adf56-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="adf56-105">実稼働アプリケーションでこれらの API を使用することは、サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="adf56-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="adf56-106">**注:** Intune の Microsoft グラフ API では、テナントの[Intune のアクティブなライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="adf56-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="adf56-107">まだ文書化されていません</span><span class="sxs-lookup"><span data-stu-id="adf56-107">Not yet documented</span></span>

## <a name="properties"></a><span data-ttu-id="adf56-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="adf56-108">Properties</span></span>
|<span data-ttu-id="adf56-109">プロパティ</span><span class="sxs-lookup"><span data-stu-id="adf56-109">Property</span></span>|<span data-ttu-id="adf56-110">型</span><span class="sxs-lookup"><span data-stu-id="adf56-110">Type</span></span>|<span data-ttu-id="adf56-111">説明</span><span class="sxs-lookup"><span data-stu-id="adf56-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="adf56-112">movieRating</span><span class="sxs-lookup"><span data-stu-id="adf56-112">movieRating</span></span>|[<span data-ttu-id="adf56-113">ratingNewZealandMoviesType</span><span class="sxs-lookup"><span data-stu-id="adf56-113">ratingNewZealandMoviesType</span></span>](../resources/intune-deviceconfig-ratingnewzealandmoviestype.md)|<span data-ttu-id="adf56-114">評価のニュージーランドを選択したムービーです。</span><span class="sxs-lookup"><span data-stu-id="adf56-114">Movies rating selected for New Zealand.</span></span> <span data-ttu-id="adf56-115">可能な値は、`allAllowed`、`allBlocked`、`general`、`parentalGuidance`、`mature`、`agesAbove13`、`agesAbove15`、`agesAbove16`、`agesAbove18`、`restricted`、`agesAbove16Restricted` です。</span><span class="sxs-lookup"><span data-stu-id="adf56-115">Possible values are: `allAllowed`, `allBlocked`, `general`, `parentalGuidance`, `mature`, `agesAbove13`, `agesAbove15`, `agesAbove16`, `agesAbove18`, `restricted`, `agesAbove16Restricted`.</span></span>|
|<span data-ttu-id="adf56-116">tvRating</span><span class="sxs-lookup"><span data-stu-id="adf56-116">tvRating</span></span>|[<span data-ttu-id="adf56-117">ratingNewZealandTelevisionType</span><span class="sxs-lookup"><span data-stu-id="adf56-117">ratingNewZealandTelevisionType</span></span>](../resources/intune-deviceconfig-ratingnewzealandtelevisiontype.md)|<span data-ttu-id="adf56-118">テレビの視聴制限がニュージーランドを選択します。</span><span class="sxs-lookup"><span data-stu-id="adf56-118">TV rating selected for New Zealand.</span></span> <span data-ttu-id="adf56-119">可能な値は、`allAllowed`、`allBlocked`、`general`、`parentalGuidance`、`adults` です。</span><span class="sxs-lookup"><span data-stu-id="adf56-119">Possible values are: `allAllowed`, `allBlocked`, `general`, `parentalGuidance`, `adults`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="adf56-120">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="adf56-120">Relationships</span></span>
<span data-ttu-id="adf56-121">なし</span><span class="sxs-lookup"><span data-stu-id="adf56-121">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="adf56-122">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="adf56-122">JSON Representation</span></span>
<span data-ttu-id="adf56-123">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="adf56-123">Here is a JSON representation of the resource.</span></span>
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




