---
title: mediaContentRatingJapan リソースの種類
description: まだ文書化されていません
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 8c4e4268857f2d76e1dcf01e047a492f80492a89
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "36031389"
---
# <a name="mediacontentratingjapan-resource-type"></a><span data-ttu-id="d8fc6-103">mediaContentRatingJapan リソースの種類</span><span class="sxs-lookup"><span data-stu-id="d8fc6-103">mediaContentRatingJapan resource type</span></span>

> <span data-ttu-id="d8fc6-104">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="d8fc6-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="d8fc6-105">まだ文書化されていません</span><span class="sxs-lookup"><span data-stu-id="d8fc6-105">Not yet documented</span></span>

## <a name="properties"></a><span data-ttu-id="d8fc6-106">プロパティ</span><span class="sxs-lookup"><span data-stu-id="d8fc6-106">Properties</span></span>
|<span data-ttu-id="d8fc6-107">プロパティ</span><span class="sxs-lookup"><span data-stu-id="d8fc6-107">Property</span></span>|<span data-ttu-id="d8fc6-108">型</span><span class="sxs-lookup"><span data-stu-id="d8fc6-108">Type</span></span>|<span data-ttu-id="d8fc6-109">説明</span><span class="sxs-lookup"><span data-stu-id="d8fc6-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d8fc6-110">movieRating</span><span class="sxs-lookup"><span data-stu-id="d8fc6-110">movieRating</span></span>|[<span data-ttu-id="d8fc6-111">ratingJapanMoviesType</span><span class="sxs-lookup"><span data-stu-id="d8fc6-111">ratingJapanMoviesType</span></span>](../resources/intune-deviceconfig-ratingjapanmoviestype.md)|<span data-ttu-id="d8fc6-112">日本向けに選択されている映画のレーティング。</span><span class="sxs-lookup"><span data-stu-id="d8fc6-112">Movies rating selected for Japan.</span></span> <span data-ttu-id="d8fc6-113">使用可能な値: `allAllowed`、`allBlocked`、`general`、`parentalGuidance`、`agesAbove15`、`agesAbove18`。</span><span class="sxs-lookup"><span data-stu-id="d8fc6-113">Possible values are: `allAllowed`, `allBlocked`, `general`, `parentalGuidance`, `agesAbove15`, `agesAbove18`.</span></span>|
|<span data-ttu-id="d8fc6-114">tvRating</span><span class="sxs-lookup"><span data-stu-id="d8fc6-114">tvRating</span></span>|[<span data-ttu-id="d8fc6-115">ratingJapanTelevisionType</span><span class="sxs-lookup"><span data-stu-id="d8fc6-115">ratingJapanTelevisionType</span></span>](../resources/intune-deviceconfig-ratingjapantelevisiontype.md)|<span data-ttu-id="d8fc6-116">日本向けに選択されているテレビのレーティング。</span><span class="sxs-lookup"><span data-stu-id="d8fc6-116">TV rating selected for Japan.</span></span> <span data-ttu-id="d8fc6-117">可能な値は、`allAllowed`、`allBlocked`、`explicitAllowed` です。</span><span class="sxs-lookup"><span data-stu-id="d8fc6-117">Possible values are: `allAllowed`, `allBlocked`, `explicitAllowed`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="d8fc6-118">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="d8fc6-118">Relationships</span></span>
<span data-ttu-id="d8fc6-119">なし</span><span class="sxs-lookup"><span data-stu-id="d8fc6-119">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="d8fc6-120">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="d8fc6-120">JSON Representation</span></span>
<span data-ttu-id="d8fc6-121">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="d8fc6-121">Here is a JSON representation of the resource.</span></span>
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



