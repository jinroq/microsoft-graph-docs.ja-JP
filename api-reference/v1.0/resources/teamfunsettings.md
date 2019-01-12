---
title: teamFunSettings リソースの種類
description: Giphy、memes、およびチームのステッカーを構成する設定を使用します。
localization_priority: Normal
author: nkramer
ms.prod: microsoft-teams
ms.openlocfilehash: c701ffe76c82a6cb4b3586272926290f634a02d9
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/12/2019
ms.locfileid: "27987672"
---
# <a name="teamfunsettings-resource-type"></a><span data-ttu-id="7bfd1-103">teamFunSettings リソースの種類</span><span class="sxs-lookup"><span data-stu-id="7bfd1-103">teamFunSettings resource type</span></span>



<span data-ttu-id="7bfd1-104">Giphy、memes、および[チーム](team.md)のステッカーを構成する設定を使用します。</span><span class="sxs-lookup"><span data-stu-id="7bfd1-104">Settings to configure use of Giphy, memes, and stickers in the [team](team.md).</span></span>

## <a name="properties"></a><span data-ttu-id="7bfd1-105">プロパティ</span><span class="sxs-lookup"><span data-stu-id="7bfd1-105">Properties</span></span>
| <span data-ttu-id="7bfd1-106">プロパティ</span><span class="sxs-lookup"><span data-stu-id="7bfd1-106">Property</span></span>     | <span data-ttu-id="7bfd1-107">種類</span><span class="sxs-lookup"><span data-stu-id="7bfd1-107">Type</span></span>   |<span data-ttu-id="7bfd1-108">説明</span><span class="sxs-lookup"><span data-stu-id="7bfd1-108">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="7bfd1-109">allowGiphy</span><span class="sxs-lookup"><span data-stu-id="7bfd1-109">allowGiphy</span></span>|<span data-ttu-id="7bfd1-110">ブール型</span><span class="sxs-lookup"><span data-stu-id="7bfd1-110">Boolean</span></span>|<span data-ttu-id="7bfd1-111">場合 true の場合、有効にする Giphy の使用を設定します。</span><span class="sxs-lookup"><span data-stu-id="7bfd1-111">If set to true, enables Giphy use.</span></span>|
|<span data-ttu-id="7bfd1-112">giphyContentRating</span><span class="sxs-lookup"><span data-stu-id="7bfd1-112">giphyContentRating</span></span>|<span data-ttu-id="7bfd1-113">文字列 (列挙型)</span><span class="sxs-lookup"><span data-stu-id="7bfd1-113">String (enum)</span></span>|<span data-ttu-id="7bfd1-114">コンテンツの規制を Giphy。</span><span class="sxs-lookup"><span data-stu-id="7bfd1-114">Giphy content rating.</span></span> <span data-ttu-id="7bfd1-115">使用可能な値は、`moderate`、`strict` です。</span><span class="sxs-lookup"><span data-stu-id="7bfd1-115">Possible values are: `moderate`, `strict`.</span></span>|
|<span data-ttu-id="7bfd1-116">allowStickersAndMemes</span><span class="sxs-lookup"><span data-stu-id="7bfd1-116">allowStickersAndMemes</span></span>|<span data-ttu-id="7bfd1-117">ブール型</span><span class="sxs-lookup"><span data-stu-id="7bfd1-117">Boolean</span></span>|<span data-ttu-id="7bfd1-118">場合は true、ステッカー、memes など、ユーザーに設定します。</span><span class="sxs-lookup"><span data-stu-id="7bfd1-118">If set to true, enables users to include stickers and memes.</span></span>|
|<span data-ttu-id="7bfd1-119">allowCustomMemes</span><span class="sxs-lookup"><span data-stu-id="7bfd1-119">allowCustomMemes</span></span>|<span data-ttu-id="7bfd1-120">ブール型</span><span class="sxs-lookup"><span data-stu-id="7bfd1-120">Boolean</span></span>|<span data-ttu-id="7bfd1-121">場合に true を設定する、カスタムの memes を含むようにユーザーをできるようにする設定です。</span><span class="sxs-lookup"><span data-stu-id="7bfd1-121">If set to true, enables users to include custom memes.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="7bfd1-122">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="7bfd1-122">JSON representation</span></span>

<span data-ttu-id="7bfd1-123">リソースの JSON 表記を次に示します。</span><span class="sxs-lookup"><span data-stu-id="7bfd1-123">The following is a JSON representation of the resource.</span></span>

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
