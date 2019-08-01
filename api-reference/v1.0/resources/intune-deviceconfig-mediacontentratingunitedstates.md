---
title: mediaContentRatingUnitedStates リソースの種類
description: まだ文書化されていません
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: c6c6df674fc4cef174892d4cdb27303c3933fcdd
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "36031375"
---
# <a name="mediacontentratingunitedstates-resource-type"></a><span data-ttu-id="29645-103">mediaContentRatingUnitedStates リソースの種類</span><span class="sxs-lookup"><span data-stu-id="29645-103">mediaContentRatingUnitedStates resource type</span></span>

> <span data-ttu-id="29645-104">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="29645-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="29645-105">まだ文書化されていません</span><span class="sxs-lookup"><span data-stu-id="29645-105">Not yet documented</span></span>

## <a name="properties"></a><span data-ttu-id="29645-106">プロパティ</span><span class="sxs-lookup"><span data-stu-id="29645-106">Properties</span></span>
|<span data-ttu-id="29645-107">プロパティ</span><span class="sxs-lookup"><span data-stu-id="29645-107">Property</span></span>|<span data-ttu-id="29645-108">型</span><span class="sxs-lookup"><span data-stu-id="29645-108">Type</span></span>|<span data-ttu-id="29645-109">説明</span><span class="sxs-lookup"><span data-stu-id="29645-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="29645-110">movieRating</span><span class="sxs-lookup"><span data-stu-id="29645-110">movieRating</span></span>|[<span data-ttu-id="29645-111">ratingUnitedStatesMoviesType</span><span class="sxs-lookup"><span data-stu-id="29645-111">ratingUnitedStatesMoviesType</span></span>](../resources/intune-deviceconfig-ratingunitedstatesmoviestype.md)|<span data-ttu-id="29645-112">米国向けに選択されている映画のレーティング。</span><span class="sxs-lookup"><span data-stu-id="29645-112">Movies rating selected for United States.</span></span> <span data-ttu-id="29645-113">可能な値は、`allAllowed`、`allBlocked`、`general`、`parentalGuidance`、`parentalGuidance13`、`restricted`、`adults` です。</span><span class="sxs-lookup"><span data-stu-id="29645-113">Possible values are: `allAllowed`, `allBlocked`, `general`, `parentalGuidance`, `parentalGuidance13`, `restricted`, `adults`.</span></span>|
|<span data-ttu-id="29645-114">tvRating</span><span class="sxs-lookup"><span data-stu-id="29645-114">tvRating</span></span>|[<span data-ttu-id="29645-115">ratingUnitedStatesTelevisionType</span><span class="sxs-lookup"><span data-stu-id="29645-115">ratingUnitedStatesTelevisionType</span></span>](../resources/intune-deviceconfig-ratingunitedstatestelevisiontype.md)|<span data-ttu-id="29645-116">米国向けに選択されているテレビのレーティング。</span><span class="sxs-lookup"><span data-stu-id="29645-116">TV rating selected for United States.</span></span> <span data-ttu-id="29645-117">可能な値は、`allAllowed`、`allBlocked`、`childrenAll`、`childrenAbove7`、`general`、`parentalGuidance`、`childrenAbove14`、`adults` です。</span><span class="sxs-lookup"><span data-stu-id="29645-117">Possible values are: `allAllowed`, `allBlocked`, `childrenAll`, `childrenAbove7`, `general`, `parentalGuidance`, `childrenAbove14`, `adults`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="29645-118">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="29645-118">Relationships</span></span>
<span data-ttu-id="29645-119">なし</span><span class="sxs-lookup"><span data-stu-id="29645-119">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="29645-120">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="29645-120">JSON Representation</span></span>
<span data-ttu-id="29645-121">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="29645-121">Here is a JSON representation of the resource.</span></span>
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



