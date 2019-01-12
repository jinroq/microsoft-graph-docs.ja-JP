---
title: mediaContentRatingUnitedStates リソースの種類
description: まだ文書化されていません
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 3e37a707b7ad190ddc1f3206f149d0dcc3c1aad3
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/12/2019
ms.locfileid: "27959225"
---
# <a name="mediacontentratingunitedstates-resource-type"></a><span data-ttu-id="97b03-103">mediaContentRatingUnitedStates リソースの種類</span><span class="sxs-lookup"><span data-stu-id="97b03-103">mediaContentRatingUnitedStates resource type</span></span>

> <span data-ttu-id="97b03-104">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="97b03-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="97b03-105">まだ文書化されていません</span><span class="sxs-lookup"><span data-stu-id="97b03-105">Not yet documented</span></span>
## <a name="properties"></a><span data-ttu-id="97b03-106">プロパティ</span><span class="sxs-lookup"><span data-stu-id="97b03-106">Properties</span></span>
|<span data-ttu-id="97b03-107">プロパティ</span><span class="sxs-lookup"><span data-stu-id="97b03-107">Property</span></span>|<span data-ttu-id="97b03-108">種類</span><span class="sxs-lookup"><span data-stu-id="97b03-108">Type</span></span>|<span data-ttu-id="97b03-109">説明</span><span class="sxs-lookup"><span data-stu-id="97b03-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="97b03-110">movieRating</span><span class="sxs-lookup"><span data-stu-id="97b03-110">movieRating</span></span>|[<span data-ttu-id="97b03-111">ratingUnitedStatesMoviesType</span><span class="sxs-lookup"><span data-stu-id="97b03-111">ratingUnitedStatesMoviesType</span></span>](../resources/intune-deviceconfig-ratingunitedstatesmoviestype.md)|<span data-ttu-id="97b03-112">評価の米国の選択したムービーです。</span><span class="sxs-lookup"><span data-stu-id="97b03-112">Movies rating selected for United States.</span></span> <span data-ttu-id="97b03-113">可能な値は、`allAllowed`、`allBlocked`、`general`、`parentalGuidance`、`parentalGuidance13`、`restricted`、`adults` です。</span><span class="sxs-lookup"><span data-stu-id="97b03-113">Possible values are: `allAllowed`, `allBlocked`, `general`, `parentalGuidance`, `parentalGuidance13`, `restricted`, `adults`.</span></span>|
|<span data-ttu-id="97b03-114">tvRating</span><span class="sxs-lookup"><span data-stu-id="97b03-114">tvRating</span></span>|[<span data-ttu-id="97b03-115">ratingUnitedStatesTelevisionType</span><span class="sxs-lookup"><span data-stu-id="97b03-115">ratingUnitedStatesTelevisionType</span></span>](../resources/intune-deviceconfig-ratingunitedstatestelevisiontype.md)|<span data-ttu-id="97b03-116">テレビの視聴制限はアメリカ合衆国を選択します。</span><span class="sxs-lookup"><span data-stu-id="97b03-116">TV rating selected for United States.</span></span> <span data-ttu-id="97b03-117">可能な値は、`allAllowed`、`allBlocked`、`childrenAll`、`childrenAbove7`、`general`、`parentalGuidance`、`childrenAbove14`、`adults` です。</span><span class="sxs-lookup"><span data-stu-id="97b03-117">Possible values are: `allAllowed`, `allBlocked`, `childrenAll`, `childrenAbove7`, `general`, `parentalGuidance`, `childrenAbove14`, `adults`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="97b03-118">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="97b03-118">Relationships</span></span>
<span data-ttu-id="97b03-119">なし</span><span class="sxs-lookup"><span data-stu-id="97b03-119">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="97b03-120">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="97b03-120">JSON Representation</span></span>
<span data-ttu-id="97b03-121">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="97b03-121">Here is a JSON representation of the resource.</span></span>
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



