---
title: mediaContentRatingAustralia リソースの種類
description: まだ文書化されていません
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: f7bd4e156551258d98885490fbcb9dc0cd90163e
ms.sourcegitcommit: 0a62bc5849f27a55d83efce9b3eb01b9711bbe1d
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/14/2019
ms.locfileid: "34992018"
---
# <a name="mediacontentratingaustralia-resource-type"></a><span data-ttu-id="8a56c-103">mediaContentRatingAustralia リソースの種類</span><span class="sxs-lookup"><span data-stu-id="8a56c-103">mediaContentRatingAustralia resource type</span></span>

> <span data-ttu-id="8a56c-104">**重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="8a56c-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="8a56c-105">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="8a56c-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="8a56c-106">まだ文書化されていません</span><span class="sxs-lookup"><span data-stu-id="8a56c-106">Not yet documented</span></span>

## <a name="properties"></a><span data-ttu-id="8a56c-107">プロパティ</span><span class="sxs-lookup"><span data-stu-id="8a56c-107">Properties</span></span>
|<span data-ttu-id="8a56c-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="8a56c-108">Property</span></span>|<span data-ttu-id="8a56c-109">型</span><span class="sxs-lookup"><span data-stu-id="8a56c-109">Type</span></span>|<span data-ttu-id="8a56c-110">説明</span><span class="sxs-lookup"><span data-stu-id="8a56c-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="8a56c-111">movieRating</span><span class="sxs-lookup"><span data-stu-id="8a56c-111">movieRating</span></span>|[<span data-ttu-id="8a56c-112">ratingAustraliaMoviesType</span><span class="sxs-lookup"><span data-stu-id="8a56c-112">ratingAustraliaMoviesType</span></span>](../resources/intune-deviceconfig-ratingaustraliamoviestype.md)|<span data-ttu-id="8a56c-113">オーストラリア向けに選択されている映画のレーティング。</span><span class="sxs-lookup"><span data-stu-id="8a56c-113">Movies rating selected for Australia.</span></span> <span data-ttu-id="8a56c-114">可能な値は、`allAllowed`、`allBlocked`、`general`、`parentalGuidance`、`mature`、`agesAbove15`、`agesAbove18` です。</span><span class="sxs-lookup"><span data-stu-id="8a56c-114">Possible values are: `allAllowed`, `allBlocked`, `general`, `parentalGuidance`, `mature`, `agesAbove15`, `agesAbove18`.</span></span>|
|<span data-ttu-id="8a56c-115">tvRating</span><span class="sxs-lookup"><span data-stu-id="8a56c-115">tvRating</span></span>|[<span data-ttu-id="8a56c-116">ratingAustraliaTelevisionType</span><span class="sxs-lookup"><span data-stu-id="8a56c-116">ratingAustraliaTelevisionType</span></span>](../resources/intune-deviceconfig-ratingaustraliatelevisiontype.md)|<span data-ttu-id="8a56c-117">オーストラリア向けに選択されているテレビのレーティング。</span><span class="sxs-lookup"><span data-stu-id="8a56c-117">TV rating selected for Australia.</span></span> <span data-ttu-id="8a56c-118">可能な値は、`allAllowed`、`allBlocked`、`preschoolers`、`children`、`general`、`parentalGuidance`、`mature`、`agesAbove15`、`agesAbove15AdultViolence` です。</span><span class="sxs-lookup"><span data-stu-id="8a56c-118">Possible values are: `allAllowed`, `allBlocked`, `preschoolers`, `children`, `general`, `parentalGuidance`, `mature`, `agesAbove15`, `agesAbove15AdultViolence`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="8a56c-119">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="8a56c-119">Relationships</span></span>
<span data-ttu-id="8a56c-120">なし</span><span class="sxs-lookup"><span data-stu-id="8a56c-120">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="8a56c-121">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="8a56c-121">JSON Representation</span></span>
<span data-ttu-id="8a56c-122">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="8a56c-122">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.mediaContentRatingAustralia"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.mediaContentRatingAustralia",
  "movieRating": "String",
  "tvRating": "String"
}
```





