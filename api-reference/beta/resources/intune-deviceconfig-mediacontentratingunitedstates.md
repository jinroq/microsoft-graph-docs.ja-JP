---
title: mediaContentRatingUnitedStates リソースの種類
description: まだ文書化されていません
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: f085bc24c3c5bd7b510ee5fa0a0b841361c0269e
ms.sourcegitcommit: 94aaf594c881c02f353c6a417460cdf783a0bfe0
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/11/2019
ms.locfileid: "33950761"
---
# <a name="mediacontentratingunitedstates-resource-type"></a><span data-ttu-id="5c47a-103">mediaContentRatingUnitedStates リソースの種類</span><span class="sxs-lookup"><span data-stu-id="5c47a-103">mediaContentRatingUnitedStates resource type</span></span>

> <span data-ttu-id="5c47a-104">**重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="5c47a-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="5c47a-105">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="5c47a-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="5c47a-106">まだ文書化されていません</span><span class="sxs-lookup"><span data-stu-id="5c47a-106">Not yet documented</span></span>

## <a name="properties"></a><span data-ttu-id="5c47a-107">プロパティ</span><span class="sxs-lookup"><span data-stu-id="5c47a-107">Properties</span></span>
|<span data-ttu-id="5c47a-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="5c47a-108">Property</span></span>|<span data-ttu-id="5c47a-109">型</span><span class="sxs-lookup"><span data-stu-id="5c47a-109">Type</span></span>|<span data-ttu-id="5c47a-110">説明</span><span class="sxs-lookup"><span data-stu-id="5c47a-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="5c47a-111">movieRating</span><span class="sxs-lookup"><span data-stu-id="5c47a-111">movieRating</span></span>|[<span data-ttu-id="5c47a-112">ratingUnitedStatesMoviesType</span><span class="sxs-lookup"><span data-stu-id="5c47a-112">ratingUnitedStatesMoviesType</span></span>](../resources/intune-deviceconfig-ratingunitedstatesmoviestype.md)|<span data-ttu-id="5c47a-113">米国向けに選択されている映画のレーティング。</span><span class="sxs-lookup"><span data-stu-id="5c47a-113">Movies rating selected for United States.</span></span> <span data-ttu-id="5c47a-114">可能な値は、`allAllowed`、`allBlocked`、`general`、`parentalGuidance`、`parentalGuidance13`、`restricted`、`adults` です。</span><span class="sxs-lookup"><span data-stu-id="5c47a-114">Possible values are: `allAllowed`, `allBlocked`, `general`, `parentalGuidance`, `parentalGuidance13`, `restricted`, `adults`.</span></span>|
|<span data-ttu-id="5c47a-115">tvRating</span><span class="sxs-lookup"><span data-stu-id="5c47a-115">tvRating</span></span>|[<span data-ttu-id="5c47a-116">ratingUnitedStatesTelevisionType</span><span class="sxs-lookup"><span data-stu-id="5c47a-116">ratingUnitedStatesTelevisionType</span></span>](../resources/intune-deviceconfig-ratingunitedstatestelevisiontype.md)|<span data-ttu-id="5c47a-117">米国向けに選択されているテレビのレーティング。</span><span class="sxs-lookup"><span data-stu-id="5c47a-117">TV rating selected for United States.</span></span> <span data-ttu-id="5c47a-118">可能な値は、`allAllowed`、`allBlocked`、`childrenAll`、`childrenAbove7`、`general`、`parentalGuidance`、`childrenAbove14`、`adults` です。</span><span class="sxs-lookup"><span data-stu-id="5c47a-118">Possible values are: `allAllowed`, `allBlocked`, `childrenAll`, `childrenAbove7`, `general`, `parentalGuidance`, `childrenAbove14`, `adults`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="5c47a-119">関係</span><span class="sxs-lookup"><span data-stu-id="5c47a-119">Relationships</span></span>
<span data-ttu-id="5c47a-120">なし</span><span class="sxs-lookup"><span data-stu-id="5c47a-120">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="5c47a-121">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="5c47a-121">JSON Representation</span></span>
<span data-ttu-id="5c47a-122">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="5c47a-122">Here is a JSON representation of the resource.</span></span>
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




