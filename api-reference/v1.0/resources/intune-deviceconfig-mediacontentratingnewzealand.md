---
title: mediaContentRatingNewZealand リソースの種類
description: まだ文書化されていません
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 5d4a22f9510a615dab746912aed1de5123184ca3
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/11/2019
ms.locfileid: "27850548"
---
# <a name="mediacontentratingnewzealand-resource-type"></a><span data-ttu-id="38fdd-103">mediaContentRatingNewZealand リソースの種類</span><span class="sxs-lookup"><span data-stu-id="38fdd-103">mediaContentRatingNewZealand resource type</span></span>

> <span data-ttu-id="38fdd-104">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="38fdd-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="38fdd-105">まだ文書化されていません</span><span class="sxs-lookup"><span data-stu-id="38fdd-105">Not yet documented</span></span>
## <a name="properties"></a><span data-ttu-id="38fdd-106">プロパティ</span><span class="sxs-lookup"><span data-stu-id="38fdd-106">Properties</span></span>
|<span data-ttu-id="38fdd-107">プロパティ</span><span class="sxs-lookup"><span data-stu-id="38fdd-107">Property</span></span>|<span data-ttu-id="38fdd-108">種類</span><span class="sxs-lookup"><span data-stu-id="38fdd-108">Type</span></span>|<span data-ttu-id="38fdd-109">説明</span><span class="sxs-lookup"><span data-stu-id="38fdd-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="38fdd-110">movieRating</span><span class="sxs-lookup"><span data-stu-id="38fdd-110">movieRating</span></span>|[<span data-ttu-id="38fdd-111">ratingNewZealandMoviesType</span><span class="sxs-lookup"><span data-stu-id="38fdd-111">ratingNewZealandMoviesType</span></span>](../resources/intune-deviceconfig-ratingnewzealandmoviestype.md)|<span data-ttu-id="38fdd-112">評価のニュージーランドを選択したムービーです。</span><span class="sxs-lookup"><span data-stu-id="38fdd-112">Movies rating selected for New Zealand.</span></span> <span data-ttu-id="38fdd-113">可能な値は、`allAllowed`、`allBlocked`、`general`、`parentalGuidance`、`mature`、`agesAbove13`、`agesAbove15`、`agesAbove16`、`agesAbove18`、`restricted`、`agesAbove16Restricted` です。</span><span class="sxs-lookup"><span data-stu-id="38fdd-113">Possible values are: `allAllowed`, `allBlocked`, `general`, `parentalGuidance`, `mature`, `agesAbove13`, `agesAbove15`, `agesAbove16`, `agesAbove18`, `restricted`, `agesAbove16Restricted`.</span></span>|
|<span data-ttu-id="38fdd-114">tvRating</span><span class="sxs-lookup"><span data-stu-id="38fdd-114">tvRating</span></span>|[<span data-ttu-id="38fdd-115">ratingNewZealandTelevisionType</span><span class="sxs-lookup"><span data-stu-id="38fdd-115">ratingNewZealandTelevisionType</span></span>](../resources/intune-deviceconfig-ratingnewzealandtelevisiontype.md)|<span data-ttu-id="38fdd-116">テレビの視聴制限がニュージーランドを選択します。</span><span class="sxs-lookup"><span data-stu-id="38fdd-116">TV rating selected for New Zealand.</span></span> <span data-ttu-id="38fdd-117">可能な値は、`allAllowed`、`allBlocked`、`general`、`parentalGuidance`、`adults` です。</span><span class="sxs-lookup"><span data-stu-id="38fdd-117">Possible values are: `allAllowed`, `allBlocked`, `general`, `parentalGuidance`, `adults`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="38fdd-118">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="38fdd-118">Relationships</span></span>
<span data-ttu-id="38fdd-119">なし</span><span class="sxs-lookup"><span data-stu-id="38fdd-119">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="38fdd-120">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="38fdd-120">JSON Representation</span></span>
<span data-ttu-id="38fdd-121">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="38fdd-121">Here is a JSON representation of the resource.</span></span>
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



