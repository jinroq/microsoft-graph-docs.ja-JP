---
title: mediaContentRatingNewZealand リソースの種類
description: まだ文書化されていません
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 4c2d9d58413153699f93841470364cb673979a17
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32572368"
---
# <a name="mediacontentratingnewzealand-resource-type"></a><span data-ttu-id="7a237-103">mediaContentRatingNewZealand リソースの種類</span><span class="sxs-lookup"><span data-stu-id="7a237-103">mediaContentRatingNewZealand resource type</span></span>

> <span data-ttu-id="7a237-104">**注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="7a237-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="7a237-105">まだ文書化されていません</span><span class="sxs-lookup"><span data-stu-id="7a237-105">Not yet documented</span></span>

## <a name="properties"></a><span data-ttu-id="7a237-106">プロパティ</span><span class="sxs-lookup"><span data-stu-id="7a237-106">Properties</span></span>
|<span data-ttu-id="7a237-107">プロパティ</span><span class="sxs-lookup"><span data-stu-id="7a237-107">Property</span></span>|<span data-ttu-id="7a237-108">型</span><span class="sxs-lookup"><span data-stu-id="7a237-108">Type</span></span>|<span data-ttu-id="7a237-109">説明</span><span class="sxs-lookup"><span data-stu-id="7a237-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="7a237-110">movieRating</span><span class="sxs-lookup"><span data-stu-id="7a237-110">movieRating</span></span>|[<span data-ttu-id="7a237-111">ratingNewZealandMoviesType</span><span class="sxs-lookup"><span data-stu-id="7a237-111">ratingNewZealandMoviesType</span></span>](../resources/intune-deviceconfig-ratingnewzealandmoviestype.md)|<span data-ttu-id="7a237-112">ニュージーランドで選択されている映画のレーティング。</span><span class="sxs-lookup"><span data-stu-id="7a237-112">Movies rating selected for New Zealand.</span></span> <span data-ttu-id="7a237-113">使用可能な値は、`allAllowed`、`allBlocked`、`general`、`parentalGuidance`、`mature`、`agesAbove13`、`agesAbove15`、`agesAbove16`、`agesAbove18`、`restricted`、`agesAbove16Restricted` です。</span><span class="sxs-lookup"><span data-stu-id="7a237-113">Possible values are: `allAllowed`, `allBlocked`, `general`, `parentalGuidance`, `mature`, `agesAbove13`, `agesAbove15`, `agesAbove16`, `agesAbove18`, `restricted`, `agesAbove16Restricted`.</span></span>|
|<span data-ttu-id="7a237-114">tvRating</span><span class="sxs-lookup"><span data-stu-id="7a237-114">tvRating</span></span>|[<span data-ttu-id="7a237-115">ratingNewZealandTelevisionType</span><span class="sxs-lookup"><span data-stu-id="7a237-115">ratingNewZealandTelevisionType</span></span>](../resources/intune-deviceconfig-ratingnewzealandtelevisiontype.md)|<span data-ttu-id="7a237-116">ニュージーランド用に選択されているテレビのレーティング。</span><span class="sxs-lookup"><span data-stu-id="7a237-116">TV rating selected for New Zealand.</span></span> <span data-ttu-id="7a237-117">可能な値は、`allAllowed`、`allBlocked`、`general`、`parentalGuidance`、`adults` です。</span><span class="sxs-lookup"><span data-stu-id="7a237-117">Possible values are: `allAllowed`, `allBlocked`, `general`, `parentalGuidance`, `adults`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="7a237-118">関係</span><span class="sxs-lookup"><span data-stu-id="7a237-118">Relationships</span></span>
<span data-ttu-id="7a237-119">なし</span><span class="sxs-lookup"><span data-stu-id="7a237-119">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="7a237-120">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="7a237-120">JSON Representation</span></span>
<span data-ttu-id="7a237-121">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="7a237-121">Here is a JSON representation of the resource.</span></span>
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



