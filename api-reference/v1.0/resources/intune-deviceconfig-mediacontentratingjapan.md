---
title: mediaContentRatingJapan リソースの種類
description: まだ文書化されていません
author: tfitzmac
ms.openlocfilehash: 1913b28b3020ffdc51edea1a8d93dd726d70efdd
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 12/18/2018
ms.locfileid: "27328470"
---
# <a name="mediacontentratingjapan-resource-type"></a><span data-ttu-id="abe41-103">mediaContentRatingJapan リソースの種類</span><span class="sxs-lookup"><span data-stu-id="abe41-103">mediaContentRatingJapan resource type</span></span>

> <span data-ttu-id="abe41-104">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="abe41-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="abe41-105">まだ文書化されていません</span><span class="sxs-lookup"><span data-stu-id="abe41-105">Not yet documented</span></span>
## <a name="properties"></a><span data-ttu-id="abe41-106">プロパティ</span><span class="sxs-lookup"><span data-stu-id="abe41-106">Properties</span></span>
|<span data-ttu-id="abe41-107">プロパティ</span><span class="sxs-lookup"><span data-stu-id="abe41-107">Property</span></span>|<span data-ttu-id="abe41-108">種類</span><span class="sxs-lookup"><span data-stu-id="abe41-108">Type</span></span>|<span data-ttu-id="abe41-109">説明</span><span class="sxs-lookup"><span data-stu-id="abe41-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="abe41-110">movieRating</span><span class="sxs-lookup"><span data-stu-id="abe41-110">movieRating</span></span>|[<span data-ttu-id="abe41-111">ratingJapanMoviesType</span><span class="sxs-lookup"><span data-stu-id="abe41-111">ratingJapanMoviesType</span></span>](../resources/intune-deviceconfig-ratingjapanmoviestype.md)|<span data-ttu-id="abe41-112">評価日本の選択したムービーです。</span><span class="sxs-lookup"><span data-stu-id="abe41-112">Movies rating selected for Japan.</span></span> <span data-ttu-id="abe41-113">使用可能な値: `allAllowed`、`allBlocked`、`general`、`parentalGuidance`、`agesAbove15`、`agesAbove18`。</span><span class="sxs-lookup"><span data-stu-id="abe41-113">Possible values are: `allAllowed`, `allBlocked`, `general`, `parentalGuidance`, `agesAbove15`, `agesAbove18`.</span></span>|
|<span data-ttu-id="abe41-114">tvRating</span><span class="sxs-lookup"><span data-stu-id="abe41-114">tvRating</span></span>|[<span data-ttu-id="abe41-115">ratingJapanTelevisionType</span><span class="sxs-lookup"><span data-stu-id="abe41-115">ratingJapanTelevisionType</span></span>](../resources/intune-deviceconfig-ratingjapantelevisiontype.md)|<span data-ttu-id="abe41-116">テレビの視聴制限が日本用に選択します。</span><span class="sxs-lookup"><span data-stu-id="abe41-116">TV rating selected for Japan.</span></span> <span data-ttu-id="abe41-117">可能な値は、`allAllowed`、`allBlocked`、`explicitAllowed` です。</span><span class="sxs-lookup"><span data-stu-id="abe41-117">Possible values are: `allAllowed`, `allBlocked`, `explicitAllowed`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="abe41-118">関係</span><span class="sxs-lookup"><span data-stu-id="abe41-118">Relationships</span></span>
<span data-ttu-id="abe41-119">なし</span><span class="sxs-lookup"><span data-stu-id="abe41-119">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="abe41-120">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="abe41-120">JSON Representation</span></span>
<span data-ttu-id="abe41-121">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="abe41-121">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.mediaContentRatingJapan"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.mediaContentRatingJapan",
  "movieRating": "String",
  "tvRating": "String"
}
```


