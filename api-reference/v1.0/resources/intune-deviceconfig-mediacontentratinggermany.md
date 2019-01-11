---
title: mediaContentRatingGermany リソースの種類
description: まだ文書化されていません
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 5dd25a8bd29211fd593daf3ecea20a7808384bc1
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/11/2019
ms.locfileid: "27860005"
---
# <a name="mediacontentratinggermany-resource-type"></a><span data-ttu-id="64bae-103">mediaContentRatingGermany リソースの種類</span><span class="sxs-lookup"><span data-stu-id="64bae-103">mediaContentRatingGermany resource type</span></span>

> <span data-ttu-id="64bae-104">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="64bae-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="64bae-105">まだ文書化されていません</span><span class="sxs-lookup"><span data-stu-id="64bae-105">Not yet documented</span></span>
## <a name="properties"></a><span data-ttu-id="64bae-106">プロパティ</span><span class="sxs-lookup"><span data-stu-id="64bae-106">Properties</span></span>
|<span data-ttu-id="64bae-107">プロパティ</span><span class="sxs-lookup"><span data-stu-id="64bae-107">Property</span></span>|<span data-ttu-id="64bae-108">種類</span><span class="sxs-lookup"><span data-stu-id="64bae-108">Type</span></span>|<span data-ttu-id="64bae-109">説明</span><span class="sxs-lookup"><span data-stu-id="64bae-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="64bae-110">movieRating</span><span class="sxs-lookup"><span data-stu-id="64bae-110">movieRating</span></span>|[<span data-ttu-id="64bae-111">ratingGermanyMoviesType</span><span class="sxs-lookup"><span data-stu-id="64bae-111">ratingGermanyMoviesType</span></span>](../resources/intune-deviceconfig-ratinggermanymoviestype.md)|<span data-ttu-id="64bae-112">映画がドイツの選択を評価します。</span><span class="sxs-lookup"><span data-stu-id="64bae-112">Movies rating selected for Germany.</span></span> <span data-ttu-id="64bae-113">可能な値は、`allAllowed`、`allBlocked`、`general`、`agesAbove6`、`agesAbove12`、`agesAbove16`、`adults` です。</span><span class="sxs-lookup"><span data-stu-id="64bae-113">Possible values are: `allAllowed`, `allBlocked`, `general`, `agesAbove6`, `agesAbove12`, `agesAbove16`, `adults`.</span></span>|
|<span data-ttu-id="64bae-114">tvRating</span><span class="sxs-lookup"><span data-stu-id="64bae-114">tvRating</span></span>|[<span data-ttu-id="64bae-115">ratingGermanyTelevisionType</span><span class="sxs-lookup"><span data-stu-id="64bae-115">ratingGermanyTelevisionType</span></span>](../resources/intune-deviceconfig-ratinggermanytelevisiontype.md)|<span data-ttu-id="64bae-116">テレビの視聴制限がドイツを選択します。</span><span class="sxs-lookup"><span data-stu-id="64bae-116">TV rating selected for Germany.</span></span> <span data-ttu-id="64bae-117">可能な値は、`allAllowed`、`allBlocked`、`general`、`agesAbove6`、`agesAbove12`、`agesAbove16`、`adults` です。</span><span class="sxs-lookup"><span data-stu-id="64bae-117">Possible values are: `allAllowed`, `allBlocked`, `general`, `agesAbove6`, `agesAbove12`, `agesAbove16`, `adults`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="64bae-118">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="64bae-118">Relationships</span></span>
<span data-ttu-id="64bae-119">なし</span><span class="sxs-lookup"><span data-stu-id="64bae-119">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="64bae-120">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="64bae-120">JSON Representation</span></span>
<span data-ttu-id="64bae-121">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="64bae-121">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.mediaContentRatingGermany"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.mediaContentRatingGermany",
  "movieRating": "String",
  "tvRating": "String"
}
```



