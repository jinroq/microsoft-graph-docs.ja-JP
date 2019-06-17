---
title: mediaContentRatingUnitedStates リソースの種類
description: まだ文書化されていません
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: aa8f9c2a1daecb447c1e0bc6b0541e42750d6328
ms.sourcegitcommit: 0a62bc5849f27a55d83efce9b3eb01b9711bbe1d
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/14/2019
ms.locfileid: "34986719"
---
# <a name="mediacontentratingunitedstates-resource-type"></a><span data-ttu-id="0efcb-103">mediaContentRatingUnitedStates リソースの種類</span><span class="sxs-lookup"><span data-stu-id="0efcb-103">mediaContentRatingUnitedStates resource type</span></span>

> <span data-ttu-id="0efcb-104">**重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="0efcb-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="0efcb-105">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="0efcb-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="0efcb-106">まだ文書化されていません</span><span class="sxs-lookup"><span data-stu-id="0efcb-106">Not yet documented</span></span>

## <a name="properties"></a><span data-ttu-id="0efcb-107">プロパティ</span><span class="sxs-lookup"><span data-stu-id="0efcb-107">Properties</span></span>
|<span data-ttu-id="0efcb-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="0efcb-108">Property</span></span>|<span data-ttu-id="0efcb-109">型</span><span class="sxs-lookup"><span data-stu-id="0efcb-109">Type</span></span>|<span data-ttu-id="0efcb-110">説明</span><span class="sxs-lookup"><span data-stu-id="0efcb-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="0efcb-111">movieRating</span><span class="sxs-lookup"><span data-stu-id="0efcb-111">movieRating</span></span>|[<span data-ttu-id="0efcb-112">ratingUnitedStatesMoviesType</span><span class="sxs-lookup"><span data-stu-id="0efcb-112">ratingUnitedStatesMoviesType</span></span>](../resources/intune-deviceconfig-ratingunitedstatesmoviestype.md)|<span data-ttu-id="0efcb-113">米国向けに選択されている映画のレーティング。</span><span class="sxs-lookup"><span data-stu-id="0efcb-113">Movies rating selected for United States.</span></span> <span data-ttu-id="0efcb-114">可能な値は、`allAllowed`、`allBlocked`、`general`、`parentalGuidance`、`parentalGuidance13`、`restricted`、`adults` です。</span><span class="sxs-lookup"><span data-stu-id="0efcb-114">Possible values are: `allAllowed`, `allBlocked`, `general`, `parentalGuidance`, `parentalGuidance13`, `restricted`, `adults`.</span></span>|
|<span data-ttu-id="0efcb-115">tvRating</span><span class="sxs-lookup"><span data-stu-id="0efcb-115">tvRating</span></span>|[<span data-ttu-id="0efcb-116">ratingUnitedStatesTelevisionType</span><span class="sxs-lookup"><span data-stu-id="0efcb-116">ratingUnitedStatesTelevisionType</span></span>](../resources/intune-deviceconfig-ratingunitedstatestelevisiontype.md)|<span data-ttu-id="0efcb-117">米国向けに選択されているテレビのレーティング。</span><span class="sxs-lookup"><span data-stu-id="0efcb-117">TV rating selected for United States.</span></span> <span data-ttu-id="0efcb-118">可能な値は、`allAllowed`、`allBlocked`、`childrenAll`、`childrenAbove7`、`general`、`parentalGuidance`、`childrenAbove14`、`adults` です。</span><span class="sxs-lookup"><span data-stu-id="0efcb-118">Possible values are: `allAllowed`, `allBlocked`, `childrenAll`, `childrenAbove7`, `general`, `parentalGuidance`, `childrenAbove14`, `adults`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="0efcb-119">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="0efcb-119">Relationships</span></span>
<span data-ttu-id="0efcb-120">なし</span><span class="sxs-lookup"><span data-stu-id="0efcb-120">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="0efcb-121">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="0efcb-121">JSON Representation</span></span>
<span data-ttu-id="0efcb-122">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="0efcb-122">Here is a JSON representation of the resource.</span></span>
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





