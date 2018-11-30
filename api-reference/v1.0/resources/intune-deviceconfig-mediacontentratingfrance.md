---
title: mediaContentRatingFrance リソースの種類
description: まだ文書化されていません
ms.openlocfilehash: bd2f4933ea05c7db193d700799cdcbdc79490356
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27020830"
---
# <a name="mediacontentratingfrance-resource-type"></a><span data-ttu-id="2b097-103">mediaContentRatingFrance リソースの種類</span><span class="sxs-lookup"><span data-stu-id="2b097-103">mediaContentRatingFrance resource type</span></span>

> <span data-ttu-id="2b097-104">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="2b097-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="2b097-105">まだ文書化されていません</span><span class="sxs-lookup"><span data-stu-id="2b097-105">Not yet documented</span></span>
## <a name="properties"></a><span data-ttu-id="2b097-106">プロパティ</span><span class="sxs-lookup"><span data-stu-id="2b097-106">Properties</span></span>
|<span data-ttu-id="2b097-107">プロパティ</span><span class="sxs-lookup"><span data-stu-id="2b097-107">Property</span></span>|<span data-ttu-id="2b097-108">型</span><span class="sxs-lookup"><span data-stu-id="2b097-108">Type</span></span>|<span data-ttu-id="2b097-109">説明</span><span class="sxs-lookup"><span data-stu-id="2b097-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="2b097-110">movieRating</span><span class="sxs-lookup"><span data-stu-id="2b097-110">movieRating</span></span>|[<span data-ttu-id="2b097-111">ratingFranceMoviesType</span><span class="sxs-lookup"><span data-stu-id="2b097-111">ratingFranceMoviesType</span></span>](../resources/intune-deviceconfig-ratingfrancemoviestype.md)|<span data-ttu-id="2b097-112">映画はフランスの選択を評価します。</span><span class="sxs-lookup"><span data-stu-id="2b097-112">Movies rating selected for France.</span></span> <span data-ttu-id="2b097-113">使用可能な値: `allAllowed`、`allBlocked`、`agesAbove10`、`agesAbove12`、`agesAbove16`、`agesAbove18`。</span><span class="sxs-lookup"><span data-stu-id="2b097-113">Possible values are: `allAllowed`, `allBlocked`, `agesAbove10`, `agesAbove12`, `agesAbove16`, `agesAbove18`.</span></span>|
|<span data-ttu-id="2b097-114">tvRating</span><span class="sxs-lookup"><span data-stu-id="2b097-114">tvRating</span></span>|[<span data-ttu-id="2b097-115">ratingFranceTelevisionType</span><span class="sxs-lookup"><span data-stu-id="2b097-115">ratingFranceTelevisionType</span></span>](../resources/intune-deviceconfig-ratingfrancetelevisiontype.md)|<span data-ttu-id="2b097-116">テレビの視聴制限がフランス用に選択します。</span><span class="sxs-lookup"><span data-stu-id="2b097-116">TV rating selected for France.</span></span> <span data-ttu-id="2b097-117">使用可能な値: `allAllowed`、`allBlocked`、`agesAbove10`、`agesAbove12`、`agesAbove16`、`agesAbove18`。</span><span class="sxs-lookup"><span data-stu-id="2b097-117">Possible values are: `allAllowed`, `allBlocked`, `agesAbove10`, `agesAbove12`, `agesAbove16`, `agesAbove18`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="2b097-118">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="2b097-118">Relationships</span></span>
<span data-ttu-id="2b097-119">なし</span><span class="sxs-lookup"><span data-stu-id="2b097-119">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="2b097-120">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="2b097-120">JSON Representation</span></span>
<span data-ttu-id="2b097-121">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="2b097-121">Here is a JSON representation of the resource.</span></span>
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



