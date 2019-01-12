---
title: mediaContentRatingNewZealand リソースの種類
description: まだ文書化されていません
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 7d6556409f0893430813d2e9dbd753f97fa76886
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/12/2019
ms.locfileid: "27932246"
---
# <a name="mediacontentratingnewzealand-resource-type"></a><span data-ttu-id="270e2-103">mediaContentRatingNewZealand リソースの種類</span><span class="sxs-lookup"><span data-stu-id="270e2-103">mediaContentRatingNewZealand resource type</span></span>

> <span data-ttu-id="270e2-104">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="270e2-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="270e2-105">まだ文書化されていません</span><span class="sxs-lookup"><span data-stu-id="270e2-105">Not yet documented</span></span>
## <a name="properties"></a><span data-ttu-id="270e2-106">プロパティ</span><span class="sxs-lookup"><span data-stu-id="270e2-106">Properties</span></span>
|<span data-ttu-id="270e2-107">プロパティ</span><span class="sxs-lookup"><span data-stu-id="270e2-107">Property</span></span>|<span data-ttu-id="270e2-108">種類</span><span class="sxs-lookup"><span data-stu-id="270e2-108">Type</span></span>|<span data-ttu-id="270e2-109">説明</span><span class="sxs-lookup"><span data-stu-id="270e2-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="270e2-110">movieRating</span><span class="sxs-lookup"><span data-stu-id="270e2-110">movieRating</span></span>|[<span data-ttu-id="270e2-111">ratingNewZealandMoviesType</span><span class="sxs-lookup"><span data-stu-id="270e2-111">ratingNewZealandMoviesType</span></span>](../resources/intune-deviceconfig-ratingnewzealandmoviestype.md)|<span data-ttu-id="270e2-112">評価のニュージーランドを選択したムービーです。</span><span class="sxs-lookup"><span data-stu-id="270e2-112">Movies rating selected for New Zealand.</span></span> <span data-ttu-id="270e2-113">可能な値は、`allAllowed`、`allBlocked`、`general`、`parentalGuidance`、`mature`、`agesAbove13`、`agesAbove15`、`agesAbove16`、`agesAbove18`、`restricted`、`agesAbove16Restricted` です。</span><span class="sxs-lookup"><span data-stu-id="270e2-113">Possible values are: `allAllowed`, `allBlocked`, `general`, `parentalGuidance`, `mature`, `agesAbove13`, `agesAbove15`, `agesAbove16`, `agesAbove18`, `restricted`, `agesAbove16Restricted`.</span></span>|
|<span data-ttu-id="270e2-114">tvRating</span><span class="sxs-lookup"><span data-stu-id="270e2-114">tvRating</span></span>|[<span data-ttu-id="270e2-115">ratingNewZealandTelevisionType</span><span class="sxs-lookup"><span data-stu-id="270e2-115">ratingNewZealandTelevisionType</span></span>](../resources/intune-deviceconfig-ratingnewzealandtelevisiontype.md)|<span data-ttu-id="270e2-116">テレビの視聴制限がニュージーランドを選択します。</span><span class="sxs-lookup"><span data-stu-id="270e2-116">TV rating selected for New Zealand.</span></span> <span data-ttu-id="270e2-117">可能な値は、`allAllowed`、`allBlocked`、`general`、`parentalGuidance`、`adults` です。</span><span class="sxs-lookup"><span data-stu-id="270e2-117">Possible values are: `allAllowed`, `allBlocked`, `general`, `parentalGuidance`, `adults`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="270e2-118">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="270e2-118">Relationships</span></span>
<span data-ttu-id="270e2-119">なし</span><span class="sxs-lookup"><span data-stu-id="270e2-119">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="270e2-120">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="270e2-120">JSON Representation</span></span>
<span data-ttu-id="270e2-121">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="270e2-121">Here is a JSON representation of the resource.</span></span>
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



