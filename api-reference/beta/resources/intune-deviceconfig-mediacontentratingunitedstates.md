---
title: mediaContentRatingUnitedStates リソースの種類
description: まだ文書化されていません
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 60208f2bace4826f06ff5a81f02bc087211d52a1
ms.sourcegitcommit: 20fef447f7e658a454a3887ea49746142c22e45c
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/11/2019
ms.locfileid: "31777901"
---
# <a name="mediacontentratingunitedstates-resource-type"></a><span data-ttu-id="6eec6-103">mediaContentRatingUnitedStates リソースの種類</span><span class="sxs-lookup"><span data-stu-id="6eec6-103">mediaContentRatingUnitedStates resource type</span></span>

> <span data-ttu-id="6eec6-104">**重要:** ベータ版の Microsoft Graph api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="6eec6-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="6eec6-105">**注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="6eec6-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="6eec6-106">まだ文書化されていません</span><span class="sxs-lookup"><span data-stu-id="6eec6-106">Not yet documented</span></span>

## <a name="properties"></a><span data-ttu-id="6eec6-107">プロパティ</span><span class="sxs-lookup"><span data-stu-id="6eec6-107">Properties</span></span>
|<span data-ttu-id="6eec6-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="6eec6-108">Property</span></span>|<span data-ttu-id="6eec6-109">型</span><span class="sxs-lookup"><span data-stu-id="6eec6-109">Type</span></span>|<span data-ttu-id="6eec6-110">説明</span><span class="sxs-lookup"><span data-stu-id="6eec6-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="6eec6-111">movieRating</span><span class="sxs-lookup"><span data-stu-id="6eec6-111">movieRating</span></span>|[<span data-ttu-id="6eec6-112">ratingUnitedStatesMoviesType</span><span class="sxs-lookup"><span data-stu-id="6eec6-112">ratingUnitedStatesMoviesType</span></span>](../resources/intune-deviceconfig-ratingunitedstatesmoviestype.md)|<span data-ttu-id="6eec6-113">米国向けに選択されている映画のレーティング。</span><span class="sxs-lookup"><span data-stu-id="6eec6-113">Movies rating selected for United States.</span></span> <span data-ttu-id="6eec6-114">可能な値は、`allAllowed`、`allBlocked`、`general`、`parentalGuidance`、`parentalGuidance13`、`restricted`、`adults` です。</span><span class="sxs-lookup"><span data-stu-id="6eec6-114">Possible values are: `allAllowed`, `allBlocked`, `general`, `parentalGuidance`, `parentalGuidance13`, `restricted`, `adults`.</span></span>|
|<span data-ttu-id="6eec6-115">tvRating</span><span class="sxs-lookup"><span data-stu-id="6eec6-115">tvRating</span></span>|[<span data-ttu-id="6eec6-116">ratingUnitedStatesTelevisionType</span><span class="sxs-lookup"><span data-stu-id="6eec6-116">ratingUnitedStatesTelevisionType</span></span>](../resources/intune-deviceconfig-ratingunitedstatestelevisiontype.md)|<span data-ttu-id="6eec6-117">米国向けに選択されているテレビのレーティング。</span><span class="sxs-lookup"><span data-stu-id="6eec6-117">TV rating selected for United States.</span></span> <span data-ttu-id="6eec6-118">可能な値は、`allAllowed`、`allBlocked`、`childrenAll`、`childrenAbove7`、`general`、`parentalGuidance`、`childrenAbove14`、`adults` です。</span><span class="sxs-lookup"><span data-stu-id="6eec6-118">Possible values are: `allAllowed`, `allBlocked`, `childrenAll`, `childrenAbove7`, `general`, `parentalGuidance`, `childrenAbove14`, `adults`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="6eec6-119">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="6eec6-119">Relationships</span></span>
<span data-ttu-id="6eec6-120">なし</span><span class="sxs-lookup"><span data-stu-id="6eec6-120">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="6eec6-121">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="6eec6-121">JSON Representation</span></span>
<span data-ttu-id="6eec6-122">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="6eec6-122">Here is a JSON representation of the resource.</span></span>
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





