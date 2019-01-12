---
title: mediaContentRatingFrance リソースの種類
description: まだ文書化されていません
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 7aa3c16df6b32f5c5c50f53959aaccc767b39bbd
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/12/2019
ms.locfileid: "27928144"
---
# <a name="mediacontentratingfrance-resource-type"></a><span data-ttu-id="d35c4-103">mediaContentRatingFrance リソースの種類</span><span class="sxs-lookup"><span data-stu-id="d35c4-103">mediaContentRatingFrance resource type</span></span>

> <span data-ttu-id="d35c4-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="d35c4-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="d35c4-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="d35c4-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="d35c4-106">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="d35c4-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="d35c4-107">まだ文書化されていません</span><span class="sxs-lookup"><span data-stu-id="d35c4-107">Not yet documented</span></span>
## <a name="properties"></a><span data-ttu-id="d35c4-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="d35c4-108">Properties</span></span>
|<span data-ttu-id="d35c4-109">プロパティ</span><span class="sxs-lookup"><span data-stu-id="d35c4-109">Property</span></span>|<span data-ttu-id="d35c4-110">型</span><span class="sxs-lookup"><span data-stu-id="d35c4-110">Type</span></span>|<span data-ttu-id="d35c4-111">説明</span><span class="sxs-lookup"><span data-stu-id="d35c4-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d35c4-112">movieRating</span><span class="sxs-lookup"><span data-stu-id="d35c4-112">movieRating</span></span>|[<span data-ttu-id="d35c4-113">ratingFranceMoviesType</span><span class="sxs-lookup"><span data-stu-id="d35c4-113">ratingFranceMoviesType</span></span>](../resources/intune-deviceconfig-ratingfrancemoviestype.md)|<span data-ttu-id="d35c4-114">映画はフランスの選択を評価します。</span><span class="sxs-lookup"><span data-stu-id="d35c4-114">Movies rating selected for France.</span></span> <span data-ttu-id="d35c4-115">使用可能な値: `allAllowed`、`allBlocked`、`agesAbove10`、`agesAbove12`、`agesAbove16`、`agesAbove18`。</span><span class="sxs-lookup"><span data-stu-id="d35c4-115">Possible values are: `allAllowed`, `allBlocked`, `agesAbove10`, `agesAbove12`, `agesAbove16`, `agesAbove18`.</span></span>|
|<span data-ttu-id="d35c4-116">tvRating</span><span class="sxs-lookup"><span data-stu-id="d35c4-116">tvRating</span></span>|[<span data-ttu-id="d35c4-117">ratingFranceTelevisionType</span><span class="sxs-lookup"><span data-stu-id="d35c4-117">ratingFranceTelevisionType</span></span>](../resources/intune-deviceconfig-ratingfrancetelevisiontype.md)|<span data-ttu-id="d35c4-118">テレビの視聴制限がフランス用に選択します。</span><span class="sxs-lookup"><span data-stu-id="d35c4-118">TV rating selected for France.</span></span> <span data-ttu-id="d35c4-119">使用可能な値: `allAllowed`、`allBlocked`、`agesAbove10`、`agesAbove12`、`agesAbove16`、`agesAbove18`。</span><span class="sxs-lookup"><span data-stu-id="d35c4-119">Possible values are: `allAllowed`, `allBlocked`, `agesAbove10`, `agesAbove12`, `agesAbove16`, `agesAbove18`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="d35c4-120">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="d35c4-120">Relationships</span></span>
<span data-ttu-id="d35c4-121">なし</span><span class="sxs-lookup"><span data-stu-id="d35c4-121">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="d35c4-122">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="d35c4-122">JSON Representation</span></span>
<span data-ttu-id="d35c4-123">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="d35c4-123">Here is a JSON representation of the resource.</span></span>
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





