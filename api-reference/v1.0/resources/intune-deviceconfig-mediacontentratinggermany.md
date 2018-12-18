---
title: mediaContentRatingGermany リソースの種類
description: まだ文書化されていません
author: tfitzmac
ms.openlocfilehash: 8add327725e5d3886d381b63c7debc16c256d810
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 12/18/2018
ms.locfileid: "27327700"
---
# <a name="mediacontentratinggermany-resource-type"></a><span data-ttu-id="7b51f-103">mediaContentRatingGermany リソースの種類</span><span class="sxs-lookup"><span data-stu-id="7b51f-103">mediaContentRatingGermany resource type</span></span>

> <span data-ttu-id="7b51f-104">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="7b51f-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="7b51f-105">まだ文書化されていません</span><span class="sxs-lookup"><span data-stu-id="7b51f-105">Not yet documented</span></span>
## <a name="properties"></a><span data-ttu-id="7b51f-106">プロパティ</span><span class="sxs-lookup"><span data-stu-id="7b51f-106">Properties</span></span>
|<span data-ttu-id="7b51f-107">プロパティ</span><span class="sxs-lookup"><span data-stu-id="7b51f-107">Property</span></span>|<span data-ttu-id="7b51f-108">種類</span><span class="sxs-lookup"><span data-stu-id="7b51f-108">Type</span></span>|<span data-ttu-id="7b51f-109">説明</span><span class="sxs-lookup"><span data-stu-id="7b51f-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="7b51f-110">movieRating</span><span class="sxs-lookup"><span data-stu-id="7b51f-110">movieRating</span></span>|[<span data-ttu-id="7b51f-111">ratingGermanyMoviesType</span><span class="sxs-lookup"><span data-stu-id="7b51f-111">ratingGermanyMoviesType</span></span>](../resources/intune-deviceconfig-ratinggermanymoviestype.md)|<span data-ttu-id="7b51f-112">映画がドイツの選択を評価します。</span><span class="sxs-lookup"><span data-stu-id="7b51f-112">Movies rating selected for Germany.</span></span> <span data-ttu-id="7b51f-113">可能な値は、`allAllowed`、`allBlocked`、`general`、`agesAbove6`、`agesAbove12`、`agesAbove16`、`adults` です。</span><span class="sxs-lookup"><span data-stu-id="7b51f-113">Possible values are: `allAllowed`, `allBlocked`, `general`, `agesAbove6`, `agesAbove12`, `agesAbove16`, `adults`.</span></span>|
|<span data-ttu-id="7b51f-114">tvRating</span><span class="sxs-lookup"><span data-stu-id="7b51f-114">tvRating</span></span>|[<span data-ttu-id="7b51f-115">ratingGermanyTelevisionType</span><span class="sxs-lookup"><span data-stu-id="7b51f-115">ratingGermanyTelevisionType</span></span>](../resources/intune-deviceconfig-ratinggermanytelevisiontype.md)|<span data-ttu-id="7b51f-116">テレビの視聴制限がドイツを選択します。</span><span class="sxs-lookup"><span data-stu-id="7b51f-116">TV rating selected for Germany.</span></span> <span data-ttu-id="7b51f-117">可能な値は、`allAllowed`、`allBlocked`、`general`、`agesAbove6`、`agesAbove12`、`agesAbove16`、`adults` です。</span><span class="sxs-lookup"><span data-stu-id="7b51f-117">Possible values are: `allAllowed`, `allBlocked`, `general`, `agesAbove6`, `agesAbove12`, `agesAbove16`, `adults`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="7b51f-118">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="7b51f-118">Relationships</span></span>
<span data-ttu-id="7b51f-119">なし</span><span class="sxs-lookup"><span data-stu-id="7b51f-119">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="7b51f-120">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="7b51f-120">JSON Representation</span></span>
<span data-ttu-id="7b51f-121">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="7b51f-121">Here is a JSON representation of the resource.</span></span>
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



