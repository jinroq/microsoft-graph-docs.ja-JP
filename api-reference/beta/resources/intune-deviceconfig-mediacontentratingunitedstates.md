---
title: mediaContentRatingUnitedStates リソースの種類
description: まだ文書化されていません
author: tfitzmac
ms.openlocfilehash: ee10df5dd5e3f915e166cb77e747f8b3f7cc2d37
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 12/18/2018
ms.locfileid: "27341322"
---
# <a name="mediacontentratingunitedstates-resource-type"></a><span data-ttu-id="c528a-103">mediaContentRatingUnitedStates リソースの種類</span><span class="sxs-lookup"><span data-stu-id="c528a-103">mediaContentRatingUnitedStates resource type</span></span>

> <span data-ttu-id="c528a-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="c528a-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="c528a-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="c528a-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="c528a-106">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="c528a-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="c528a-107">まだ文書化されていません</span><span class="sxs-lookup"><span data-stu-id="c528a-107">Not yet documented</span></span>
## <a name="properties"></a><span data-ttu-id="c528a-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="c528a-108">Properties</span></span>
|<span data-ttu-id="c528a-109">プロパティ</span><span class="sxs-lookup"><span data-stu-id="c528a-109">Property</span></span>|<span data-ttu-id="c528a-110">種類</span><span class="sxs-lookup"><span data-stu-id="c528a-110">Type</span></span>|<span data-ttu-id="c528a-111">説明</span><span class="sxs-lookup"><span data-stu-id="c528a-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c528a-112">movieRating</span><span class="sxs-lookup"><span data-stu-id="c528a-112">movieRating</span></span>|[<span data-ttu-id="c528a-113">ratingUnitedStatesMoviesType</span><span class="sxs-lookup"><span data-stu-id="c528a-113">ratingUnitedStatesMoviesType</span></span>](../resources/intune-deviceconfig-ratingunitedstatesmoviestype.md)|<span data-ttu-id="c528a-114">評価の米国の選択したムービーです。</span><span class="sxs-lookup"><span data-stu-id="c528a-114">Movies rating selected for United States.</span></span> <span data-ttu-id="c528a-115">可能な値は、`allAllowed`、`allBlocked`、`general`、`parentalGuidance`、`parentalGuidance13`、`restricted`、`adults` です。</span><span class="sxs-lookup"><span data-stu-id="c528a-115">Possible values are: `allAllowed`, `allBlocked`, `general`, `parentalGuidance`, `parentalGuidance13`, `restricted`, `adults`.</span></span>|
|<span data-ttu-id="c528a-116">tvRating</span><span class="sxs-lookup"><span data-stu-id="c528a-116">tvRating</span></span>|[<span data-ttu-id="c528a-117">ratingUnitedStatesTelevisionType</span><span class="sxs-lookup"><span data-stu-id="c528a-117">ratingUnitedStatesTelevisionType</span></span>](../resources/intune-deviceconfig-ratingunitedstatestelevisiontype.md)|<span data-ttu-id="c528a-118">テレビの視聴制限はアメリカ合衆国を選択します。</span><span class="sxs-lookup"><span data-stu-id="c528a-118">TV rating selected for United States.</span></span> <span data-ttu-id="c528a-119">可能な値は、`allAllowed`、`allBlocked`、`childrenAll`、`childrenAbove7`、`general`、`parentalGuidance`、`childrenAbove14`、`adults` です。</span><span class="sxs-lookup"><span data-stu-id="c528a-119">Possible values are: `allAllowed`, `allBlocked`, `childrenAll`, `childrenAbove7`, `general`, `parentalGuidance`, `childrenAbove14`, `adults`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="c528a-120">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="c528a-120">Relationships</span></span>
<span data-ttu-id="c528a-121">なし</span><span class="sxs-lookup"><span data-stu-id="c528a-121">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="c528a-122">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="c528a-122">JSON Representation</span></span>
<span data-ttu-id="c528a-123">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="c528a-123">Here is a JSON representation of the resource.</span></span>
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





