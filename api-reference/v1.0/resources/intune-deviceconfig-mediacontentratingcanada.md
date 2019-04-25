---
title: mediaContentRatingCanada リソースの種類
description: まだ文書化されていません
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 88975975b07eb2805ee5f73cc416e3803d5fe24f
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32572354"
---
# <a name="mediacontentratingcanada-resource-type"></a><span data-ttu-id="8b2ea-103">mediaContentRatingCanada リソースの種類</span><span class="sxs-lookup"><span data-stu-id="8b2ea-103">mediaContentRatingCanada resource type</span></span>

> <span data-ttu-id="8b2ea-104">**注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="8b2ea-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="8b2ea-105">まだ文書化されていません</span><span class="sxs-lookup"><span data-stu-id="8b2ea-105">Not yet documented</span></span>

## <a name="properties"></a><span data-ttu-id="8b2ea-106">プロパティ</span><span class="sxs-lookup"><span data-stu-id="8b2ea-106">Properties</span></span>
|<span data-ttu-id="8b2ea-107">プロパティ</span><span class="sxs-lookup"><span data-stu-id="8b2ea-107">Property</span></span>|<span data-ttu-id="8b2ea-108">型</span><span class="sxs-lookup"><span data-stu-id="8b2ea-108">Type</span></span>|<span data-ttu-id="8b2ea-109">説明</span><span class="sxs-lookup"><span data-stu-id="8b2ea-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="8b2ea-110">movieRating</span><span class="sxs-lookup"><span data-stu-id="8b2ea-110">movieRating</span></span>|[<span data-ttu-id="8b2ea-111">ratingCanadaMoviesType</span><span class="sxs-lookup"><span data-stu-id="8b2ea-111">ratingCanadaMoviesType</span></span>](../resources/intune-deviceconfig-ratingcanadamoviestype.md)|<span data-ttu-id="8b2ea-112">カナダ向けに選択されている映画のレーティング。</span><span class="sxs-lookup"><span data-stu-id="8b2ea-112">Movies rating selected for Canada.</span></span> <span data-ttu-id="8b2ea-113">可能な値は、`allAllowed`、`allBlocked`、`general`、`parentalGuidance`、`agesAbove14`、`agesAbove18`、`restricted` です。</span><span class="sxs-lookup"><span data-stu-id="8b2ea-113">Possible values are: `allAllowed`, `allBlocked`, `general`, `parentalGuidance`, `agesAbove14`, `agesAbove18`, `restricted`.</span></span>|
|<span data-ttu-id="8b2ea-114">tvRating</span><span class="sxs-lookup"><span data-stu-id="8b2ea-114">tvRating</span></span>|[<span data-ttu-id="8b2ea-115">ratingCanadaTelevisionType</span><span class="sxs-lookup"><span data-stu-id="8b2ea-115">ratingCanadaTelevisionType</span></span>](../resources/intune-deviceconfig-ratingcanadatelevisiontype.md)|<span data-ttu-id="8b2ea-116">カナダ向けに選択されているテレビのレーティング。</span><span class="sxs-lookup"><span data-stu-id="8b2ea-116">TV rating selected for Canada.</span></span> <span data-ttu-id="8b2ea-117">可能な値は、`allAllowed`、`allBlocked`、`children`、`childrenAbove8`、`general`、`parentalGuidance`、`agesAbove14`、`agesAbove18` です。</span><span class="sxs-lookup"><span data-stu-id="8b2ea-117">Possible values are: `allAllowed`, `allBlocked`, `children`, `childrenAbove8`, `general`, `parentalGuidance`, `agesAbove14`, `agesAbove18`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="8b2ea-118">関係</span><span class="sxs-lookup"><span data-stu-id="8b2ea-118">Relationships</span></span>
<span data-ttu-id="8b2ea-119">なし</span><span class="sxs-lookup"><span data-stu-id="8b2ea-119">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="8b2ea-120">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="8b2ea-120">JSON Representation</span></span>
<span data-ttu-id="8b2ea-121">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="8b2ea-121">Here is a JSON representation of the resource.</span></span>
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



