---
title: mediaContentRatingCanada リソースの種類
description: まだ文書化されていません
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 430baf0e6adaf53d922dc6cf94c8640107869ec4
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/11/2019
ms.locfileid: "27879934"
---
# <a name="mediacontentratingcanada-resource-type"></a><span data-ttu-id="b05c7-103">mediaContentRatingCanada リソースの種類</span><span class="sxs-lookup"><span data-stu-id="b05c7-103">mediaContentRatingCanada resource type</span></span>

> <span data-ttu-id="b05c7-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="b05c7-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="b05c7-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="b05c7-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="b05c7-106">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="b05c7-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="b05c7-107">まだ文書化されていません</span><span class="sxs-lookup"><span data-stu-id="b05c7-107">Not yet documented</span></span>
## <a name="properties"></a><span data-ttu-id="b05c7-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="b05c7-108">Properties</span></span>
|<span data-ttu-id="b05c7-109">プロパティ</span><span class="sxs-lookup"><span data-stu-id="b05c7-109">Property</span></span>|<span data-ttu-id="b05c7-110">種類</span><span class="sxs-lookup"><span data-stu-id="b05c7-110">Type</span></span>|<span data-ttu-id="b05c7-111">説明</span><span class="sxs-lookup"><span data-stu-id="b05c7-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b05c7-112">movieRating</span><span class="sxs-lookup"><span data-stu-id="b05c7-112">movieRating</span></span>|[<span data-ttu-id="b05c7-113">ratingCanadaMoviesType</span><span class="sxs-lookup"><span data-stu-id="b05c7-113">ratingCanadaMoviesType</span></span>](../resources/intune-deviceconfig-ratingcanadamoviestype.md)|<span data-ttu-id="b05c7-114">評価のカナダの選択したムービーです。</span><span class="sxs-lookup"><span data-stu-id="b05c7-114">Movies rating selected for Canada.</span></span> <span data-ttu-id="b05c7-115">可能な値は、`allAllowed`、`allBlocked`、`general`、`parentalGuidance`、`agesAbove14`、`agesAbove18`、`restricted` です。</span><span class="sxs-lookup"><span data-stu-id="b05c7-115">Possible values are: `allAllowed`, `allBlocked`, `general`, `parentalGuidance`, `agesAbove14`, `agesAbove18`, `restricted`.</span></span>|
|<span data-ttu-id="b05c7-116">tvRating</span><span class="sxs-lookup"><span data-stu-id="b05c7-116">tvRating</span></span>|[<span data-ttu-id="b05c7-117">ratingCanadaTelevisionType</span><span class="sxs-lookup"><span data-stu-id="b05c7-117">ratingCanadaTelevisionType</span></span>](../resources/intune-deviceconfig-ratingcanadatelevisiontype.md)|<span data-ttu-id="b05c7-118">テレビの視聴制限がカナダを選択します。</span><span class="sxs-lookup"><span data-stu-id="b05c7-118">TV rating selected for Canada.</span></span> <span data-ttu-id="b05c7-119">可能な値は、`allAllowed`、`allBlocked`、`children`、`childrenAbove8`、`general`、`parentalGuidance`、`agesAbove14`、`agesAbove18` です。</span><span class="sxs-lookup"><span data-stu-id="b05c7-119">Possible values are: `allAllowed`, `allBlocked`, `children`, `childrenAbove8`, `general`, `parentalGuidance`, `agesAbove14`, `agesAbove18`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="b05c7-120">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="b05c7-120">Relationships</span></span>
<span data-ttu-id="b05c7-121">なし</span><span class="sxs-lookup"><span data-stu-id="b05c7-121">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="b05c7-122">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="b05c7-122">JSON Representation</span></span>
<span data-ttu-id="b05c7-123">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="b05c7-123">Here is a JSON representation of the resource.</span></span>
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





