---
title: mediaContentRatingFrance リソースの種類
description: まだ文書化されていません
author: tfitzmac
ms.openlocfilehash: 0981a73fdc1e8468d9e8ab8590387dfa357a39c9
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 12/18/2018
ms.locfileid: "27361643"
---
# <a name="mediacontentratingfrance-resource-type"></a><span data-ttu-id="8b30d-103">mediaContentRatingFrance リソースの種類</span><span class="sxs-lookup"><span data-stu-id="8b30d-103">mediaContentRatingFrance resource type</span></span>

> <span data-ttu-id="8b30d-104">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="8b30d-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="8b30d-105">まだ文書化されていません</span><span class="sxs-lookup"><span data-stu-id="8b30d-105">Not yet documented</span></span>
## <a name="properties"></a><span data-ttu-id="8b30d-106">プロパティ</span><span class="sxs-lookup"><span data-stu-id="8b30d-106">Properties</span></span>
|<span data-ttu-id="8b30d-107">プロパティ</span><span class="sxs-lookup"><span data-stu-id="8b30d-107">Property</span></span>|<span data-ttu-id="8b30d-108">種類</span><span class="sxs-lookup"><span data-stu-id="8b30d-108">Type</span></span>|<span data-ttu-id="8b30d-109">説明</span><span class="sxs-lookup"><span data-stu-id="8b30d-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="8b30d-110">movieRating</span><span class="sxs-lookup"><span data-stu-id="8b30d-110">movieRating</span></span>|[<span data-ttu-id="8b30d-111">ratingFranceMoviesType</span><span class="sxs-lookup"><span data-stu-id="8b30d-111">ratingFranceMoviesType</span></span>](../resources/intune-deviceconfig-ratingfrancemoviestype.md)|<span data-ttu-id="8b30d-112">映画はフランスの選択を評価します。</span><span class="sxs-lookup"><span data-stu-id="8b30d-112">Movies rating selected for France.</span></span> <span data-ttu-id="8b30d-113">使用可能な値: `allAllowed`、`allBlocked`、`agesAbove10`、`agesAbove12`、`agesAbove16`、`agesAbove18`。</span><span class="sxs-lookup"><span data-stu-id="8b30d-113">Possible values are: `allAllowed`, `allBlocked`, `agesAbove10`, `agesAbove12`, `agesAbove16`, `agesAbove18`.</span></span>|
|<span data-ttu-id="8b30d-114">tvRating</span><span class="sxs-lookup"><span data-stu-id="8b30d-114">tvRating</span></span>|[<span data-ttu-id="8b30d-115">ratingFranceTelevisionType</span><span class="sxs-lookup"><span data-stu-id="8b30d-115">ratingFranceTelevisionType</span></span>](../resources/intune-deviceconfig-ratingfrancetelevisiontype.md)|<span data-ttu-id="8b30d-116">テレビの視聴制限がフランス用に選択します。</span><span class="sxs-lookup"><span data-stu-id="8b30d-116">TV rating selected for France.</span></span> <span data-ttu-id="8b30d-117">使用可能な値: `allAllowed`、`allBlocked`、`agesAbove10`、`agesAbove12`、`agesAbove16`、`agesAbove18`。</span><span class="sxs-lookup"><span data-stu-id="8b30d-117">Possible values are: `allAllowed`, `allBlocked`, `agesAbove10`, `agesAbove12`, `agesAbove16`, `agesAbove18`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="8b30d-118">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="8b30d-118">Relationships</span></span>
<span data-ttu-id="8b30d-119">なし</span><span class="sxs-lookup"><span data-stu-id="8b30d-119">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="8b30d-120">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="8b30d-120">JSON Representation</span></span>
<span data-ttu-id="8b30d-121">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="8b30d-121">Here is a JSON representation of the resource.</span></span>
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



