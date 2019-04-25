---
title: mediaContentRatingJapan リソースの種類
description: まだ文書化されていません
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 0543aec86312d90a5896ed3f06f004c87d8e6a58
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32574181"
---
# <a name="mediacontentratingjapan-resource-type"></a><span data-ttu-id="a057e-103">mediaContentRatingJapan リソースの種類</span><span class="sxs-lookup"><span data-stu-id="a057e-103">mediaContentRatingJapan resource type</span></span>

> <span data-ttu-id="a057e-104">**注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="a057e-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="a057e-105">まだ文書化されていません</span><span class="sxs-lookup"><span data-stu-id="a057e-105">Not yet documented</span></span>

## <a name="properties"></a><span data-ttu-id="a057e-106">プロパティ</span><span class="sxs-lookup"><span data-stu-id="a057e-106">Properties</span></span>
|<span data-ttu-id="a057e-107">プロパティ</span><span class="sxs-lookup"><span data-stu-id="a057e-107">Property</span></span>|<span data-ttu-id="a057e-108">型</span><span class="sxs-lookup"><span data-stu-id="a057e-108">Type</span></span>|<span data-ttu-id="a057e-109">説明</span><span class="sxs-lookup"><span data-stu-id="a057e-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a057e-110">movieRating</span><span class="sxs-lookup"><span data-stu-id="a057e-110">movieRating</span></span>|[<span data-ttu-id="a057e-111">ratingJapanMoviesType</span><span class="sxs-lookup"><span data-stu-id="a057e-111">ratingJapanMoviesType</span></span>](../resources/intune-deviceconfig-ratingjapanmoviestype.md)|<span data-ttu-id="a057e-112">日本向けに選択されている映画のレーティング。</span><span class="sxs-lookup"><span data-stu-id="a057e-112">Movies rating selected for Japan.</span></span> <span data-ttu-id="a057e-113">使用可能な値: `allAllowed`、`allBlocked`、`general`、`parentalGuidance`、`agesAbove15`、`agesAbove18`。</span><span class="sxs-lookup"><span data-stu-id="a057e-113">Possible values are: `allAllowed`, `allBlocked`, `general`, `parentalGuidance`, `agesAbove15`, `agesAbove18`.</span></span>|
|<span data-ttu-id="a057e-114">tvRating</span><span class="sxs-lookup"><span data-stu-id="a057e-114">tvRating</span></span>|[<span data-ttu-id="a057e-115">ratingJapanTelevisionType</span><span class="sxs-lookup"><span data-stu-id="a057e-115">ratingJapanTelevisionType</span></span>](../resources/intune-deviceconfig-ratingjapantelevisiontype.md)|<span data-ttu-id="a057e-116">日本向けに選択されているテレビのレーティング。</span><span class="sxs-lookup"><span data-stu-id="a057e-116">TV rating selected for Japan.</span></span> <span data-ttu-id="a057e-117">可能な値は、`allAllowed`、`allBlocked`、`explicitAllowed` です。</span><span class="sxs-lookup"><span data-stu-id="a057e-117">Possible values are: `allAllowed`, `allBlocked`, `explicitAllowed`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="a057e-118">関係</span><span class="sxs-lookup"><span data-stu-id="a057e-118">Relationships</span></span>
<span data-ttu-id="a057e-119">なし</span><span class="sxs-lookup"><span data-stu-id="a057e-119">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="a057e-120">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="a057e-120">JSON Representation</span></span>
<span data-ttu-id="a057e-121">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="a057e-121">Here is a JSON representation of the resource.</span></span>
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



