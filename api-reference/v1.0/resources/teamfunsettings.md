---
title: teamFunSettings リソースの種類
description: Giphy、memes、およびチームのステッカーを構成する設定を使用します。
localization_priority: Normal
ms.openlocfilehash: 3257e54744ef14a94a0570ae45afd271c1514bb0
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/11/2019
ms.locfileid: "27825600"
---
# <a name="teamfunsettings-resource-type"></a><span data-ttu-id="893a8-103">teamFunSettings リソースの種類</span><span class="sxs-lookup"><span data-stu-id="893a8-103">teamFunSettings resource type</span></span>



<span data-ttu-id="893a8-104">Giphy、memes、および[チーム](team.md)のステッカーを構成する設定を使用します。</span><span class="sxs-lookup"><span data-stu-id="893a8-104">Settings to configure use of Giphy, memes, and stickers in the [team](team.md).</span></span>

## <a name="properties"></a><span data-ttu-id="893a8-105">プロパティ</span><span class="sxs-lookup"><span data-stu-id="893a8-105">Properties</span></span>
| <span data-ttu-id="893a8-106">プロパティ</span><span class="sxs-lookup"><span data-stu-id="893a8-106">Property</span></span>     | <span data-ttu-id="893a8-107">種類</span><span class="sxs-lookup"><span data-stu-id="893a8-107">Type</span></span>   |<span data-ttu-id="893a8-108">説明</span><span class="sxs-lookup"><span data-stu-id="893a8-108">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="893a8-109">allowGiphy</span><span class="sxs-lookup"><span data-stu-id="893a8-109">allowGiphy</span></span>|<span data-ttu-id="893a8-110">ブール型</span><span class="sxs-lookup"><span data-stu-id="893a8-110">Boolean</span></span>|<span data-ttu-id="893a8-111">場合 true の場合、有効にする Giphy の使用を設定します。</span><span class="sxs-lookup"><span data-stu-id="893a8-111">If set to true, enables Giphy use.</span></span>|
|<span data-ttu-id="893a8-112">giphyContentRating</span><span class="sxs-lookup"><span data-stu-id="893a8-112">giphyContentRating</span></span>|<span data-ttu-id="893a8-113">文字列 (列挙型)</span><span class="sxs-lookup"><span data-stu-id="893a8-113">String (enum)</span></span>|<span data-ttu-id="893a8-114">コンテンツの規制を Giphy。</span><span class="sxs-lookup"><span data-stu-id="893a8-114">Giphy content rating.</span></span> <span data-ttu-id="893a8-115">使用可能な値は、`moderate`、`strict` です。</span><span class="sxs-lookup"><span data-stu-id="893a8-115">Possible values are: `moderate`, `strict`.</span></span>|
|<span data-ttu-id="893a8-116">allowStickersAndMemes</span><span class="sxs-lookup"><span data-stu-id="893a8-116">allowStickersAndMemes</span></span>|<span data-ttu-id="893a8-117">ブール型</span><span class="sxs-lookup"><span data-stu-id="893a8-117">Boolean</span></span>|<span data-ttu-id="893a8-118">場合は true、ステッカー、memes など、ユーザーに設定します。</span><span class="sxs-lookup"><span data-stu-id="893a8-118">If set to true, enables users to include stickers and memes.</span></span>|
|<span data-ttu-id="893a8-119">allowCustomMemes</span><span class="sxs-lookup"><span data-stu-id="893a8-119">allowCustomMemes</span></span>|<span data-ttu-id="893a8-120">ブール型</span><span class="sxs-lookup"><span data-stu-id="893a8-120">Boolean</span></span>|<span data-ttu-id="893a8-121">場合に true を設定する、カスタムの memes を含むようにユーザーをできるようにする設定です。</span><span class="sxs-lookup"><span data-stu-id="893a8-121">If set to true, enables users to include custom memes.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="893a8-122">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="893a8-122">JSON representation</span></span>

<span data-ttu-id="893a8-123">リソースの JSON 表記を次に示します。</span><span class="sxs-lookup"><span data-stu-id="893a8-123">The following is a JSON representation of the resource.</span></span>

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
