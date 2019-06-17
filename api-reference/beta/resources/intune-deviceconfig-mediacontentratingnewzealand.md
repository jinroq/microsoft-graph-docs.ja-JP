---
title: mediaContentRatingNewZealand リソースの種類
description: まだ文書化されていません
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: c69f2d22494e23783c39d781fee28ece49241b52
ms.sourcegitcommit: 0a62bc5849f27a55d83efce9b3eb01b9711bbe1d
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/14/2019
ms.locfileid: "34986761"
---
# <a name="mediacontentratingnewzealand-resource-type"></a><span data-ttu-id="75f07-103">mediaContentRatingNewZealand リソースの種類</span><span class="sxs-lookup"><span data-stu-id="75f07-103">mediaContentRatingNewZealand resource type</span></span>

> <span data-ttu-id="75f07-104">**重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="75f07-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="75f07-105">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="75f07-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="75f07-106">まだ文書化されていません</span><span class="sxs-lookup"><span data-stu-id="75f07-106">Not yet documented</span></span>

## <a name="properties"></a><span data-ttu-id="75f07-107">プロパティ</span><span class="sxs-lookup"><span data-stu-id="75f07-107">Properties</span></span>
|<span data-ttu-id="75f07-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="75f07-108">Property</span></span>|<span data-ttu-id="75f07-109">型</span><span class="sxs-lookup"><span data-stu-id="75f07-109">Type</span></span>|<span data-ttu-id="75f07-110">説明</span><span class="sxs-lookup"><span data-stu-id="75f07-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="75f07-111">movieRating</span><span class="sxs-lookup"><span data-stu-id="75f07-111">movieRating</span></span>|[<span data-ttu-id="75f07-112">ratingNewZealandMoviesType</span><span class="sxs-lookup"><span data-stu-id="75f07-112">ratingNewZealandMoviesType</span></span>](../resources/intune-deviceconfig-ratingnewzealandmoviestype.md)|<span data-ttu-id="75f07-113">ニュージーランドで選択されている映画のレーティング。</span><span class="sxs-lookup"><span data-stu-id="75f07-113">Movies rating selected for New Zealand.</span></span> <span data-ttu-id="75f07-114">使用可能な値は、`allAllowed`、`allBlocked`、`general`、`parentalGuidance`、`mature`、`agesAbove13`、`agesAbove15`、`agesAbove16`、`agesAbove18`、`restricted`、`agesAbove16Restricted` です。</span><span class="sxs-lookup"><span data-stu-id="75f07-114">Possible values are: `allAllowed`, `allBlocked`, `general`, `parentalGuidance`, `mature`, `agesAbove13`, `agesAbove15`, `agesAbove16`, `agesAbove18`, `restricted`, `agesAbove16Restricted`.</span></span>|
|<span data-ttu-id="75f07-115">tvRating</span><span class="sxs-lookup"><span data-stu-id="75f07-115">tvRating</span></span>|[<span data-ttu-id="75f07-116">ratingNewZealandTelevisionType</span><span class="sxs-lookup"><span data-stu-id="75f07-116">ratingNewZealandTelevisionType</span></span>](../resources/intune-deviceconfig-ratingnewzealandtelevisiontype.md)|<span data-ttu-id="75f07-117">ニュージーランド用に選択されているテレビのレーティング。</span><span class="sxs-lookup"><span data-stu-id="75f07-117">TV rating selected for New Zealand.</span></span> <span data-ttu-id="75f07-118">可能な値は、`allAllowed`、`allBlocked`、`general`、`parentalGuidance`、`adults` です。</span><span class="sxs-lookup"><span data-stu-id="75f07-118">Possible values are: `allAllowed`, `allBlocked`, `general`, `parentalGuidance`, `adults`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="75f07-119">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="75f07-119">Relationships</span></span>
<span data-ttu-id="75f07-120">なし</span><span class="sxs-lookup"><span data-stu-id="75f07-120">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="75f07-121">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="75f07-121">JSON Representation</span></span>
<span data-ttu-id="75f07-122">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="75f07-122">Here is a JSON representation of the resource.</span></span>
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





