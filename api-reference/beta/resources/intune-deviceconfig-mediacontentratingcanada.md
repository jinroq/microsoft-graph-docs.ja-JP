---
title: mediaContentRatingCanada リソースの種類
description: まだ文書化されていません
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 5c4c5f863fb20833586d7ea97ea59d293d702870
ms.sourcegitcommit: 94aaf594c881c02f353c6a417460cdf783a0bfe0
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/11/2019
ms.locfileid: "33944860"
---
# <a name="mediacontentratingcanada-resource-type"></a><span data-ttu-id="95a09-103">mediaContentRatingCanada リソースの種類</span><span class="sxs-lookup"><span data-stu-id="95a09-103">mediaContentRatingCanada resource type</span></span>

> <span data-ttu-id="95a09-104">**重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="95a09-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="95a09-105">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="95a09-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="95a09-106">まだ文書化されていません</span><span class="sxs-lookup"><span data-stu-id="95a09-106">Not yet documented</span></span>

## <a name="properties"></a><span data-ttu-id="95a09-107">プロパティ</span><span class="sxs-lookup"><span data-stu-id="95a09-107">Properties</span></span>
|<span data-ttu-id="95a09-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="95a09-108">Property</span></span>|<span data-ttu-id="95a09-109">型</span><span class="sxs-lookup"><span data-stu-id="95a09-109">Type</span></span>|<span data-ttu-id="95a09-110">説明</span><span class="sxs-lookup"><span data-stu-id="95a09-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="95a09-111">movieRating</span><span class="sxs-lookup"><span data-stu-id="95a09-111">movieRating</span></span>|[<span data-ttu-id="95a09-112">ratingCanadaMoviesType</span><span class="sxs-lookup"><span data-stu-id="95a09-112">ratingCanadaMoviesType</span></span>](../resources/intune-deviceconfig-ratingcanadamoviestype.md)|<span data-ttu-id="95a09-113">カナダ向けに選択されている映画のレーティング。</span><span class="sxs-lookup"><span data-stu-id="95a09-113">Movies rating selected for Canada.</span></span> <span data-ttu-id="95a09-114">可能な値は、`allAllowed`、`allBlocked`、`general`、`parentalGuidance`、`agesAbove14`、`agesAbove18`、`restricted` です。</span><span class="sxs-lookup"><span data-stu-id="95a09-114">Possible values are: `allAllowed`, `allBlocked`, `general`, `parentalGuidance`, `agesAbove14`, `agesAbove18`, `restricted`.</span></span>|
|<span data-ttu-id="95a09-115">tvRating</span><span class="sxs-lookup"><span data-stu-id="95a09-115">tvRating</span></span>|[<span data-ttu-id="95a09-116">ratingCanadaTelevisionType</span><span class="sxs-lookup"><span data-stu-id="95a09-116">ratingCanadaTelevisionType</span></span>](../resources/intune-deviceconfig-ratingcanadatelevisiontype.md)|<span data-ttu-id="95a09-117">カナダ向けに選択されているテレビのレーティング。</span><span class="sxs-lookup"><span data-stu-id="95a09-117">TV rating selected for Canada.</span></span> <span data-ttu-id="95a09-118">可能な値は、`allAllowed`、`allBlocked`、`children`、`childrenAbove8`、`general`、`parentalGuidance`、`agesAbove14`、`agesAbove18` です。</span><span class="sxs-lookup"><span data-stu-id="95a09-118">Possible values are: `allAllowed`, `allBlocked`, `children`, `childrenAbove8`, `general`, `parentalGuidance`, `agesAbove14`, `agesAbove18`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="95a09-119">関係</span><span class="sxs-lookup"><span data-stu-id="95a09-119">Relationships</span></span>
<span data-ttu-id="95a09-120">なし</span><span class="sxs-lookup"><span data-stu-id="95a09-120">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="95a09-121">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="95a09-121">JSON Representation</span></span>
<span data-ttu-id="95a09-122">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="95a09-122">Here is a JSON representation of the resource.</span></span>
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




