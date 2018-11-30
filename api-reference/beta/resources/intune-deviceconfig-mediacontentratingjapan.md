---
title: mediaContentRatingJapan リソースの種類
description: まだ文書化されていません
ms.openlocfilehash: 2fdf6ea6115f066df697a778e44e0476feac7d96
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27068179"
---
# <a name="mediacontentratingjapan-resource-type"></a><span data-ttu-id="b73ce-103">mediaContentRatingJapan リソースの種類</span><span class="sxs-lookup"><span data-stu-id="b73ce-103">mediaContentRatingJapan resource type</span></span>

> <span data-ttu-id="b73ce-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="b73ce-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="b73ce-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="b73ce-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="b73ce-106">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="b73ce-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="b73ce-107">まだ文書化されていません</span><span class="sxs-lookup"><span data-stu-id="b73ce-107">Not yet documented</span></span>
## <a name="properties"></a><span data-ttu-id="b73ce-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="b73ce-108">Properties</span></span>
|<span data-ttu-id="b73ce-109">プロパティ</span><span class="sxs-lookup"><span data-stu-id="b73ce-109">Property</span></span>|<span data-ttu-id="b73ce-110">型</span><span class="sxs-lookup"><span data-stu-id="b73ce-110">Type</span></span>|<span data-ttu-id="b73ce-111">説明</span><span class="sxs-lookup"><span data-stu-id="b73ce-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b73ce-112">movieRating</span><span class="sxs-lookup"><span data-stu-id="b73ce-112">movieRating</span></span>|[<span data-ttu-id="b73ce-113">ratingJapanMoviesType</span><span class="sxs-lookup"><span data-stu-id="b73ce-113">ratingJapanMoviesType</span></span>](../resources/intune-deviceconfig-ratingjapanmoviestype.md)|<span data-ttu-id="b73ce-114">評価日本の選択したムービーです。</span><span class="sxs-lookup"><span data-stu-id="b73ce-114">Movies rating selected for Japan.</span></span> <span data-ttu-id="b73ce-115">使用可能な値: `allAllowed`、`allBlocked`、`general`、`parentalGuidance`、`agesAbove15`、`agesAbove18`。</span><span class="sxs-lookup"><span data-stu-id="b73ce-115">Possible values are: `allAllowed`, `allBlocked`, `general`, `parentalGuidance`, `agesAbove15`, `agesAbove18`.</span></span>|
|<span data-ttu-id="b73ce-116">tvRating</span><span class="sxs-lookup"><span data-stu-id="b73ce-116">tvRating</span></span>|[<span data-ttu-id="b73ce-117">ratingJapanTelevisionType</span><span class="sxs-lookup"><span data-stu-id="b73ce-117">ratingJapanTelevisionType</span></span>](../resources/intune-deviceconfig-ratingjapantelevisiontype.md)|<span data-ttu-id="b73ce-118">テレビの視聴制限が日本用に選択します。</span><span class="sxs-lookup"><span data-stu-id="b73ce-118">TV rating selected for Japan.</span></span> <span data-ttu-id="b73ce-119">可能な値は、`allAllowed`、`allBlocked`、`explicitAllowed` です。</span><span class="sxs-lookup"><span data-stu-id="b73ce-119">Possible values are: `allAllowed`, `allBlocked`, `explicitAllowed`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="b73ce-120">関係</span><span class="sxs-lookup"><span data-stu-id="b73ce-120">Relationships</span></span>
<span data-ttu-id="b73ce-121">なし</span><span class="sxs-lookup"><span data-stu-id="b73ce-121">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="b73ce-122">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="b73ce-122">JSON Representation</span></span>
<span data-ttu-id="b73ce-123">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="b73ce-123">Here is a JSON representation of the resource.</span></span>
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





