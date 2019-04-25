---
title: teamFunSettings リソースの種類
description: チームでの Giphy、ミーム、およびステッカーの使用を構成する設定。
localization_priority: Normal
author: nkramer
ms.prod: microsoft-teams
ms.openlocfilehash: c701ffe76c82a6cb4b3586272926290f634a02d9
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32548517"
---
# <a name="teamfunsettings-resource-type"></a><span data-ttu-id="7243b-103">teamFunSettings リソースの種類</span><span class="sxs-lookup"><span data-stu-id="7243b-103">teamFunSettings resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="7243b-104">[チーム](team.md)での giphy、memes、ステッカーの使用を構成するための設定。</span><span class="sxs-lookup"><span data-stu-id="7243b-104">Settings to configure use of Giphy, memes, and stickers in the [team](team.md).</span></span>

## <a name="properties"></a><span data-ttu-id="7243b-105">プロパティ</span><span class="sxs-lookup"><span data-stu-id="7243b-105">Properties</span></span>
| <span data-ttu-id="7243b-106">プロパティ</span><span class="sxs-lookup"><span data-stu-id="7243b-106">Property</span></span>     | <span data-ttu-id="7243b-107">型</span><span class="sxs-lookup"><span data-stu-id="7243b-107">Type</span></span>   |<span data-ttu-id="7243b-108">説明</span><span class="sxs-lookup"><span data-stu-id="7243b-108">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="7243b-109">allowgiphy</span><span class="sxs-lookup"><span data-stu-id="7243b-109">allowGiphy</span></span>|<span data-ttu-id="7243b-110">ブール値</span><span class="sxs-lookup"><span data-stu-id="7243b-110">Boolean</span></span>|<span data-ttu-id="7243b-111">true に設定すると、giphy の使用が有効になります。</span><span class="sxs-lookup"><span data-stu-id="7243b-111">If set to true, enables Giphy use.</span></span>|
|<span data-ttu-id="7243b-112">giphyContentRating</span><span class="sxs-lookup"><span data-stu-id="7243b-112">giphyContentRating</span></span>|<span data-ttu-id="7243b-113">String (enum)</span><span class="sxs-lookup"><span data-stu-id="7243b-113">String (enum)</span></span>|<span data-ttu-id="7243b-114">giphy コンテンツの評価。</span><span class="sxs-lookup"><span data-stu-id="7243b-114">Giphy content rating.</span></span> <span data-ttu-id="7243b-115">可能な値は、`moderate`、`strict` です。</span><span class="sxs-lookup"><span data-stu-id="7243b-115">Possible values are: `moderate`, `strict`.</span></span>|
|<span data-ttu-id="7243b-116">allowStickersAndMemes</span><span class="sxs-lookup"><span data-stu-id="7243b-116">allowStickersAndMemes</span></span>|<span data-ttu-id="7243b-117">ブール値</span><span class="sxs-lookup"><span data-stu-id="7243b-117">Boolean</span></span>|<span data-ttu-id="7243b-118">true に設定すると、ユーザーはステッカーと memes を含めることができます。</span><span class="sxs-lookup"><span data-stu-id="7243b-118">If set to true, enables users to include stickers and memes.</span></span>|
|<span data-ttu-id="7243b-119">allowcustommemes</span><span class="sxs-lookup"><span data-stu-id="7243b-119">allowCustomMemes</span></span>|<span data-ttu-id="7243b-120">ブール値</span><span class="sxs-lookup"><span data-stu-id="7243b-120">Boolean</span></span>|<span data-ttu-id="7243b-121">true に設定すると、ユーザーはカスタム memes 含めることができます。</span><span class="sxs-lookup"><span data-stu-id="7243b-121">If set to true, enables users to include custom memes.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="7243b-122">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="7243b-122">JSON representation</span></span>

<span data-ttu-id="7243b-123">リソースの JSON 表記を次に示します。</span><span class="sxs-lookup"><span data-stu-id="7243b-123">The following is a JSON representation of the resource.</span></span>

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
