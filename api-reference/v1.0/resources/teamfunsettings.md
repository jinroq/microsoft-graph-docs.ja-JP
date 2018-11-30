---
title: teamFunSettings リソースの種類
description: Giphy、memes、およびチームのステッカーを構成する設定を使用します。
ms.openlocfilehash: ef816d027f015155cc09195c359523c83589725e
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27020602"
---
# <a name="teamfunsettings-resource-type"></a><span data-ttu-id="46b25-103">teamFunSettings リソースの種類</span><span class="sxs-lookup"><span data-stu-id="46b25-103">teamFunSettings resource type</span></span>



<span data-ttu-id="46b25-104">Giphy、memes、および[チーム](team.md)のステッカーを構成する設定を使用します。</span><span class="sxs-lookup"><span data-stu-id="46b25-104">Settings to configure use of Giphy, memes, and stickers in the [team](team.md).</span></span>

## <a name="properties"></a><span data-ttu-id="46b25-105">プロパティ</span><span class="sxs-lookup"><span data-stu-id="46b25-105">Properties</span></span>
| <span data-ttu-id="46b25-106">プロパティ</span><span class="sxs-lookup"><span data-stu-id="46b25-106">Property</span></span>     | <span data-ttu-id="46b25-107">型</span><span class="sxs-lookup"><span data-stu-id="46b25-107">Type</span></span>   |<span data-ttu-id="46b25-108">説明</span><span class="sxs-lookup"><span data-stu-id="46b25-108">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="46b25-109">allowGiphy</span><span class="sxs-lookup"><span data-stu-id="46b25-109">allowGiphy</span></span>|<span data-ttu-id="46b25-110">ブール値</span><span class="sxs-lookup"><span data-stu-id="46b25-110">Boolean</span></span>|<span data-ttu-id="46b25-111">場合 true の場合、有効にする Giphy の使用を設定します。</span><span class="sxs-lookup"><span data-stu-id="46b25-111">If set to true, enables Giphy use.</span></span>|
|<span data-ttu-id="46b25-112">giphyContentRating</span><span class="sxs-lookup"><span data-stu-id="46b25-112">giphyContentRating</span></span>|<span data-ttu-id="46b25-113">文字列 (列挙型)</span><span class="sxs-lookup"><span data-stu-id="46b25-113">String (enum)</span></span>|<span data-ttu-id="46b25-114">コンテンツの規制を Giphy。</span><span class="sxs-lookup"><span data-stu-id="46b25-114">Giphy content rating.</span></span> <span data-ttu-id="46b25-115">使用可能な値は、`moderate`、`strict` です。</span><span class="sxs-lookup"><span data-stu-id="46b25-115">Possible values are: `moderate`, `strict`.</span></span>|
|<span data-ttu-id="46b25-116">allowStickersAndMemes</span><span class="sxs-lookup"><span data-stu-id="46b25-116">allowStickersAndMemes</span></span>|<span data-ttu-id="46b25-117">ブール値</span><span class="sxs-lookup"><span data-stu-id="46b25-117">Boolean</span></span>|<span data-ttu-id="46b25-118">場合は true、ステッカー、memes など、ユーザーに設定します。</span><span class="sxs-lookup"><span data-stu-id="46b25-118">If set to true, enables users to include stickers and memes.</span></span>|
|<span data-ttu-id="46b25-119">allowCustomMemes</span><span class="sxs-lookup"><span data-stu-id="46b25-119">allowCustomMemes</span></span>|<span data-ttu-id="46b25-120">ブール値</span><span class="sxs-lookup"><span data-stu-id="46b25-120">Boolean</span></span>|<span data-ttu-id="46b25-121">場合に true を設定する、カスタムの memes を含むようにユーザーをできるようにする設定です。</span><span class="sxs-lookup"><span data-stu-id="46b25-121">If set to true, enables users to include custom memes.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="46b25-122">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="46b25-122">JSON representation</span></span>

<span data-ttu-id="46b25-123">リソースの JSON 表記を次に示します。</span><span class="sxs-lookup"><span data-stu-id="46b25-123">The following is a JSON representation of the resource.</span></span>

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
