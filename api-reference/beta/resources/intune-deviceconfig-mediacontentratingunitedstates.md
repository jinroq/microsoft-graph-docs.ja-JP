---
title: mediaContentRatingUnitedStates リソースの種類
description: まだ文書化されていません
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: cebfd525eb77c3e6e939605b80693e733f594e7d
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/12/2019
ms.locfileid: "27912611"
---
# <a name="mediacontentratingunitedstates-resource-type"></a><span data-ttu-id="3af7b-103">mediaContentRatingUnitedStates リソースの種類</span><span class="sxs-lookup"><span data-stu-id="3af7b-103">mediaContentRatingUnitedStates resource type</span></span>

> <span data-ttu-id="3af7b-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="3af7b-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="3af7b-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="3af7b-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="3af7b-106">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="3af7b-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="3af7b-107">まだ文書化されていません</span><span class="sxs-lookup"><span data-stu-id="3af7b-107">Not yet documented</span></span>
## <a name="properties"></a><span data-ttu-id="3af7b-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="3af7b-108">Properties</span></span>
|<span data-ttu-id="3af7b-109">プロパティ</span><span class="sxs-lookup"><span data-stu-id="3af7b-109">Property</span></span>|<span data-ttu-id="3af7b-110">種類</span><span class="sxs-lookup"><span data-stu-id="3af7b-110">Type</span></span>|<span data-ttu-id="3af7b-111">説明</span><span class="sxs-lookup"><span data-stu-id="3af7b-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="3af7b-112">movieRating</span><span class="sxs-lookup"><span data-stu-id="3af7b-112">movieRating</span></span>|[<span data-ttu-id="3af7b-113">ratingUnitedStatesMoviesType</span><span class="sxs-lookup"><span data-stu-id="3af7b-113">ratingUnitedStatesMoviesType</span></span>](../resources/intune-deviceconfig-ratingunitedstatesmoviestype.md)|<span data-ttu-id="3af7b-114">評価の米国の選択したムービーです。</span><span class="sxs-lookup"><span data-stu-id="3af7b-114">Movies rating selected for United States.</span></span> <span data-ttu-id="3af7b-115">可能な値は、`allAllowed`、`allBlocked`、`general`、`parentalGuidance`、`parentalGuidance13`、`restricted`、`adults` です。</span><span class="sxs-lookup"><span data-stu-id="3af7b-115">Possible values are: `allAllowed`, `allBlocked`, `general`, `parentalGuidance`, `parentalGuidance13`, `restricted`, `adults`.</span></span>|
|<span data-ttu-id="3af7b-116">tvRating</span><span class="sxs-lookup"><span data-stu-id="3af7b-116">tvRating</span></span>|[<span data-ttu-id="3af7b-117">ratingUnitedStatesTelevisionType</span><span class="sxs-lookup"><span data-stu-id="3af7b-117">ratingUnitedStatesTelevisionType</span></span>](../resources/intune-deviceconfig-ratingunitedstatestelevisiontype.md)|<span data-ttu-id="3af7b-118">テレビの視聴制限はアメリカ合衆国を選択します。</span><span class="sxs-lookup"><span data-stu-id="3af7b-118">TV rating selected for United States.</span></span> <span data-ttu-id="3af7b-119">可能な値は、`allAllowed`、`allBlocked`、`childrenAll`、`childrenAbove7`、`general`、`parentalGuidance`、`childrenAbove14`、`adults` です。</span><span class="sxs-lookup"><span data-stu-id="3af7b-119">Possible values are: `allAllowed`, `allBlocked`, `childrenAll`, `childrenAbove7`, `general`, `parentalGuidance`, `childrenAbove14`, `adults`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="3af7b-120">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="3af7b-120">Relationships</span></span>
<span data-ttu-id="3af7b-121">なし</span><span class="sxs-lookup"><span data-stu-id="3af7b-121">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="3af7b-122">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="3af7b-122">JSON Representation</span></span>
<span data-ttu-id="3af7b-123">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="3af7b-123">Here is a JSON representation of the resource.</span></span>
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





