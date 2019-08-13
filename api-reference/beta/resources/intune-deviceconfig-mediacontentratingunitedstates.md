---
title: mediaContentRatingUnitedStates リソースの種類
description: まだ文書化されていません
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: bb659bfb8fc193e477270e635cecf9f94c7ca114
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/13/2019
ms.locfileid: "36368661"
---
# <a name="mediacontentratingunitedstates-resource-type"></a><span data-ttu-id="22277-103">mediaContentRatingUnitedStates リソースの種類</span><span class="sxs-lookup"><span data-stu-id="22277-103">mediaContentRatingUnitedStates resource type</span></span>

> <span data-ttu-id="22277-104">**重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="22277-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="22277-105">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="22277-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="22277-106">まだ文書化されていません</span><span class="sxs-lookup"><span data-stu-id="22277-106">Not yet documented</span></span>

## <a name="properties"></a><span data-ttu-id="22277-107">プロパティ</span><span class="sxs-lookup"><span data-stu-id="22277-107">Properties</span></span>
|<span data-ttu-id="22277-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="22277-108">Property</span></span>|<span data-ttu-id="22277-109">型</span><span class="sxs-lookup"><span data-stu-id="22277-109">Type</span></span>|<span data-ttu-id="22277-110">説明</span><span class="sxs-lookup"><span data-stu-id="22277-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="22277-111">movieRating</span><span class="sxs-lookup"><span data-stu-id="22277-111">movieRating</span></span>|[<span data-ttu-id="22277-112">ratingUnitedStatesMoviesType</span><span class="sxs-lookup"><span data-stu-id="22277-112">ratingUnitedStatesMoviesType</span></span>](../resources/intune-deviceconfig-ratingunitedstatesmoviestype.md)|<span data-ttu-id="22277-113">米国向けに選択されている映画のレーティング。</span><span class="sxs-lookup"><span data-stu-id="22277-113">Movies rating selected for United States.</span></span> <span data-ttu-id="22277-114">可能な値は、`allAllowed`、`allBlocked`、`general`、`parentalGuidance`、`parentalGuidance13`、`restricted`、`adults` です。</span><span class="sxs-lookup"><span data-stu-id="22277-114">Possible values are: `allAllowed`, `allBlocked`, `general`, `parentalGuidance`, `parentalGuidance13`, `restricted`, `adults`.</span></span>|
|<span data-ttu-id="22277-115">tvRating</span><span class="sxs-lookup"><span data-stu-id="22277-115">tvRating</span></span>|[<span data-ttu-id="22277-116">ratingUnitedStatesTelevisionType</span><span class="sxs-lookup"><span data-stu-id="22277-116">ratingUnitedStatesTelevisionType</span></span>](../resources/intune-deviceconfig-ratingunitedstatestelevisiontype.md)|<span data-ttu-id="22277-117">米国向けに選択されているテレビのレーティング。</span><span class="sxs-lookup"><span data-stu-id="22277-117">TV rating selected for United States.</span></span> <span data-ttu-id="22277-118">可能な値は、`allAllowed`、`allBlocked`、`childrenAll`、`childrenAbove7`、`general`、`parentalGuidance`、`childrenAbove14`、`adults` です。</span><span class="sxs-lookup"><span data-stu-id="22277-118">Possible values are: `allAllowed`, `allBlocked`, `childrenAll`, `childrenAbove7`, `general`, `parentalGuidance`, `childrenAbove14`, `adults`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="22277-119">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="22277-119">Relationships</span></span>
<span data-ttu-id="22277-120">なし</span><span class="sxs-lookup"><span data-stu-id="22277-120">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="22277-121">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="22277-121">JSON Representation</span></span>
<span data-ttu-id="22277-122">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="22277-122">Here is a JSON representation of the resource.</span></span>
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



