---
title: mediaContentRatingNewZealand リソースの種類
description: まだ文書化されていません
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 9d06658905a5a6e5aaab79bb159a87fe4cb5cf7a
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "36031396"
---
# <a name="mediacontentratingnewzealand-resource-type"></a><span data-ttu-id="08383-103">mediaContentRatingNewZealand リソースの種類</span><span class="sxs-lookup"><span data-stu-id="08383-103">mediaContentRatingNewZealand resource type</span></span>

> <span data-ttu-id="08383-104">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="08383-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="08383-105">まだ文書化されていません</span><span class="sxs-lookup"><span data-stu-id="08383-105">Not yet documented</span></span>

## <a name="properties"></a><span data-ttu-id="08383-106">プロパティ</span><span class="sxs-lookup"><span data-stu-id="08383-106">Properties</span></span>
|<span data-ttu-id="08383-107">プロパティ</span><span class="sxs-lookup"><span data-stu-id="08383-107">Property</span></span>|<span data-ttu-id="08383-108">型</span><span class="sxs-lookup"><span data-stu-id="08383-108">Type</span></span>|<span data-ttu-id="08383-109">説明</span><span class="sxs-lookup"><span data-stu-id="08383-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="08383-110">movieRating</span><span class="sxs-lookup"><span data-stu-id="08383-110">movieRating</span></span>|[<span data-ttu-id="08383-111">ratingNewZealandMoviesType</span><span class="sxs-lookup"><span data-stu-id="08383-111">ratingNewZealandMoviesType</span></span>](../resources/intune-deviceconfig-ratingnewzealandmoviestype.md)|<span data-ttu-id="08383-112">ニュージーランドで選択されている映画のレーティング。</span><span class="sxs-lookup"><span data-stu-id="08383-112">Movies rating selected for New Zealand.</span></span> <span data-ttu-id="08383-113">使用可能な値は、`allAllowed`、`allBlocked`、`general`、`parentalGuidance`、`mature`、`agesAbove13`、`agesAbove15`、`agesAbove16`、`agesAbove18`、`restricted`、`agesAbove16Restricted` です。</span><span class="sxs-lookup"><span data-stu-id="08383-113">Possible values are: `allAllowed`, `allBlocked`, `general`, `parentalGuidance`, `mature`, `agesAbove13`, `agesAbove15`, `agesAbove16`, `agesAbove18`, `restricted`, `agesAbove16Restricted`.</span></span>|
|<span data-ttu-id="08383-114">tvRating</span><span class="sxs-lookup"><span data-stu-id="08383-114">tvRating</span></span>|[<span data-ttu-id="08383-115">ratingNewZealandTelevisionType</span><span class="sxs-lookup"><span data-stu-id="08383-115">ratingNewZealandTelevisionType</span></span>](../resources/intune-deviceconfig-ratingnewzealandtelevisiontype.md)|<span data-ttu-id="08383-116">ニュージーランド用に選択されているテレビのレーティング。</span><span class="sxs-lookup"><span data-stu-id="08383-116">TV rating selected for New Zealand.</span></span> <span data-ttu-id="08383-117">可能な値は、`allAllowed`、`allBlocked`、`general`、`parentalGuidance`、`adults` です。</span><span class="sxs-lookup"><span data-stu-id="08383-117">Possible values are: `allAllowed`, `allBlocked`, `general`, `parentalGuidance`, `adults`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="08383-118">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="08383-118">Relationships</span></span>
<span data-ttu-id="08383-119">なし</span><span class="sxs-lookup"><span data-stu-id="08383-119">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="08383-120">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="08383-120">JSON Representation</span></span>
<span data-ttu-id="08383-121">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="08383-121">Here is a JSON representation of the resource.</span></span>
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



