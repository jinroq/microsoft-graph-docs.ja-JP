---
title: mediaContentRatingNewZealand リソースの種類
description: まだ文書化されていません
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 31d3dcf84b6343bcb03430fa27f901ca02580044
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/11/2019
ms.locfileid: "27837963"
---
# <a name="mediacontentratingnewzealand-resource-type"></a><span data-ttu-id="e0fe4-103">mediaContentRatingNewZealand リソースの種類</span><span class="sxs-lookup"><span data-stu-id="e0fe4-103">mediaContentRatingNewZealand resource type</span></span>

> <span data-ttu-id="e0fe4-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="e0fe4-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="e0fe4-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="e0fe4-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="e0fe4-106">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="e0fe4-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="e0fe4-107">まだ文書化されていません</span><span class="sxs-lookup"><span data-stu-id="e0fe4-107">Not yet documented</span></span>
## <a name="properties"></a><span data-ttu-id="e0fe4-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="e0fe4-108">Properties</span></span>
|<span data-ttu-id="e0fe4-109">プロパティ</span><span class="sxs-lookup"><span data-stu-id="e0fe4-109">Property</span></span>|<span data-ttu-id="e0fe4-110">種類</span><span class="sxs-lookup"><span data-stu-id="e0fe4-110">Type</span></span>|<span data-ttu-id="e0fe4-111">説明</span><span class="sxs-lookup"><span data-stu-id="e0fe4-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e0fe4-112">movieRating</span><span class="sxs-lookup"><span data-stu-id="e0fe4-112">movieRating</span></span>|[<span data-ttu-id="e0fe4-113">ratingNewZealandMoviesType</span><span class="sxs-lookup"><span data-stu-id="e0fe4-113">ratingNewZealandMoviesType</span></span>](../resources/intune-deviceconfig-ratingnewzealandmoviestype.md)|<span data-ttu-id="e0fe4-114">評価のニュージーランドを選択したムービーです。</span><span class="sxs-lookup"><span data-stu-id="e0fe4-114">Movies rating selected for New Zealand.</span></span> <span data-ttu-id="e0fe4-115">可能な値は、`allAllowed`、`allBlocked`、`general`、`parentalGuidance`、`mature`、`agesAbove13`、`agesAbove15`、`agesAbove16`、`agesAbove18`、`restricted`、`agesAbove16Restricted` です。</span><span class="sxs-lookup"><span data-stu-id="e0fe4-115">Possible values are: `allAllowed`, `allBlocked`, `general`, `parentalGuidance`, `mature`, `agesAbove13`, `agesAbove15`, `agesAbove16`, `agesAbove18`, `restricted`, `agesAbove16Restricted`.</span></span>|
|<span data-ttu-id="e0fe4-116">tvRating</span><span class="sxs-lookup"><span data-stu-id="e0fe4-116">tvRating</span></span>|[<span data-ttu-id="e0fe4-117">ratingNewZealandTelevisionType</span><span class="sxs-lookup"><span data-stu-id="e0fe4-117">ratingNewZealandTelevisionType</span></span>](../resources/intune-deviceconfig-ratingnewzealandtelevisiontype.md)|<span data-ttu-id="e0fe4-118">テレビの視聴制限がニュージーランドを選択します。</span><span class="sxs-lookup"><span data-stu-id="e0fe4-118">TV rating selected for New Zealand.</span></span> <span data-ttu-id="e0fe4-119">可能な値は、`allAllowed`、`allBlocked`、`general`、`parentalGuidance`、`adults` です。</span><span class="sxs-lookup"><span data-stu-id="e0fe4-119">Possible values are: `allAllowed`, `allBlocked`, `general`, `parentalGuidance`, `adults`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="e0fe4-120">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="e0fe4-120">Relationships</span></span>
<span data-ttu-id="e0fe4-121">なし</span><span class="sxs-lookup"><span data-stu-id="e0fe4-121">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="e0fe4-122">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="e0fe4-122">JSON Representation</span></span>
<span data-ttu-id="e0fe4-123">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="e0fe4-123">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.mediaContentRatingNewZealand"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.mediaContentRatingNewZealand",
  "movieRating": "String",
  "tvRating": "String"
}
```





