---
title: teamFunSettings リソースの種類
description: Giphy、memes、およびチームのステッカーを構成する設定を使用します。
localization_priority: Normal
author: nkramer
ms.prod: microsoft-teams
ms.openlocfilehash: dc8d4cfa05f7bc6cbda9dfbf5d113370a1981ba5
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/24/2019
ms.locfileid: "29515861"
---
# <a name="teamfunsettings-resource-type"></a><span data-ttu-id="35d58-103">teamFunSettings リソースの種類</span><span class="sxs-lookup"><span data-stu-id="35d58-103">teamFunSettings resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="35d58-104">Giphy、memes、および[チーム](team.md)のステッカーを構成する設定を使用します。</span><span class="sxs-lookup"><span data-stu-id="35d58-104">Settings to configure use of Giphy, memes, and stickers in the [team](team.md).</span></span>

## <a name="properties"></a><span data-ttu-id="35d58-105">プロパティ</span><span class="sxs-lookup"><span data-stu-id="35d58-105">Properties</span></span>
| <span data-ttu-id="35d58-106">プロパティ</span><span class="sxs-lookup"><span data-stu-id="35d58-106">Property</span></span>     | <span data-ttu-id="35d58-107">型</span><span class="sxs-lookup"><span data-stu-id="35d58-107">Type</span></span>   |<span data-ttu-id="35d58-108">説明</span><span class="sxs-lookup"><span data-stu-id="35d58-108">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="35d58-109">allowGiphy</span><span class="sxs-lookup"><span data-stu-id="35d58-109">allowGiphy</span></span>|<span data-ttu-id="35d58-110">ブール値</span><span class="sxs-lookup"><span data-stu-id="35d58-110">Boolean</span></span>|<span data-ttu-id="35d58-111">場合 true の場合、有効にする Giphy の使用を設定します。</span><span class="sxs-lookup"><span data-stu-id="35d58-111">If set to true, enables Giphy use.</span></span>|
|<span data-ttu-id="35d58-112">giphyContentRating</span><span class="sxs-lookup"><span data-stu-id="35d58-112">giphyContentRating</span></span>|<span data-ttu-id="35d58-113">文字列 (列挙型)</span><span class="sxs-lookup"><span data-stu-id="35d58-113">String (enum)</span></span>|<span data-ttu-id="35d58-114">コンテンツの規制を Giphy。</span><span class="sxs-lookup"><span data-stu-id="35d58-114">Giphy content rating.</span></span> <span data-ttu-id="35d58-115">使用可能な値は、`moderate`、`strict` です。</span><span class="sxs-lookup"><span data-stu-id="35d58-115">Possible values are: `moderate`, `strict`.</span></span>|
|<span data-ttu-id="35d58-116">allowStickersAndMemes</span><span class="sxs-lookup"><span data-stu-id="35d58-116">allowStickersAndMemes</span></span>|<span data-ttu-id="35d58-117">ブール値</span><span class="sxs-lookup"><span data-stu-id="35d58-117">Boolean</span></span>|<span data-ttu-id="35d58-118">場合は true、ステッカー、memes など、ユーザーに設定します。</span><span class="sxs-lookup"><span data-stu-id="35d58-118">If set to true, enables users to include stickers and memes.</span></span>|
|<span data-ttu-id="35d58-119">allowCustomMemes</span><span class="sxs-lookup"><span data-stu-id="35d58-119">allowCustomMemes</span></span>|<span data-ttu-id="35d58-120">ブール値</span><span class="sxs-lookup"><span data-stu-id="35d58-120">Boolean</span></span>|<span data-ttu-id="35d58-121">場合に true を設定する、カスタムの memes を含むようにユーザーをできるようにする設定です。</span><span class="sxs-lookup"><span data-stu-id="35d58-121">If set to true, enables users to include custom memes.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="35d58-122">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="35d58-122">JSON representation</span></span>

<span data-ttu-id="35d58-123">リソースの JSON 表記を次に示します。</span><span class="sxs-lookup"><span data-stu-id="35d58-123">The following is a JSON representation of the resource.</span></span>

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
  "suppressions": [
    "Error: /api-reference/beta/resources/teamfunsettings.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
