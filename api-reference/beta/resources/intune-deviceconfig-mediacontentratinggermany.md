---
title: mediaContentRatingGermany リソースの種類
description: まだ文書化されていません
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: f9602b688cb1e4acda7531bbfc6b5a1f4d66a3e2
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/12/2019
ms.locfileid: "27923489"
---
# <a name="mediacontentratinggermany-resource-type"></a><span data-ttu-id="646fc-103">mediaContentRatingGermany リソースの種類</span><span class="sxs-lookup"><span data-stu-id="646fc-103">mediaContentRatingGermany resource type</span></span>

> <span data-ttu-id="646fc-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="646fc-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="646fc-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="646fc-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="646fc-106">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="646fc-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="646fc-107">まだ文書化されていません</span><span class="sxs-lookup"><span data-stu-id="646fc-107">Not yet documented</span></span>
## <a name="properties"></a><span data-ttu-id="646fc-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="646fc-108">Properties</span></span>
|<span data-ttu-id="646fc-109">プロパティ</span><span class="sxs-lookup"><span data-stu-id="646fc-109">Property</span></span>|<span data-ttu-id="646fc-110">種類</span><span class="sxs-lookup"><span data-stu-id="646fc-110">Type</span></span>|<span data-ttu-id="646fc-111">説明</span><span class="sxs-lookup"><span data-stu-id="646fc-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="646fc-112">movieRating</span><span class="sxs-lookup"><span data-stu-id="646fc-112">movieRating</span></span>|[<span data-ttu-id="646fc-113">ratingGermanyMoviesType</span><span class="sxs-lookup"><span data-stu-id="646fc-113">ratingGermanyMoviesType</span></span>](../resources/intune-deviceconfig-ratinggermanymoviestype.md)|<span data-ttu-id="646fc-114">映画がドイツの選択を評価します。</span><span class="sxs-lookup"><span data-stu-id="646fc-114">Movies rating selected for Germany.</span></span> <span data-ttu-id="646fc-115">可能な値は、`allAllowed`、`allBlocked`、`general`、`agesAbove6`、`agesAbove12`、`agesAbove16`、`adults` です。</span><span class="sxs-lookup"><span data-stu-id="646fc-115">Possible values are: `allAllowed`, `allBlocked`, `general`, `agesAbove6`, `agesAbove12`, `agesAbove16`, `adults`.</span></span>|
|<span data-ttu-id="646fc-116">tvRating</span><span class="sxs-lookup"><span data-stu-id="646fc-116">tvRating</span></span>|[<span data-ttu-id="646fc-117">ratingGermanyTelevisionType</span><span class="sxs-lookup"><span data-stu-id="646fc-117">ratingGermanyTelevisionType</span></span>](../resources/intune-deviceconfig-ratinggermanytelevisiontype.md)|<span data-ttu-id="646fc-118">テレビの視聴制限がドイツを選択します。</span><span class="sxs-lookup"><span data-stu-id="646fc-118">TV rating selected for Germany.</span></span> <span data-ttu-id="646fc-119">可能な値は、`allAllowed`、`allBlocked`、`general`、`agesAbove6`、`agesAbove12`、`agesAbove16`、`adults` です。</span><span class="sxs-lookup"><span data-stu-id="646fc-119">Possible values are: `allAllowed`, `allBlocked`, `general`, `agesAbove6`, `agesAbove12`, `agesAbove16`, `adults`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="646fc-120">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="646fc-120">Relationships</span></span>
<span data-ttu-id="646fc-121">なし</span><span class="sxs-lookup"><span data-stu-id="646fc-121">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="646fc-122">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="646fc-122">JSON Representation</span></span>
<span data-ttu-id="646fc-123">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="646fc-123">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.mediaContentRatingGermany"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.mediaContentRatingGermany",
  "movieRating": "String",
  "tvRating": "String"
}
```





