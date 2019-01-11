---
title: mediaContentRatingFrance リソースの種類
description: まだ文書化されていません
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 502abcae283b7e97e04ab2c342e6b526b41f64f4
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/11/2019
ms.locfileid: "27829884"
---
# <a name="mediacontentratingfrance-resource-type"></a><span data-ttu-id="53b24-103">mediaContentRatingFrance リソースの種類</span><span class="sxs-lookup"><span data-stu-id="53b24-103">mediaContentRatingFrance resource type</span></span>

> <span data-ttu-id="53b24-104">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="53b24-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="53b24-105">まだ文書化されていません</span><span class="sxs-lookup"><span data-stu-id="53b24-105">Not yet documented</span></span>
## <a name="properties"></a><span data-ttu-id="53b24-106">プロパティ</span><span class="sxs-lookup"><span data-stu-id="53b24-106">Properties</span></span>
|<span data-ttu-id="53b24-107">プロパティ</span><span class="sxs-lookup"><span data-stu-id="53b24-107">Property</span></span>|<span data-ttu-id="53b24-108">種類</span><span class="sxs-lookup"><span data-stu-id="53b24-108">Type</span></span>|<span data-ttu-id="53b24-109">説明</span><span class="sxs-lookup"><span data-stu-id="53b24-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="53b24-110">movieRating</span><span class="sxs-lookup"><span data-stu-id="53b24-110">movieRating</span></span>|[<span data-ttu-id="53b24-111">ratingFranceMoviesType</span><span class="sxs-lookup"><span data-stu-id="53b24-111">ratingFranceMoviesType</span></span>](../resources/intune-deviceconfig-ratingfrancemoviestype.md)|<span data-ttu-id="53b24-112">映画はフランスの選択を評価します。</span><span class="sxs-lookup"><span data-stu-id="53b24-112">Movies rating selected for France.</span></span> <span data-ttu-id="53b24-113">使用可能な値: `allAllowed`、`allBlocked`、`agesAbove10`、`agesAbove12`、`agesAbove16`、`agesAbove18`。</span><span class="sxs-lookup"><span data-stu-id="53b24-113">Possible values are: `allAllowed`, `allBlocked`, `agesAbove10`, `agesAbove12`, `agesAbove16`, `agesAbove18`.</span></span>|
|<span data-ttu-id="53b24-114">tvRating</span><span class="sxs-lookup"><span data-stu-id="53b24-114">tvRating</span></span>|[<span data-ttu-id="53b24-115">ratingFranceTelevisionType</span><span class="sxs-lookup"><span data-stu-id="53b24-115">ratingFranceTelevisionType</span></span>](../resources/intune-deviceconfig-ratingfrancetelevisiontype.md)|<span data-ttu-id="53b24-116">テレビの視聴制限がフランス用に選択します。</span><span class="sxs-lookup"><span data-stu-id="53b24-116">TV rating selected for France.</span></span> <span data-ttu-id="53b24-117">使用可能な値: `allAllowed`、`allBlocked`、`agesAbove10`、`agesAbove12`、`agesAbove16`、`agesAbove18`。</span><span class="sxs-lookup"><span data-stu-id="53b24-117">Possible values are: `allAllowed`, `allBlocked`, `agesAbove10`, `agesAbove12`, `agesAbove16`, `agesAbove18`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="53b24-118">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="53b24-118">Relationships</span></span>
<span data-ttu-id="53b24-119">なし</span><span class="sxs-lookup"><span data-stu-id="53b24-119">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="53b24-120">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="53b24-120">JSON Representation</span></span>
<span data-ttu-id="53b24-121">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="53b24-121">Here is a JSON representation of the resource.</span></span>
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



