---
title: teamFunSettings リソースの種類
description: Giphy、memes、およびチームのステッカーを構成する設定を使用します。
localization_priority: Normal
author: nkramer
ms.prod: microsoft-teams
ms.openlocfilehash: b4c30afb6d0c10e8f011b779cf257a1627ff7b48
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/12/2019
ms.locfileid: "27949781"
---
# <a name="teamfunsettings-resource-type"></a><span data-ttu-id="444ad-103">teamFunSettings リソースの種類</span><span class="sxs-lookup"><span data-stu-id="444ad-103">teamFunSettings resource type</span></span>

> <span data-ttu-id="444ad-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="444ad-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="444ad-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="444ad-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="444ad-106">Giphy、memes、および[チーム](team.md)のステッカーを構成する設定を使用します。</span><span class="sxs-lookup"><span data-stu-id="444ad-106">Settings to configure use of Giphy, memes, and stickers in the [team](team.md).</span></span>

## <a name="properties"></a><span data-ttu-id="444ad-107">プロパティ</span><span class="sxs-lookup"><span data-stu-id="444ad-107">Properties</span></span>
| <span data-ttu-id="444ad-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="444ad-108">Property</span></span>     | <span data-ttu-id="444ad-109">種類</span><span class="sxs-lookup"><span data-stu-id="444ad-109">Type</span></span>   |<span data-ttu-id="444ad-110">説明</span><span class="sxs-lookup"><span data-stu-id="444ad-110">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="444ad-111">allowGiphy</span><span class="sxs-lookup"><span data-stu-id="444ad-111">allowGiphy</span></span>|<span data-ttu-id="444ad-112">ブール型</span><span class="sxs-lookup"><span data-stu-id="444ad-112">Boolean</span></span>|<span data-ttu-id="444ad-113">場合 true の場合、有効にする Giphy の使用を設定します。</span><span class="sxs-lookup"><span data-stu-id="444ad-113">If set to true, enables Giphy use.</span></span>|
|<span data-ttu-id="444ad-114">giphyContentRating</span><span class="sxs-lookup"><span data-stu-id="444ad-114">giphyContentRating</span></span>|<span data-ttu-id="444ad-115">文字列 (列挙型)</span><span class="sxs-lookup"><span data-stu-id="444ad-115">String (enum)</span></span>|<span data-ttu-id="444ad-116">コンテンツの規制を Giphy。</span><span class="sxs-lookup"><span data-stu-id="444ad-116">Giphy content rating.</span></span> <span data-ttu-id="444ad-117">使用可能な値は、`moderate`、`strict` です。</span><span class="sxs-lookup"><span data-stu-id="444ad-117">Possible values are: `moderate`, `strict`.</span></span>|
|<span data-ttu-id="444ad-118">allowStickersAndMemes</span><span class="sxs-lookup"><span data-stu-id="444ad-118">allowStickersAndMemes</span></span>|<span data-ttu-id="444ad-119">ブール型</span><span class="sxs-lookup"><span data-stu-id="444ad-119">Boolean</span></span>|<span data-ttu-id="444ad-120">場合は true、ステッカー、memes など、ユーザーに設定します。</span><span class="sxs-lookup"><span data-stu-id="444ad-120">If set to true, enables users to include stickers and memes.</span></span>|
|<span data-ttu-id="444ad-121">allowCustomMemes</span><span class="sxs-lookup"><span data-stu-id="444ad-121">allowCustomMemes</span></span>|<span data-ttu-id="444ad-122">ブール型</span><span class="sxs-lookup"><span data-stu-id="444ad-122">Boolean</span></span>|<span data-ttu-id="444ad-123">場合に true を設定する、カスタムの memes を含むようにユーザーをできるようにする設定です。</span><span class="sxs-lookup"><span data-stu-id="444ad-123">If set to true, enables users to include custom memes.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="444ad-124">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="444ad-124">JSON representation</span></span>

<span data-ttu-id="444ad-125">リソースの JSON 表記を次に示します。</span><span class="sxs-lookup"><span data-stu-id="444ad-125">The following is a JSON representation of the resource.</span></span>

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
