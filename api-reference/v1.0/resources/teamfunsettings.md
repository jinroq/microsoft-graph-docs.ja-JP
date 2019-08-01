---
title: teamFunSettings リソースの種類
description: チームでの Giphy、ミーム、およびステッカーの使用を構成する設定。
localization_priority: Normal
author: nkramer
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: 7605cf55e985791f6723b88485f5a51b2636e026
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "36033874"
---
# <a name="teamfunsettings-resource-type"></a><span data-ttu-id="a2359-103">teamFunSettings リソースの種類</span><span class="sxs-lookup"><span data-stu-id="a2359-103">teamFunSettings resource type</span></span>



<span data-ttu-id="a2359-104">[チーム](team.md)での giphy、memes、ステッカーの使用を構成するための設定。</span><span class="sxs-lookup"><span data-stu-id="a2359-104">Settings to configure use of Giphy, memes, and stickers in the [team](team.md).</span></span>

## <a name="properties"></a><span data-ttu-id="a2359-105">プロパティ</span><span class="sxs-lookup"><span data-stu-id="a2359-105">Properties</span></span>
| <span data-ttu-id="a2359-106">プロパティ</span><span class="sxs-lookup"><span data-stu-id="a2359-106">Property</span></span>     | <span data-ttu-id="a2359-107">型</span><span class="sxs-lookup"><span data-stu-id="a2359-107">Type</span></span>   |<span data-ttu-id="a2359-108">説明</span><span class="sxs-lookup"><span data-stu-id="a2359-108">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="a2359-109">allowGiphy</span><span class="sxs-lookup"><span data-stu-id="a2359-109">allowGiphy</span></span>|<span data-ttu-id="a2359-110">Boolean</span><span class="sxs-lookup"><span data-stu-id="a2359-110">Boolean</span></span>|<span data-ttu-id="a2359-111">True に設定すると、Giphy の使用が有効になります。</span><span class="sxs-lookup"><span data-stu-id="a2359-111">If set to true, enables Giphy use.</span></span>|
|<span data-ttu-id="a2359-112">giphyContentRating</span><span class="sxs-lookup"><span data-stu-id="a2359-112">giphyContentRating</span></span>|<span data-ttu-id="a2359-113">String (enum)</span><span class="sxs-lookup"><span data-stu-id="a2359-113">String (enum)</span></span>|<span data-ttu-id="a2359-114">Giphy コンテンツの評価。</span><span class="sxs-lookup"><span data-stu-id="a2359-114">Giphy content rating.</span></span> <span data-ttu-id="a2359-115">可能な値は、`moderate`、`strict` です。</span><span class="sxs-lookup"><span data-stu-id="a2359-115">Possible values are: `moderate`, `strict`.</span></span>|
|<span data-ttu-id="a2359-116">allowStickersAndMemes</span><span class="sxs-lookup"><span data-stu-id="a2359-116">allowStickersAndMemes</span></span>|<span data-ttu-id="a2359-117">Boolean</span><span class="sxs-lookup"><span data-stu-id="a2359-117">Boolean</span></span>|<span data-ttu-id="a2359-118">True に設定すると、ユーザーはステッカーと memes を含めることができます。</span><span class="sxs-lookup"><span data-stu-id="a2359-118">If set to true, enables users to include stickers and memes.</span></span>|
|<span data-ttu-id="a2359-119">allowCustomMemes</span><span class="sxs-lookup"><span data-stu-id="a2359-119">allowCustomMemes</span></span>|<span data-ttu-id="a2359-120">Boolean</span><span class="sxs-lookup"><span data-stu-id="a2359-120">Boolean</span></span>|<span data-ttu-id="a2359-121">True に設定すると、ユーザーはカスタム memes 含めることができます。</span><span class="sxs-lookup"><span data-stu-id="a2359-121">If set to true, enables users to include custom memes.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="a2359-122">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="a2359-122">JSON representation</span></span>

<span data-ttu-id="a2359-123">リソースの JSON 表記を次に示します。</span><span class="sxs-lookup"><span data-stu-id="a2359-123">The following is a JSON representation of the resource.</span></span>

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
<!-- {
  "type": "#page.annotation",
  "description": "team's funSettings resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
