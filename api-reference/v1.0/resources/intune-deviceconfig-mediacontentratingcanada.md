---
title: mediaContentRatingCanada リソースの種類
description: まだ文書化されていません
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: c40691556e9a8f674256c040a98f22e6ef9d717f
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/11/2019
ms.locfileid: "27857310"
---
# <a name="mediacontentratingcanada-resource-type"></a><span data-ttu-id="6caa0-103">mediaContentRatingCanada リソースの種類</span><span class="sxs-lookup"><span data-stu-id="6caa0-103">mediaContentRatingCanada resource type</span></span>

> <span data-ttu-id="6caa0-104">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="6caa0-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="6caa0-105">まだ文書化されていません</span><span class="sxs-lookup"><span data-stu-id="6caa0-105">Not yet documented</span></span>
## <a name="properties"></a><span data-ttu-id="6caa0-106">プロパティ</span><span class="sxs-lookup"><span data-stu-id="6caa0-106">Properties</span></span>
|<span data-ttu-id="6caa0-107">プロパティ</span><span class="sxs-lookup"><span data-stu-id="6caa0-107">Property</span></span>|<span data-ttu-id="6caa0-108">種類</span><span class="sxs-lookup"><span data-stu-id="6caa0-108">Type</span></span>|<span data-ttu-id="6caa0-109">説明</span><span class="sxs-lookup"><span data-stu-id="6caa0-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="6caa0-110">movieRating</span><span class="sxs-lookup"><span data-stu-id="6caa0-110">movieRating</span></span>|[<span data-ttu-id="6caa0-111">ratingCanadaMoviesType</span><span class="sxs-lookup"><span data-stu-id="6caa0-111">ratingCanadaMoviesType</span></span>](../resources/intune-deviceconfig-ratingcanadamoviestype.md)|<span data-ttu-id="6caa0-112">評価のカナダの選択したムービーです。</span><span class="sxs-lookup"><span data-stu-id="6caa0-112">Movies rating selected for Canada.</span></span> <span data-ttu-id="6caa0-113">可能な値は、`allAllowed`、`allBlocked`、`general`、`parentalGuidance`、`agesAbove14`、`agesAbove18`、`restricted` です。</span><span class="sxs-lookup"><span data-stu-id="6caa0-113">Possible values are: `allAllowed`, `allBlocked`, `general`, `parentalGuidance`, `agesAbove14`, `agesAbove18`, `restricted`.</span></span>|
|<span data-ttu-id="6caa0-114">tvRating</span><span class="sxs-lookup"><span data-stu-id="6caa0-114">tvRating</span></span>|[<span data-ttu-id="6caa0-115">ratingCanadaTelevisionType</span><span class="sxs-lookup"><span data-stu-id="6caa0-115">ratingCanadaTelevisionType</span></span>](../resources/intune-deviceconfig-ratingcanadatelevisiontype.md)|<span data-ttu-id="6caa0-116">テレビの視聴制限がカナダを選択します。</span><span class="sxs-lookup"><span data-stu-id="6caa0-116">TV rating selected for Canada.</span></span> <span data-ttu-id="6caa0-117">可能な値は、`allAllowed`、`allBlocked`、`children`、`childrenAbove8`、`general`、`parentalGuidance`、`agesAbove14`、`agesAbove18` です。</span><span class="sxs-lookup"><span data-stu-id="6caa0-117">Possible values are: `allAllowed`, `allBlocked`, `children`, `childrenAbove8`, `general`, `parentalGuidance`, `agesAbove14`, `agesAbove18`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="6caa0-118">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="6caa0-118">Relationships</span></span>
<span data-ttu-id="6caa0-119">なし</span><span class="sxs-lookup"><span data-stu-id="6caa0-119">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="6caa0-120">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="6caa0-120">JSON Representation</span></span>
<span data-ttu-id="6caa0-121">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="6caa0-121">Here is a JSON representation of the resource.</span></span>
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



