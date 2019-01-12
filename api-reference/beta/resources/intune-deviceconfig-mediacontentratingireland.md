---
title: mediaContentRatingIreland リソースの種類
description: まだ文書化されていません
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 9516c98350c239393e735008e91d966f8c6ae7a2
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/12/2019
ms.locfileid: "27957999"
---
# <a name="mediacontentratingireland-resource-type"></a><span data-ttu-id="f0915-103">mediaContentRatingIreland リソースの種類</span><span class="sxs-lookup"><span data-stu-id="f0915-103">mediaContentRatingIreland resource type</span></span>

> <span data-ttu-id="f0915-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="f0915-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="f0915-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="f0915-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="f0915-106">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="f0915-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="f0915-107">まだ文書化されていません</span><span class="sxs-lookup"><span data-stu-id="f0915-107">Not yet documented</span></span>
## <a name="properties"></a><span data-ttu-id="f0915-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="f0915-108">Properties</span></span>
|<span data-ttu-id="f0915-109">プロパティ</span><span class="sxs-lookup"><span data-stu-id="f0915-109">Property</span></span>|<span data-ttu-id="f0915-110">種類</span><span class="sxs-lookup"><span data-stu-id="f0915-110">Type</span></span>|<span data-ttu-id="f0915-111">説明</span><span class="sxs-lookup"><span data-stu-id="f0915-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f0915-112">movieRating</span><span class="sxs-lookup"><span data-stu-id="f0915-112">movieRating</span></span>|[<span data-ttu-id="f0915-113">ratingIrelandMoviesType</span><span class="sxs-lookup"><span data-stu-id="f0915-113">ratingIrelandMoviesType</span></span>](../resources/intune-deviceconfig-ratingirelandmoviestype.md)|<span data-ttu-id="f0915-114">評価のアイルランドの選択したムービーです。</span><span class="sxs-lookup"><span data-stu-id="f0915-114">Movies rating selected for Ireland.</span></span> <span data-ttu-id="f0915-115">可能な値は、`allAllowed`、`allBlocked`、`general`、`parentalGuidance`、`agesAbove12`、`agesAbove15`、`agesAbove16`、`adults` です。</span><span class="sxs-lookup"><span data-stu-id="f0915-115">Possible values are: `allAllowed`, `allBlocked`, `general`, `parentalGuidance`, `agesAbove12`, `agesAbove15`, `agesAbove16`, `adults`.</span></span>|
|<span data-ttu-id="f0915-116">tvRating</span><span class="sxs-lookup"><span data-stu-id="f0915-116">tvRating</span></span>|[<span data-ttu-id="f0915-117">ratingIrelandTelevisionType</span><span class="sxs-lookup"><span data-stu-id="f0915-117">ratingIrelandTelevisionType</span></span>](../resources/intune-deviceconfig-ratingirelandtelevisiontype.md)|<span data-ttu-id="f0915-118">テレビの視聴制限はアイルランドのために選択します。</span><span class="sxs-lookup"><span data-stu-id="f0915-118">TV rating selected for Ireland.</span></span> <span data-ttu-id="f0915-119">可能な値は、`allAllowed`、`allBlocked`、`general`、`children`、`youngAdults`、`parentalSupervision`、`mature` です。</span><span class="sxs-lookup"><span data-stu-id="f0915-119">Possible values are: `allAllowed`, `allBlocked`, `general`, `children`, `youngAdults`, `parentalSupervision`, `mature`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="f0915-120">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="f0915-120">Relationships</span></span>
<span data-ttu-id="f0915-121">なし</span><span class="sxs-lookup"><span data-stu-id="f0915-121">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="f0915-122">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="f0915-122">JSON Representation</span></span>
<span data-ttu-id="f0915-123">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="f0915-123">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.mediaContentRatingIreland"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.mediaContentRatingIreland",
  "movieRating": "String",
  "tvRating": "String"
}
```





