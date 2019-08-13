---
title: mediaContentRatingFrance リソースの種類
description: まだ文書化されていません
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 892daf67977086b647d74567660d3b4c3d4eec53
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/13/2019
ms.locfileid: "36368752"
---
# <a name="mediacontentratingfrance-resource-type"></a><span data-ttu-id="15cb2-103">mediaContentRatingFrance リソースの種類</span><span class="sxs-lookup"><span data-stu-id="15cb2-103">mediaContentRatingFrance resource type</span></span>

> <span data-ttu-id="15cb2-104">**重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="15cb2-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="15cb2-105">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="15cb2-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="15cb2-106">まだ文書化されていません</span><span class="sxs-lookup"><span data-stu-id="15cb2-106">Not yet documented</span></span>

## <a name="properties"></a><span data-ttu-id="15cb2-107">プロパティ</span><span class="sxs-lookup"><span data-stu-id="15cb2-107">Properties</span></span>
|<span data-ttu-id="15cb2-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="15cb2-108">Property</span></span>|<span data-ttu-id="15cb2-109">型</span><span class="sxs-lookup"><span data-stu-id="15cb2-109">Type</span></span>|<span data-ttu-id="15cb2-110">説明</span><span class="sxs-lookup"><span data-stu-id="15cb2-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="15cb2-111">movieRating</span><span class="sxs-lookup"><span data-stu-id="15cb2-111">movieRating</span></span>|[<span data-ttu-id="15cb2-112">ratingFranceMoviesType</span><span class="sxs-lookup"><span data-stu-id="15cb2-112">ratingFranceMoviesType</span></span>](../resources/intune-deviceconfig-ratingfrancemoviestype.md)|<span data-ttu-id="15cb2-113">フランスに対して選択されている映画のレーティング。</span><span class="sxs-lookup"><span data-stu-id="15cb2-113">Movies rating selected for France.</span></span> <span data-ttu-id="15cb2-114">使用可能な値: `allAllowed`、`allBlocked`、`agesAbove10`、`agesAbove12`、`agesAbove16`、`agesAbove18`。</span><span class="sxs-lookup"><span data-stu-id="15cb2-114">Possible values are: `allAllowed`, `allBlocked`, `agesAbove10`, `agesAbove12`, `agesAbove16`, `agesAbove18`.</span></span>|
|<span data-ttu-id="15cb2-115">tvRating</span><span class="sxs-lookup"><span data-stu-id="15cb2-115">tvRating</span></span>|[<span data-ttu-id="15cb2-116">ratingFranceTelevisionType</span><span class="sxs-lookup"><span data-stu-id="15cb2-116">ratingFranceTelevisionType</span></span>](../resources/intune-deviceconfig-ratingfrancetelevisiontype.md)|<span data-ttu-id="15cb2-117">フランスに対して選択されているテレビのレーティング。</span><span class="sxs-lookup"><span data-stu-id="15cb2-117">TV rating selected for France.</span></span> <span data-ttu-id="15cb2-118">使用可能な値: `allAllowed`、`allBlocked`、`agesAbove10`、`agesAbove12`、`agesAbove16`、`agesAbove18`。</span><span class="sxs-lookup"><span data-stu-id="15cb2-118">Possible values are: `allAllowed`, `allBlocked`, `agesAbove10`, `agesAbove12`, `agesAbove16`, `agesAbove18`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="15cb2-119">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="15cb2-119">Relationships</span></span>
<span data-ttu-id="15cb2-120">なし</span><span class="sxs-lookup"><span data-stu-id="15cb2-120">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="15cb2-121">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="15cb2-121">JSON Representation</span></span>
<span data-ttu-id="15cb2-122">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="15cb2-122">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.mediaContentRatingFrance"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.mediaContentRatingFrance",
  "movieRating": "String",
  "tvRating": "String"
}
```



