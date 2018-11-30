---
title: mediaContentRatingNewZealand リソースの種類
description: まだ文書化されていません
ms.openlocfilehash: 0d34843ef7cc624b222694cc8fbe0fa7a7c1b74c
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27022009"
---
# <a name="mediacontentratingnewzealand-resource-type"></a><span data-ttu-id="cd64b-103">mediaContentRatingNewZealand リソースの種類</span><span class="sxs-lookup"><span data-stu-id="cd64b-103">mediaContentRatingNewZealand resource type</span></span>

> <span data-ttu-id="cd64b-104">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="cd64b-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="cd64b-105">まだ文書化されていません</span><span class="sxs-lookup"><span data-stu-id="cd64b-105">Not yet documented</span></span>
## <a name="properties"></a><span data-ttu-id="cd64b-106">プロパティ</span><span class="sxs-lookup"><span data-stu-id="cd64b-106">Properties</span></span>
|<span data-ttu-id="cd64b-107">プロパティ</span><span class="sxs-lookup"><span data-stu-id="cd64b-107">Property</span></span>|<span data-ttu-id="cd64b-108">型</span><span class="sxs-lookup"><span data-stu-id="cd64b-108">Type</span></span>|<span data-ttu-id="cd64b-109">説明</span><span class="sxs-lookup"><span data-stu-id="cd64b-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="cd64b-110">movieRating</span><span class="sxs-lookup"><span data-stu-id="cd64b-110">movieRating</span></span>|[<span data-ttu-id="cd64b-111">ratingNewZealandMoviesType</span><span class="sxs-lookup"><span data-stu-id="cd64b-111">ratingNewZealandMoviesType</span></span>](../resources/intune-deviceconfig-ratingnewzealandmoviestype.md)|<span data-ttu-id="cd64b-112">評価のニュージーランドを選択したムービーです。</span><span class="sxs-lookup"><span data-stu-id="cd64b-112">Movies rating selected for New Zealand.</span></span> <span data-ttu-id="cd64b-113">可能な値は、`allAllowed`、`allBlocked`、`general`、`parentalGuidance`、`mature`、`agesAbove13`、`agesAbove15`、`agesAbove16`、`agesAbove18`、`restricted`、`agesAbove16Restricted` です。</span><span class="sxs-lookup"><span data-stu-id="cd64b-113">Possible values are: `allAllowed`, `allBlocked`, `general`, `parentalGuidance`, `mature`, `agesAbove13`, `agesAbove15`, `agesAbove16`, `agesAbove18`, `restricted`, `agesAbove16Restricted`.</span></span>|
|<span data-ttu-id="cd64b-114">tvRating</span><span class="sxs-lookup"><span data-stu-id="cd64b-114">tvRating</span></span>|[<span data-ttu-id="cd64b-115">ratingNewZealandTelevisionType</span><span class="sxs-lookup"><span data-stu-id="cd64b-115">ratingNewZealandTelevisionType</span></span>](../resources/intune-deviceconfig-ratingnewzealandtelevisiontype.md)|<span data-ttu-id="cd64b-116">テレビの視聴制限がニュージーランドを選択します。</span><span class="sxs-lookup"><span data-stu-id="cd64b-116">TV rating selected for New Zealand.</span></span> <span data-ttu-id="cd64b-117">可能な値は、`allAllowed`、`allBlocked`、`general`、`parentalGuidance`、`adults` です。</span><span class="sxs-lookup"><span data-stu-id="cd64b-117">Possible values are: `allAllowed`, `allBlocked`, `general`, `parentalGuidance`, `adults`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="cd64b-118">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="cd64b-118">Relationships</span></span>
<span data-ttu-id="cd64b-119">なし</span><span class="sxs-lookup"><span data-stu-id="cd64b-119">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="cd64b-120">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="cd64b-120">JSON Representation</span></span>
<span data-ttu-id="cd64b-121">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="cd64b-121">Here is a JSON representation of the resource.</span></span>
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



