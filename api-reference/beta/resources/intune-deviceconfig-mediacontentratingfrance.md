---
title: mediaContentRatingFrance リソースの種類
description: まだ文書化されていません
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: e149077493280145b2681cc2ad0111ec45534a0c
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/11/2019
ms.locfileid: "27862315"
---
# <a name="mediacontentratingfrance-resource-type"></a><span data-ttu-id="01c0c-103">mediaContentRatingFrance リソースの種類</span><span class="sxs-lookup"><span data-stu-id="01c0c-103">mediaContentRatingFrance resource type</span></span>

> <span data-ttu-id="01c0c-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="01c0c-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="01c0c-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="01c0c-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="01c0c-106">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="01c0c-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="01c0c-107">まだ文書化されていません</span><span class="sxs-lookup"><span data-stu-id="01c0c-107">Not yet documented</span></span>
## <a name="properties"></a><span data-ttu-id="01c0c-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="01c0c-108">Properties</span></span>
|<span data-ttu-id="01c0c-109">プロパティ</span><span class="sxs-lookup"><span data-stu-id="01c0c-109">Property</span></span>|<span data-ttu-id="01c0c-110">種類</span><span class="sxs-lookup"><span data-stu-id="01c0c-110">Type</span></span>|<span data-ttu-id="01c0c-111">説明</span><span class="sxs-lookup"><span data-stu-id="01c0c-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="01c0c-112">movieRating</span><span class="sxs-lookup"><span data-stu-id="01c0c-112">movieRating</span></span>|[<span data-ttu-id="01c0c-113">ratingFranceMoviesType</span><span class="sxs-lookup"><span data-stu-id="01c0c-113">ratingFranceMoviesType</span></span>](../resources/intune-deviceconfig-ratingfrancemoviestype.md)|<span data-ttu-id="01c0c-114">映画はフランスの選択を評価します。</span><span class="sxs-lookup"><span data-stu-id="01c0c-114">Movies rating selected for France.</span></span> <span data-ttu-id="01c0c-115">使用可能な値: `allAllowed`、`allBlocked`、`agesAbove10`、`agesAbove12`、`agesAbove16`、`agesAbove18`。</span><span class="sxs-lookup"><span data-stu-id="01c0c-115">Possible values are: `allAllowed`, `allBlocked`, `agesAbove10`, `agesAbove12`, `agesAbove16`, `agesAbove18`.</span></span>|
|<span data-ttu-id="01c0c-116">tvRating</span><span class="sxs-lookup"><span data-stu-id="01c0c-116">tvRating</span></span>|[<span data-ttu-id="01c0c-117">ratingFranceTelevisionType</span><span class="sxs-lookup"><span data-stu-id="01c0c-117">ratingFranceTelevisionType</span></span>](../resources/intune-deviceconfig-ratingfrancetelevisiontype.md)|<span data-ttu-id="01c0c-118">テレビの視聴制限がフランス用に選択します。</span><span class="sxs-lookup"><span data-stu-id="01c0c-118">TV rating selected for France.</span></span> <span data-ttu-id="01c0c-119">使用可能な値: `allAllowed`、`allBlocked`、`agesAbove10`、`agesAbove12`、`agesAbove16`、`agesAbove18`。</span><span class="sxs-lookup"><span data-stu-id="01c0c-119">Possible values are: `allAllowed`, `allBlocked`, `agesAbove10`, `agesAbove12`, `agesAbove16`, `agesAbove18`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="01c0c-120">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="01c0c-120">Relationships</span></span>
<span data-ttu-id="01c0c-121">なし</span><span class="sxs-lookup"><span data-stu-id="01c0c-121">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="01c0c-122">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="01c0c-122">JSON Representation</span></span>
<span data-ttu-id="01c0c-123">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="01c0c-123">Here is a JSON representation of the resource.</span></span>
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





