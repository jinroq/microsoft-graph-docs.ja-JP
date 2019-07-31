---
author: JeremyKelley
description: サムネイル リソースの種類は、ビットマップ表示を含む画像、ビデオ、ドキュメント、任意のアイテムのサムネイルを表します。
ms.date: 09/10/2017
title: Thumbnail
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
ms.openlocfilehash: 752d46f1c8a769f9f571fd13d940586fda653a58
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "36007663"
---
# <a name="thumbnail-resource-type"></a><span data-ttu-id="cc854-103">サムネイル リソースの種類</span><span class="sxs-lookup"><span data-stu-id="cc854-103">Thumbnail resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="cc854-104">**サムネイル** リソースの種類は、ビットマップ表示を含む画像、ビデオ、ドキュメント、任意のアイテムのサムネイルを表します。</span><span class="sxs-lookup"><span data-stu-id="cc854-104">The **thumbnail** resource type represents a thumbnail for an image, video, document, or any item that has a bitmap representation.</span></span>

## <a name="json-representation"></a><span data-ttu-id="cc854-105">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="cc854-105">JSON representation</span></span>

<span data-ttu-id="cc854-106">以下は、**サムネイル** リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="cc854-106">Here is a JSON representation of the **thumbnail** resource.</span></span>

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

## <a name="properties"></a><span data-ttu-id="cc854-107">プロパティ</span><span class="sxs-lookup"><span data-stu-id="cc854-107">Properties</span></span>

| <span data-ttu-id="cc854-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="cc854-108">Property</span></span>     | <span data-ttu-id="cc854-109">型</span><span class="sxs-lookup"><span data-stu-id="cc854-109">Type</span></span>   | <span data-ttu-id="cc854-110">説明</span><span class="sxs-lookup"><span data-stu-id="cc854-110">Description</span></span>                                                                                                                 |
| :----------- | :----- | :-------------------------------------------------------------------------------------------------------------------------- |
| <span data-ttu-id="cc854-111">height</span><span class="sxs-lookup"><span data-stu-id="cc854-111">height</span></span>       | <span data-ttu-id="cc854-112">Int32</span><span class="sxs-lookup"><span data-stu-id="cc854-112">Int32</span></span>  | <span data-ttu-id="cc854-113">サムネイルの高さ (ピクセル単位)。</span><span class="sxs-lookup"><span data-stu-id="cc854-113">The height of the thumbnail, in pixels.</span></span>                                                                                     |
| <span data-ttu-id="cc854-114">sourceItemId</span><span class="sxs-lookup"><span data-stu-id="cc854-114">sourceItemId</span></span> | <span data-ttu-id="cc854-115">String</span><span class="sxs-lookup"><span data-stu-id="cc854-115">String</span></span> | <span data-ttu-id="cc854-p101">サムネイルを提供したアイテムの一意識別子。フォルダーのサムネイルが要求された場合にのみ利用可能です。</span><span class="sxs-lookup"><span data-stu-id="cc854-p101">The unique identifier of the item that provided the thumbnail. This is only available when a folder thumbnail is requested.</span></span> |
| <span data-ttu-id="cc854-118">url</span><span class="sxs-lookup"><span data-stu-id="cc854-118">url</span></span>          | <span data-ttu-id="cc854-119">String</span><span class="sxs-lookup"><span data-stu-id="cc854-119">String</span></span> | <span data-ttu-id="cc854-120">サムネイルのコンテンツをフェッチするために使用する URL。</span><span class="sxs-lookup"><span data-stu-id="cc854-120">The URL used to fetch the thumbnail content.</span></span>                                                                                |
| <span data-ttu-id="cc854-121">width</span><span class="sxs-lookup"><span data-stu-id="cc854-121">width</span></span>        | <span data-ttu-id="cc854-122">Int32</span><span class="sxs-lookup"><span data-stu-id="cc854-122">Int32</span></span>  | <span data-ttu-id="cc854-123">サムネイルの幅 (ピクセル単位)。</span><span class="sxs-lookup"><span data-stu-id="cc854-123">The width of the thumbnail, in pixels.</span></span>                                                                                      |
| <span data-ttu-id="cc854-124">content</span><span class="sxs-lookup"><span data-stu-id="cc854-124">content</span></span> | <span data-ttu-id="cc854-125">Stream</span><span class="sxs-lookup"><span data-stu-id="cc854-125">Stream</span></span> | <span data-ttu-id="cc854-126">サムネイルのコンテンツ ストリーム。</span><span class="sxs-lookup"><span data-stu-id="cc854-126">The content stream for the thumbnail.</span></span> |


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Thumbnail resource represents a single thumbnail for an item.",
  "section": "documentation",
  "tocPath": "Resources/Thumbnail",
  "suppressions": []
}
-->
