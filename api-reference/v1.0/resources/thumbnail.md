---
author: rgregg
ms.author: rgregg
ms.date: 09/10/2017
title: サムネイル
localization_priority: Normal
ms.openlocfilehash: 9c972842515de15b726d4496f915806ca5298313
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/11/2019
ms.locfileid: "27839614"
---
# <a name="thumbnail-resource-type"></a><span data-ttu-id="5f910-102">サムネイル リソースの種類</span><span class="sxs-lookup"><span data-stu-id="5f910-102">Thumbnail resource type</span></span>

<span data-ttu-id="5f910-103">**サムネイル** リソースの種類は、ビットマップ表示を含む画像、ビデオ、ドキュメント、任意のアイテムのサムネイルを表します。</span><span class="sxs-lookup"><span data-stu-id="5f910-103">The **thumbnail** resource type represents a thumbnail for an image, video, document, or any item that has a bitmap representation.</span></span>

## <a name="json-representation"></a><span data-ttu-id="5f910-104">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="5f910-104">JSON representation</span></span>

<span data-ttu-id="5f910-105">以下は、**サムネイル** リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="5f910-105">Here is a JSON representation of the **thumbnail** resource.</span></span>

<!--{
  "blockType": "resource",
  "optionalProperties": [
    "content",
    "height",
    "width",
    "sourceItemId"
  ],
  "@odata.type": "microsoft.graph.thumbnail"
}-->

```json
{
  "height": 1024,
  "sourceItemId": "string",
  "url": "string",
  "width": 1024,
  "content": "stream"
}
```

## <a name="properties"></a><span data-ttu-id="5f910-106">プロパティ</span><span class="sxs-lookup"><span data-stu-id="5f910-106">Properties</span></span>

| <span data-ttu-id="5f910-107">プロパティ</span><span class="sxs-lookup"><span data-stu-id="5f910-107">Property</span></span>     | <span data-ttu-id="5f910-108">型</span><span class="sxs-lookup"><span data-stu-id="5f910-108">Type</span></span>   | <span data-ttu-id="5f910-109">説明</span><span class="sxs-lookup"><span data-stu-id="5f910-109">Description</span></span>
| :----------- | :----- | :----------------------------------------------------
| <span data-ttu-id="5f910-110">height</span><span class="sxs-lookup"><span data-stu-id="5f910-110">height</span></span>       | <span data-ttu-id="5f910-111">Int32</span><span class="sxs-lookup"><span data-stu-id="5f910-111">Int32</span></span>  | <span data-ttu-id="5f910-112">サムネイルの高さ (ピクセル単位)。</span><span class="sxs-lookup"><span data-stu-id="5f910-112">The height of the thumbnail, in pixels.</span></span>
| <span data-ttu-id="5f910-113">sourceItemId</span><span class="sxs-lookup"><span data-stu-id="5f910-113">sourceItemId</span></span> | <span data-ttu-id="5f910-114">String</span><span class="sxs-lookup"><span data-stu-id="5f910-114">String</span></span> | <span data-ttu-id="5f910-p101">サムネイルを提供したアイテムの一意識別子。フォルダーのサムネイルが要求された場合にのみ利用可能です。</span><span class="sxs-lookup"><span data-stu-id="5f910-p101">The unique identifier of the item that provided the thumbnail. This is only available when a folder thumbnail is requested.</span></span>
| <span data-ttu-id="5f910-117">url</span><span class="sxs-lookup"><span data-stu-id="5f910-117">url</span></span>          | <span data-ttu-id="5f910-118">String</span><span class="sxs-lookup"><span data-stu-id="5f910-118">String</span></span> | <span data-ttu-id="5f910-119">サムネイルのコンテンツをフェッチするために使用する URL。</span><span class="sxs-lookup"><span data-stu-id="5f910-119">The URL used to fetch the thumbnail content.</span></span>
| <span data-ttu-id="5f910-120">width</span><span class="sxs-lookup"><span data-stu-id="5f910-120">width</span></span>        | <span data-ttu-id="5f910-121">Int32</span><span class="sxs-lookup"><span data-stu-id="5f910-121">Int32</span></span>  | <span data-ttu-id="5f910-122">サムネイルの幅 (ピクセル単位)。</span><span class="sxs-lookup"><span data-stu-id="5f910-122">The width of the thumbnail, in pixels.</span></span>
| <span data-ttu-id="5f910-123">content</span><span class="sxs-lookup"><span data-stu-id="5f910-123">content</span></span>      | <span data-ttu-id="5f910-124">Stream</span><span class="sxs-lookup"><span data-stu-id="5f910-124">Stream</span></span> | <span data-ttu-id="5f910-125">サムネイルのコンテンツ ストリーム。</span><span class="sxs-lookup"><span data-stu-id="5f910-125">The content stream for the thumbnail.</span></span>

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Thumbnail resource represents a single thumbnail for an item.",
  "section": "documentation",
  "tocPath": "Resources/Thumbnail"
} -->
