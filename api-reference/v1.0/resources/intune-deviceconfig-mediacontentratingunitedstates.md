---
title: mediaContentRatingUnitedStates リソースの種類
description: まだ文書化されていません
author: tfitzmac
ms.openlocfilehash: b69e09684097ffbd85cf8117e4dd17779cbc5c67
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 12/18/2018
ms.locfileid: "27319454"
---
# <a name="mediacontentratingunitedstates-resource-type"></a><span data-ttu-id="e51b3-103">mediaContentRatingUnitedStates リソースの種類</span><span class="sxs-lookup"><span data-stu-id="e51b3-103">mediaContentRatingUnitedStates resource type</span></span>

> <span data-ttu-id="e51b3-104">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="e51b3-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="e51b3-105">まだ文書化されていません</span><span class="sxs-lookup"><span data-stu-id="e51b3-105">Not yet documented</span></span>
## <a name="properties"></a><span data-ttu-id="e51b3-106">プロパティ</span><span class="sxs-lookup"><span data-stu-id="e51b3-106">Properties</span></span>
|<span data-ttu-id="e51b3-107">プロパティ</span><span class="sxs-lookup"><span data-stu-id="e51b3-107">Property</span></span>|<span data-ttu-id="e51b3-108">種類</span><span class="sxs-lookup"><span data-stu-id="e51b3-108">Type</span></span>|<span data-ttu-id="e51b3-109">説明</span><span class="sxs-lookup"><span data-stu-id="e51b3-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e51b3-110">movieRating</span><span class="sxs-lookup"><span data-stu-id="e51b3-110">movieRating</span></span>|[<span data-ttu-id="e51b3-111">ratingUnitedStatesMoviesType</span><span class="sxs-lookup"><span data-stu-id="e51b3-111">ratingUnitedStatesMoviesType</span></span>](../resources/intune-deviceconfig-ratingunitedstatesmoviestype.md)|<span data-ttu-id="e51b3-112">評価の米国の選択したムービーです。</span><span class="sxs-lookup"><span data-stu-id="e51b3-112">Movies rating selected for United States.</span></span> <span data-ttu-id="e51b3-113">可能な値は、`allAllowed`、`allBlocked`、`general`、`parentalGuidance`、`parentalGuidance13`、`restricted`、`adults` です。</span><span class="sxs-lookup"><span data-stu-id="e51b3-113">Possible values are: `allAllowed`, `allBlocked`, `general`, `parentalGuidance`, `parentalGuidance13`, `restricted`, `adults`.</span></span>|
|<span data-ttu-id="e51b3-114">tvRating</span><span class="sxs-lookup"><span data-stu-id="e51b3-114">tvRating</span></span>|[<span data-ttu-id="e51b3-115">ratingUnitedStatesTelevisionType</span><span class="sxs-lookup"><span data-stu-id="e51b3-115">ratingUnitedStatesTelevisionType</span></span>](../resources/intune-deviceconfig-ratingunitedstatestelevisiontype.md)|<span data-ttu-id="e51b3-116">テレビの視聴制限はアメリカ合衆国を選択します。</span><span class="sxs-lookup"><span data-stu-id="e51b3-116">TV rating selected for United States.</span></span> <span data-ttu-id="e51b3-117">可能な値は、`allAllowed`、`allBlocked`、`childrenAll`、`childrenAbove7`、`general`、`parentalGuidance`、`childrenAbove14`、`adults` です。</span><span class="sxs-lookup"><span data-stu-id="e51b3-117">Possible values are: `allAllowed`, `allBlocked`, `childrenAll`, `childrenAbove7`, `general`, `parentalGuidance`, `childrenAbove14`, `adults`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="e51b3-118">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="e51b3-118">Relationships</span></span>
<span data-ttu-id="e51b3-119">なし</span><span class="sxs-lookup"><span data-stu-id="e51b3-119">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="e51b3-120">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="e51b3-120">JSON Representation</span></span>
<span data-ttu-id="e51b3-121">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="e51b3-121">Here is a JSON representation of the resource.</span></span>
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



