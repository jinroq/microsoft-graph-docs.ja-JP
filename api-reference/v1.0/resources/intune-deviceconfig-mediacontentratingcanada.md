---
title: mediaContentRatingCanada リソースの種類
description: まだ文書化されていません
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 9b4151b810fcfbc56c652492fff9fa1f3f841189
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/12/2019
ms.locfileid: "27932183"
---
# <a name="mediacontentratingcanada-resource-type"></a><span data-ttu-id="10816-103">mediaContentRatingCanada リソースの種類</span><span class="sxs-lookup"><span data-stu-id="10816-103">mediaContentRatingCanada resource type</span></span>

> <span data-ttu-id="10816-104">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="10816-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="10816-105">まだ文書化されていません</span><span class="sxs-lookup"><span data-stu-id="10816-105">Not yet documented</span></span>
## <a name="properties"></a><span data-ttu-id="10816-106">プロパティ</span><span class="sxs-lookup"><span data-stu-id="10816-106">Properties</span></span>
|<span data-ttu-id="10816-107">プロパティ</span><span class="sxs-lookup"><span data-stu-id="10816-107">Property</span></span>|<span data-ttu-id="10816-108">型</span><span class="sxs-lookup"><span data-stu-id="10816-108">Type</span></span>|<span data-ttu-id="10816-109">説明</span><span class="sxs-lookup"><span data-stu-id="10816-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="10816-110">movieRating</span><span class="sxs-lookup"><span data-stu-id="10816-110">movieRating</span></span>|[<span data-ttu-id="10816-111">ratingCanadaMoviesType</span><span class="sxs-lookup"><span data-stu-id="10816-111">ratingCanadaMoviesType</span></span>](../resources/intune-deviceconfig-ratingcanadamoviestype.md)|<span data-ttu-id="10816-112">評価のカナダの選択したムービーです。</span><span class="sxs-lookup"><span data-stu-id="10816-112">Movies rating selected for Canada.</span></span> <span data-ttu-id="10816-113">可能な値は、`allAllowed`、`allBlocked`、`general`、`parentalGuidance`、`agesAbove14`、`agesAbove18`、`restricted` です。</span><span class="sxs-lookup"><span data-stu-id="10816-113">Possible values are: `allAllowed`, `allBlocked`, `general`, `parentalGuidance`, `agesAbove14`, `agesAbove18`, `restricted`.</span></span>|
|<span data-ttu-id="10816-114">tvRating</span><span class="sxs-lookup"><span data-stu-id="10816-114">tvRating</span></span>|[<span data-ttu-id="10816-115">ratingCanadaTelevisionType</span><span class="sxs-lookup"><span data-stu-id="10816-115">ratingCanadaTelevisionType</span></span>](../resources/intune-deviceconfig-ratingcanadatelevisiontype.md)|<span data-ttu-id="10816-116">テレビの視聴制限がカナダを選択します。</span><span class="sxs-lookup"><span data-stu-id="10816-116">TV rating selected for Canada.</span></span> <span data-ttu-id="10816-117">可能な値は、`allAllowed`、`allBlocked`、`children`、`childrenAbove8`、`general`、`parentalGuidance`、`agesAbove14`、`agesAbove18` です。</span><span class="sxs-lookup"><span data-stu-id="10816-117">Possible values are: `allAllowed`, `allBlocked`, `children`, `childrenAbove8`, `general`, `parentalGuidance`, `agesAbove14`, `agesAbove18`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="10816-118">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="10816-118">Relationships</span></span>
<span data-ttu-id="10816-119">なし</span><span class="sxs-lookup"><span data-stu-id="10816-119">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="10816-120">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="10816-120">JSON Representation</span></span>
<span data-ttu-id="10816-121">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="10816-121">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.mediaContentRatingCanada"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.mediaContentRatingCanada",
  "movieRating": "String",
  "tvRating": "String"
}
```



