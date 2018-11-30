---
title: mediaContentRatingUnitedStates リソースの種類
description: まだ文書化されていません
ms.openlocfilehash: b96241f31e232f39f62a09d7fff8560e5a89e237
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27023200"
---
# <a name="mediacontentratingunitedstates-resource-type"></a><span data-ttu-id="39019-103">mediaContentRatingUnitedStates リソースの種類</span><span class="sxs-lookup"><span data-stu-id="39019-103">mediaContentRatingUnitedStates resource type</span></span>

> <span data-ttu-id="39019-104">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="39019-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="39019-105">まだ文書化されていません</span><span class="sxs-lookup"><span data-stu-id="39019-105">Not yet documented</span></span>
## <a name="properties"></a><span data-ttu-id="39019-106">プロパティ</span><span class="sxs-lookup"><span data-stu-id="39019-106">Properties</span></span>
|<span data-ttu-id="39019-107">プロパティ</span><span class="sxs-lookup"><span data-stu-id="39019-107">Property</span></span>|<span data-ttu-id="39019-108">型</span><span class="sxs-lookup"><span data-stu-id="39019-108">Type</span></span>|<span data-ttu-id="39019-109">説明</span><span class="sxs-lookup"><span data-stu-id="39019-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="39019-110">movieRating</span><span class="sxs-lookup"><span data-stu-id="39019-110">movieRating</span></span>|[<span data-ttu-id="39019-111">ratingUnitedStatesMoviesType</span><span class="sxs-lookup"><span data-stu-id="39019-111">ratingUnitedStatesMoviesType</span></span>](../resources/intune-deviceconfig-ratingunitedstatesmoviestype.md)|<span data-ttu-id="39019-112">評価の米国の選択したムービーです。</span><span class="sxs-lookup"><span data-stu-id="39019-112">Movies rating selected for United States.</span></span> <span data-ttu-id="39019-113">可能な値は、`allAllowed`、`allBlocked`、`general`、`parentalGuidance`、`parentalGuidance13`、`restricted`、`adults` です。</span><span class="sxs-lookup"><span data-stu-id="39019-113">Possible values are: `allAllowed`, `allBlocked`, `general`, `parentalGuidance`, `parentalGuidance13`, `restricted`, `adults`.</span></span>|
|<span data-ttu-id="39019-114">tvRating</span><span class="sxs-lookup"><span data-stu-id="39019-114">tvRating</span></span>|[<span data-ttu-id="39019-115">ratingUnitedStatesTelevisionType</span><span class="sxs-lookup"><span data-stu-id="39019-115">ratingUnitedStatesTelevisionType</span></span>](../resources/intune-deviceconfig-ratingunitedstatestelevisiontype.md)|<span data-ttu-id="39019-116">テレビの視聴制限はアメリカ合衆国を選択します。</span><span class="sxs-lookup"><span data-stu-id="39019-116">TV rating selected for United States.</span></span> <span data-ttu-id="39019-117">可能な値は、`allAllowed`、`allBlocked`、`childrenAll`、`childrenAbove7`、`general`、`parentalGuidance`、`childrenAbove14`、`adults` です。</span><span class="sxs-lookup"><span data-stu-id="39019-117">Possible values are: `allAllowed`, `allBlocked`, `childrenAll`, `childrenAbove7`, `general`, `parentalGuidance`, `childrenAbove14`, `adults`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="39019-118">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="39019-118">Relationships</span></span>
<span data-ttu-id="39019-119">なし</span><span class="sxs-lookup"><span data-stu-id="39019-119">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="39019-120">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="39019-120">JSON Representation</span></span>
<span data-ttu-id="39019-121">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="39019-121">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.mediaContentRatingUnitedStates"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.mediaContentRatingUnitedStates",
  "movieRating": "String",
  "tvRating": "String"
}
```



