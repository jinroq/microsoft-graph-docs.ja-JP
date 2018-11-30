---
title: mediaContentRatingFrance リソースの種類
description: まだ文書化されていません
ms.openlocfilehash: dabadb4d03181d3cd66db582005c4ec58f28aa9d
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27068399"
---
# <a name="mediacontentratingfrance-resource-type"></a><span data-ttu-id="f34eb-103">mediaContentRatingFrance リソースの種類</span><span class="sxs-lookup"><span data-stu-id="f34eb-103">mediaContentRatingFrance resource type</span></span>

> <span data-ttu-id="f34eb-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="f34eb-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="f34eb-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="f34eb-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="f34eb-106">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="f34eb-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="f34eb-107">まだ文書化されていません</span><span class="sxs-lookup"><span data-stu-id="f34eb-107">Not yet documented</span></span>
## <a name="properties"></a><span data-ttu-id="f34eb-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="f34eb-108">Properties</span></span>
|<span data-ttu-id="f34eb-109">プロパティ</span><span class="sxs-lookup"><span data-stu-id="f34eb-109">Property</span></span>|<span data-ttu-id="f34eb-110">型</span><span class="sxs-lookup"><span data-stu-id="f34eb-110">Type</span></span>|<span data-ttu-id="f34eb-111">説明</span><span class="sxs-lookup"><span data-stu-id="f34eb-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f34eb-112">movieRating</span><span class="sxs-lookup"><span data-stu-id="f34eb-112">movieRating</span></span>|[<span data-ttu-id="f34eb-113">ratingFranceMoviesType</span><span class="sxs-lookup"><span data-stu-id="f34eb-113">ratingFranceMoviesType</span></span>](../resources/intune-deviceconfig-ratingfrancemoviestype.md)|<span data-ttu-id="f34eb-114">映画はフランスの選択を評価します。</span><span class="sxs-lookup"><span data-stu-id="f34eb-114">Movies rating selected for France.</span></span> <span data-ttu-id="f34eb-115">使用可能な値: `allAllowed`、`allBlocked`、`agesAbove10`、`agesAbove12`、`agesAbove16`、`agesAbove18`。</span><span class="sxs-lookup"><span data-stu-id="f34eb-115">Possible values are: `allAllowed`, `allBlocked`, `agesAbove10`, `agesAbove12`, `agesAbove16`, `agesAbove18`.</span></span>|
|<span data-ttu-id="f34eb-116">tvRating</span><span class="sxs-lookup"><span data-stu-id="f34eb-116">tvRating</span></span>|[<span data-ttu-id="f34eb-117">ratingFranceTelevisionType</span><span class="sxs-lookup"><span data-stu-id="f34eb-117">ratingFranceTelevisionType</span></span>](../resources/intune-deviceconfig-ratingfrancetelevisiontype.md)|<span data-ttu-id="f34eb-118">テレビの視聴制限がフランス用に選択します。</span><span class="sxs-lookup"><span data-stu-id="f34eb-118">TV rating selected for France.</span></span> <span data-ttu-id="f34eb-119">使用可能な値: `allAllowed`、`allBlocked`、`agesAbove10`、`agesAbove12`、`agesAbove16`、`agesAbove18`。</span><span class="sxs-lookup"><span data-stu-id="f34eb-119">Possible values are: `allAllowed`, `allBlocked`, `agesAbove10`, `agesAbove12`, `agesAbove16`, `agesAbove18`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="f34eb-120">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="f34eb-120">Relationships</span></span>
<span data-ttu-id="f34eb-121">なし</span><span class="sxs-lookup"><span data-stu-id="f34eb-121">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="f34eb-122">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="f34eb-122">JSON Representation</span></span>
<span data-ttu-id="f34eb-123">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="f34eb-123">Here is a JSON representation of the resource.</span></span>
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





