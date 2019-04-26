---
title: teamFunSettings リソースの種類
description: チームでの Giphy、ミーム、およびステッカーの使用を構成する設定。
localization_priority: Normal
author: nkramer
ms.prod: microsoft-teams
ms.openlocfilehash: 0f96157072ac7b6de403f82822226f316c8dcd46
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/26/2019
ms.locfileid: "33341709"
---
# <a name="teamfunsettings-resource-type"></a><span data-ttu-id="860ff-103">teamFunSettings リソースの種類</span><span class="sxs-lookup"><span data-stu-id="860ff-103">teamFunSettings resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="860ff-104">[チーム](team.md)での giphy、memes、ステッカーの使用を構成するための設定。</span><span class="sxs-lookup"><span data-stu-id="860ff-104">Settings to configure use of Giphy, memes, and stickers in the [team](team.md).</span></span>

## <a name="properties"></a><span data-ttu-id="860ff-105">プロパティ</span><span class="sxs-lookup"><span data-stu-id="860ff-105">Properties</span></span>
| <span data-ttu-id="860ff-106">プロパティ</span><span class="sxs-lookup"><span data-stu-id="860ff-106">Property</span></span>     | <span data-ttu-id="860ff-107">型</span><span class="sxs-lookup"><span data-stu-id="860ff-107">Type</span></span>   |<span data-ttu-id="860ff-108">説明</span><span class="sxs-lookup"><span data-stu-id="860ff-108">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="860ff-109">allowgiphy</span><span class="sxs-lookup"><span data-stu-id="860ff-109">allowGiphy</span></span>|<span data-ttu-id="860ff-110">Boolean</span><span class="sxs-lookup"><span data-stu-id="860ff-110">Boolean</span></span>|<span data-ttu-id="860ff-111">true に設定すると、giphy の使用が有効になります。</span><span class="sxs-lookup"><span data-stu-id="860ff-111">If set to true, enables Giphy use.</span></span>|
|<span data-ttu-id="860ff-112">giphyContentRating</span><span class="sxs-lookup"><span data-stu-id="860ff-112">giphyContentRating</span></span>|<span data-ttu-id="860ff-113">String (enum)</span><span class="sxs-lookup"><span data-stu-id="860ff-113">String (enum)</span></span>|<span data-ttu-id="860ff-114">giphy コンテンツの評価。</span><span class="sxs-lookup"><span data-stu-id="860ff-114">Giphy content rating.</span></span> <span data-ttu-id="860ff-115">可能な値は、`moderate`、`strict` です。</span><span class="sxs-lookup"><span data-stu-id="860ff-115">Possible values are: `moderate`, `strict`.</span></span>|
|<span data-ttu-id="860ff-116">allowStickersAndMemes</span><span class="sxs-lookup"><span data-stu-id="860ff-116">allowStickersAndMemes</span></span>|<span data-ttu-id="860ff-117">Boolean</span><span class="sxs-lookup"><span data-stu-id="860ff-117">Boolean</span></span>|<span data-ttu-id="860ff-118">true に設定すると、ユーザーはステッカーと memes を含めることができます。</span><span class="sxs-lookup"><span data-stu-id="860ff-118">If set to true, enables users to include stickers and memes.</span></span>|
|<span data-ttu-id="860ff-119">allowcustommemes</span><span class="sxs-lookup"><span data-stu-id="860ff-119">allowCustomMemes</span></span>|<span data-ttu-id="860ff-120">Boolean</span><span class="sxs-lookup"><span data-stu-id="860ff-120">Boolean</span></span>|<span data-ttu-id="860ff-121">true に設定すると、ユーザーはカスタム memes 含めることができます。</span><span class="sxs-lookup"><span data-stu-id="860ff-121">If set to true, enables users to include custom memes.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="860ff-122">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="860ff-122">JSON representation</span></span>

<span data-ttu-id="860ff-123">リソースの JSON 表記を次に示します。</span><span class="sxs-lookup"><span data-stu-id="860ff-123">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.teamFunSettings"
}-->

```json
{
  "allowGiphy": true,
  "giphyContentRating": "strict",
  "allowStickersAndMemes": true,
  "allowCustomMemes": true
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "team's funSettings resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
