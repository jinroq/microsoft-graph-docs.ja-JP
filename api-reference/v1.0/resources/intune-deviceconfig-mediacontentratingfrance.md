---
title: mediaContentRatingFrance リソースの種類
description: まだ文書化されていません
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 4f6fe2e4f4ca0f629ac0d4dbc387aab68122896c
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/12/2019
ms.locfileid: "27913115"
---
# <a name="mediacontentratingfrance-resource-type"></a><span data-ttu-id="fbb5a-103">mediaContentRatingFrance リソースの種類</span><span class="sxs-lookup"><span data-stu-id="fbb5a-103">mediaContentRatingFrance resource type</span></span>

> <span data-ttu-id="fbb5a-104">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="fbb5a-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="fbb5a-105">まだ文書化されていません</span><span class="sxs-lookup"><span data-stu-id="fbb5a-105">Not yet documented</span></span>
## <a name="properties"></a><span data-ttu-id="fbb5a-106">プロパティ</span><span class="sxs-lookup"><span data-stu-id="fbb5a-106">Properties</span></span>
|<span data-ttu-id="fbb5a-107">プロパティ</span><span class="sxs-lookup"><span data-stu-id="fbb5a-107">Property</span></span>|<span data-ttu-id="fbb5a-108">種類</span><span class="sxs-lookup"><span data-stu-id="fbb5a-108">Type</span></span>|<span data-ttu-id="fbb5a-109">説明</span><span class="sxs-lookup"><span data-stu-id="fbb5a-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="fbb5a-110">movieRating</span><span class="sxs-lookup"><span data-stu-id="fbb5a-110">movieRating</span></span>|[<span data-ttu-id="fbb5a-111">ratingFranceMoviesType</span><span class="sxs-lookup"><span data-stu-id="fbb5a-111">ratingFranceMoviesType</span></span>](../resources/intune-deviceconfig-ratingfrancemoviestype.md)|<span data-ttu-id="fbb5a-112">映画はフランスの選択を評価します。</span><span class="sxs-lookup"><span data-stu-id="fbb5a-112">Movies rating selected for France.</span></span> <span data-ttu-id="fbb5a-113">使用可能な値: `allAllowed`、`allBlocked`、`agesAbove10`、`agesAbove12`、`agesAbove16`、`agesAbove18`。</span><span class="sxs-lookup"><span data-stu-id="fbb5a-113">Possible values are: `allAllowed`, `allBlocked`, `agesAbove10`, `agesAbove12`, `agesAbove16`, `agesAbove18`.</span></span>|
|<span data-ttu-id="fbb5a-114">tvRating</span><span class="sxs-lookup"><span data-stu-id="fbb5a-114">tvRating</span></span>|[<span data-ttu-id="fbb5a-115">ratingFranceTelevisionType</span><span class="sxs-lookup"><span data-stu-id="fbb5a-115">ratingFranceTelevisionType</span></span>](../resources/intune-deviceconfig-ratingfrancetelevisiontype.md)|<span data-ttu-id="fbb5a-116">テレビの視聴制限がフランス用に選択します。</span><span class="sxs-lookup"><span data-stu-id="fbb5a-116">TV rating selected for France.</span></span> <span data-ttu-id="fbb5a-117">使用可能な値: `allAllowed`、`allBlocked`、`agesAbove10`、`agesAbove12`、`agesAbove16`、`agesAbove18`。</span><span class="sxs-lookup"><span data-stu-id="fbb5a-117">Possible values are: `allAllowed`, `allBlocked`, `agesAbove10`, `agesAbove12`, `agesAbove16`, `agesAbove18`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="fbb5a-118">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="fbb5a-118">Relationships</span></span>
<span data-ttu-id="fbb5a-119">なし</span><span class="sxs-lookup"><span data-stu-id="fbb5a-119">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="fbb5a-120">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="fbb5a-120">JSON Representation</span></span>
<span data-ttu-id="fbb5a-121">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="fbb5a-121">Here is a JSON representation of the resource.</span></span>
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



