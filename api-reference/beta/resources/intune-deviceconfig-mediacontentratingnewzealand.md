---
title: mediaContentRatingNewZealand リソースの種類
description: まだ文書化されていません
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 4ea4656e24afe5d78bac2b4a69f51c145de2708d
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "35970088"
---
# <a name="mediacontentratingnewzealand-resource-type"></a><span data-ttu-id="d7cd8-103">mediaContentRatingNewZealand リソースの種類</span><span class="sxs-lookup"><span data-stu-id="d7cd8-103">mediaContentRatingNewZealand resource type</span></span>

> <span data-ttu-id="d7cd8-104">**重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="d7cd8-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="d7cd8-105">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="d7cd8-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="d7cd8-106">まだ文書化されていません</span><span class="sxs-lookup"><span data-stu-id="d7cd8-106">Not yet documented</span></span>

## <a name="properties"></a><span data-ttu-id="d7cd8-107">プロパティ</span><span class="sxs-lookup"><span data-stu-id="d7cd8-107">Properties</span></span>
|<span data-ttu-id="d7cd8-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="d7cd8-108">Property</span></span>|<span data-ttu-id="d7cd8-109">型</span><span class="sxs-lookup"><span data-stu-id="d7cd8-109">Type</span></span>|<span data-ttu-id="d7cd8-110">説明</span><span class="sxs-lookup"><span data-stu-id="d7cd8-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d7cd8-111">movieRating</span><span class="sxs-lookup"><span data-stu-id="d7cd8-111">movieRating</span></span>|[<span data-ttu-id="d7cd8-112">ratingNewZealandMoviesType</span><span class="sxs-lookup"><span data-stu-id="d7cd8-112">ratingNewZealandMoviesType</span></span>](../resources/intune-deviceconfig-ratingnewzealandmoviestype.md)|<span data-ttu-id="d7cd8-113">ニュージーランドで選択されている映画のレーティング。</span><span class="sxs-lookup"><span data-stu-id="d7cd8-113">Movies rating selected for New Zealand.</span></span> <span data-ttu-id="d7cd8-114">使用可能な値は、`allAllowed`、`allBlocked`、`general`、`parentalGuidance`、`mature`、`agesAbove13`、`agesAbove15`、`agesAbove16`、`agesAbove18`、`restricted`、`agesAbove16Restricted` です。</span><span class="sxs-lookup"><span data-stu-id="d7cd8-114">Possible values are: `allAllowed`, `allBlocked`, `general`, `parentalGuidance`, `mature`, `agesAbove13`, `agesAbove15`, `agesAbove16`, `agesAbove18`, `restricted`, `agesAbove16Restricted`.</span></span>|
|<span data-ttu-id="d7cd8-115">tvRating</span><span class="sxs-lookup"><span data-stu-id="d7cd8-115">tvRating</span></span>|[<span data-ttu-id="d7cd8-116">ratingNewZealandTelevisionType</span><span class="sxs-lookup"><span data-stu-id="d7cd8-116">ratingNewZealandTelevisionType</span></span>](../resources/intune-deviceconfig-ratingnewzealandtelevisiontype.md)|<span data-ttu-id="d7cd8-117">ニュージーランド用に選択されているテレビのレーティング。</span><span class="sxs-lookup"><span data-stu-id="d7cd8-117">TV rating selected for New Zealand.</span></span> <span data-ttu-id="d7cd8-118">可能な値は、`allAllowed`、`allBlocked`、`general`、`parentalGuidance`、`adults` です。</span><span class="sxs-lookup"><span data-stu-id="d7cd8-118">Possible values are: `allAllowed`, `allBlocked`, `general`, `parentalGuidance`, `adults`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="d7cd8-119">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="d7cd8-119">Relationships</span></span>
<span data-ttu-id="d7cd8-120">なし</span><span class="sxs-lookup"><span data-stu-id="d7cd8-120">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="d7cd8-121">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="d7cd8-121">JSON Representation</span></span>
<span data-ttu-id="d7cd8-122">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="d7cd8-122">Here is a JSON representation of the resource.</span></span>
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





