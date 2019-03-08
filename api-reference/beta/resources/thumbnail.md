---
author: JeremyKelley
ms.author: JeremyKelley
ms.date: 09/10/2017
title: Thumbnail
localization_priority: Normal
ms.openlocfilehash: 485714109005415d4a2c98fbbf2befb50ca991d0
ms.sourcegitcommit: b877a8dc9aeaf74f975ca495b401ffff001d7699
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 03/08/2019
ms.locfileid: "30481756"
---
# <a name="thumbnail-resource-type"></a><span data-ttu-id="ce386-102">サムネイル リソースの種類</span><span class="sxs-lookup"><span data-stu-id="ce386-102">Thumbnail resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="ce386-103">**サムネイル** リソースの種類は、ビットマップ表示を含む画像、ビデオ、ドキュメント、任意のアイテムのサムネイルを表します。</span><span class="sxs-lookup"><span data-stu-id="ce386-103">The **thumbnail** resource type represents a thumbnail for an image, video, document, or any item that has a bitmap representation.</span></span>

## <a name="json-representation"></a><span data-ttu-id="ce386-104">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="ce386-104">JSON representation</span></span>

<span data-ttu-id="ce386-105">以下は、**サムネイル** リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="ce386-105">Here is a JSON representation of the **thumbnail** resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": ["content", "height", "width", "sourceItemId"],
  "@odata.type": "microsoft.graph.thumbnail"
}-->

```json
{
  "height": 1024,
  "sourceItemId": "string",
  "url": "string",
  "width": 1024,

  /* relationships */
  "content": "stream"
}
```

## <a name="properties"></a><span data-ttu-id="ce386-106">プロパティ</span><span class="sxs-lookup"><span data-stu-id="ce386-106">Properties</span></span>

| <span data-ttu-id="ce386-107">プロパティ</span><span class="sxs-lookup"><span data-stu-id="ce386-107">Property</span></span>     | <span data-ttu-id="ce386-108">種類</span><span class="sxs-lookup"><span data-stu-id="ce386-108">Type</span></span>   | <span data-ttu-id="ce386-109">説明</span><span class="sxs-lookup"><span data-stu-id="ce386-109">Description</span></span>                                                                                                                 |
| :----------- | :----- | :-------------------------------------------------------------------------------------------------------------------------- |
| <span data-ttu-id="ce386-110">height</span><span class="sxs-lookup"><span data-stu-id="ce386-110">height</span></span>       | <span data-ttu-id="ce386-111">Int32</span><span class="sxs-lookup"><span data-stu-id="ce386-111">Int32</span></span>  | <span data-ttu-id="ce386-112">サムネイルの高さ (ピクセル単位)。</span><span class="sxs-lookup"><span data-stu-id="ce386-112">The height of the thumbnail, in pixels.</span></span>                                                                                     |
| <span data-ttu-id="ce386-113">sourceItemId</span><span class="sxs-lookup"><span data-stu-id="ce386-113">sourceItemId</span></span> | <span data-ttu-id="ce386-114">String</span><span class="sxs-lookup"><span data-stu-id="ce386-114">String</span></span> | <span data-ttu-id="ce386-p101">サムネイルを提供したアイテムの一意識別子。フォルダーのサムネイルが要求された場合にのみ利用可能です。</span><span class="sxs-lookup"><span data-stu-id="ce386-p101">The unique identifier of the item that provided the thumbnail. This is only available when a folder thumbnail is requested.</span></span> |
| <span data-ttu-id="ce386-117">url</span><span class="sxs-lookup"><span data-stu-id="ce386-117">url</span></span>          | <span data-ttu-id="ce386-118">String</span><span class="sxs-lookup"><span data-stu-id="ce386-118">String</span></span> | <span data-ttu-id="ce386-119">サムネイルのコンテンツをフェッチするために使用する URL。</span><span class="sxs-lookup"><span data-stu-id="ce386-119">The URL used to fetch the thumbnail content.</span></span>                                                                                |
| <span data-ttu-id="ce386-120">width</span><span class="sxs-lookup"><span data-stu-id="ce386-120">width</span></span>        | <span data-ttu-id="ce386-121">Int32</span><span class="sxs-lookup"><span data-stu-id="ce386-121">Int32</span></span>  | <span data-ttu-id="ce386-122">サムネイルの幅 (ピクセル単位)。</span><span class="sxs-lookup"><span data-stu-id="ce386-122">The width of the thumbnail, in pixels.</span></span>                                                                                      |

## <a name="relationships"></a><span data-ttu-id="ce386-123">関係</span><span class="sxs-lookup"><span data-stu-id="ce386-123">Relationships</span></span>

| <span data-ttu-id="ce386-124">名前</span><span class="sxs-lookup"><span data-stu-id="ce386-124">Name</span></span>    | <span data-ttu-id="ce386-125">種類</span><span class="sxs-lookup"><span data-stu-id="ce386-125">Type</span></span>   | <span data-ttu-id="ce386-126">説明</span><span class="sxs-lookup"><span data-stu-id="ce386-126">Description</span></span>                           |
| :------ | :----- | :------------------------------------ |
| <span data-ttu-id="ce386-127">content</span><span class="sxs-lookup"><span data-stu-id="ce386-127">content</span></span> | <span data-ttu-id="ce386-128">Stream</span><span class="sxs-lookup"><span data-stu-id="ce386-128">Stream</span></span> | <span data-ttu-id="ce386-129">サムネイルのコンテンツ ストリーム。</span><span class="sxs-lookup"><span data-stu-id="ce386-129">The content stream for the thumbnail.</span></span> |

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Thumbnail resource represents a single thumbnail for an item.",
  "section": "documentation",
  "tocPath": "Resources/Thumbnail",
  "suppressions": [
    "Error: /api-reference/beta/resources/thumbnail.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
