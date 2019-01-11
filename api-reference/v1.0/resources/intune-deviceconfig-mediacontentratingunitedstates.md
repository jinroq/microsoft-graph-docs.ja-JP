---
title: mediaContentRatingUnitedStates リソースの種類
description: まだ文書化されていません
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 28229d14f5914bcae9a014fca587ad03b6236647
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/11/2019
ms.locfileid: "27879605"
---
# <a name="mediacontentratingunitedstates-resource-type"></a><span data-ttu-id="49eec-103">mediaContentRatingUnitedStates リソースの種類</span><span class="sxs-lookup"><span data-stu-id="49eec-103">mediaContentRatingUnitedStates resource type</span></span>

> <span data-ttu-id="49eec-104">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="49eec-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="49eec-105">まだ文書化されていません</span><span class="sxs-lookup"><span data-stu-id="49eec-105">Not yet documented</span></span>
## <a name="properties"></a><span data-ttu-id="49eec-106">プロパティ</span><span class="sxs-lookup"><span data-stu-id="49eec-106">Properties</span></span>
|<span data-ttu-id="49eec-107">プロパティ</span><span class="sxs-lookup"><span data-stu-id="49eec-107">Property</span></span>|<span data-ttu-id="49eec-108">種類</span><span class="sxs-lookup"><span data-stu-id="49eec-108">Type</span></span>|<span data-ttu-id="49eec-109">説明</span><span class="sxs-lookup"><span data-stu-id="49eec-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="49eec-110">movieRating</span><span class="sxs-lookup"><span data-stu-id="49eec-110">movieRating</span></span>|[<span data-ttu-id="49eec-111">ratingUnitedStatesMoviesType</span><span class="sxs-lookup"><span data-stu-id="49eec-111">ratingUnitedStatesMoviesType</span></span>](../resources/intune-deviceconfig-ratingunitedstatesmoviestype.md)|<span data-ttu-id="49eec-112">評価の米国の選択したムービーです。</span><span class="sxs-lookup"><span data-stu-id="49eec-112">Movies rating selected for United States.</span></span> <span data-ttu-id="49eec-113">可能な値は、`allAllowed`、`allBlocked`、`general`、`parentalGuidance`、`parentalGuidance13`、`restricted`、`adults` です。</span><span class="sxs-lookup"><span data-stu-id="49eec-113">Possible values are: `allAllowed`, `allBlocked`, `general`, `parentalGuidance`, `parentalGuidance13`, `restricted`, `adults`.</span></span>|
|<span data-ttu-id="49eec-114">tvRating</span><span class="sxs-lookup"><span data-stu-id="49eec-114">tvRating</span></span>|[<span data-ttu-id="49eec-115">ratingUnitedStatesTelevisionType</span><span class="sxs-lookup"><span data-stu-id="49eec-115">ratingUnitedStatesTelevisionType</span></span>](../resources/intune-deviceconfig-ratingunitedstatestelevisiontype.md)|<span data-ttu-id="49eec-116">テレビの視聴制限はアメリカ合衆国を選択します。</span><span class="sxs-lookup"><span data-stu-id="49eec-116">TV rating selected for United States.</span></span> <span data-ttu-id="49eec-117">可能な値は、`allAllowed`、`allBlocked`、`childrenAll`、`childrenAbove7`、`general`、`parentalGuidance`、`childrenAbove14`、`adults` です。</span><span class="sxs-lookup"><span data-stu-id="49eec-117">Possible values are: `allAllowed`, `allBlocked`, `childrenAll`, `childrenAbove7`, `general`, `parentalGuidance`, `childrenAbove14`, `adults`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="49eec-118">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="49eec-118">Relationships</span></span>
<span data-ttu-id="49eec-119">なし</span><span class="sxs-lookup"><span data-stu-id="49eec-119">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="49eec-120">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="49eec-120">JSON Representation</span></span>
<span data-ttu-id="49eec-121">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="49eec-121">Here is a JSON representation of the resource.</span></span>
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



