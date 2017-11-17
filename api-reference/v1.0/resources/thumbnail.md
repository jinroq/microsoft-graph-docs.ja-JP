---
author: rgregg
ms.author: rgregg
ms.date: 09/10/2017
title: "サムネイル"
ms.openlocfilehash: 065c6ae7bbd4f6aca3172afd4399f0a1b5ff3d25
ms.sourcegitcommit: 7aea7a97e36e6d146214de3a90fdbc71628aadba
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 09/28/2017
---
# <a name="thumbnail-resource-type"></a><span data-ttu-id="0dec3-102">Thumbnail リソース型</span><span class="sxs-lookup"><span data-stu-id="0dec3-102">Thumbnail resource type</span></span>

<span data-ttu-id="0dec3-103">**サムネイル** リソースの種類は、ビットマップ表示を含む画像、ビデオ、ドキュメント、任意のアイテムのサムネイルを表します。</span><span class="sxs-lookup"><span data-stu-id="0dec3-103">The **thumbnail** resource type represents a thumbnail for an image, video, document, or any item that has a bitmap representation.</span></span>

## <a name="json-representation"></a><span data-ttu-id="0dec3-104">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="0dec3-104">JSON representation</span></span>

<span data-ttu-id="0dec3-105">以下は、**サムネイル** リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="0dec3-105">Here is a JSON representation of the **thumbnail** resource.</span></span>

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

## <a name="properties"></a><span data-ttu-id="0dec3-106">プロパティ</span><span class="sxs-lookup"><span data-stu-id="0dec3-106">Properties</span></span>

| <span data-ttu-id="0dec3-107">プロパティ</span><span class="sxs-lookup"><span data-stu-id="0dec3-107">Property</span></span>     | <span data-ttu-id="0dec3-108">型</span><span class="sxs-lookup"><span data-stu-id="0dec3-108">Type</span></span>   | <span data-ttu-id="0dec3-109">説明</span><span class="sxs-lookup"><span data-stu-id="0dec3-109">Description</span></span>                                                                                                                 |
| :----------- | :----- | :-------------------------------------------------------------------------------------------------------------------------- |
| <span data-ttu-id="0dec3-110">height</span><span class="sxs-lookup"><span data-stu-id="0dec3-110">height</span></span>       | <span data-ttu-id="0dec3-111">Int32</span><span class="sxs-lookup"><span data-stu-id="0dec3-111">Int32</span></span>  | <span data-ttu-id="0dec3-112">サムネイルの高さ (ピクセル単位)。</span><span class="sxs-lookup"><span data-stu-id="0dec3-112">The height of the thumbnail, in pixels.</span></span>                                                                                     |
| <span data-ttu-id="0dec3-113">sourceItemId</span><span class="sxs-lookup"><span data-stu-id="0dec3-113">sourceItemId</span></span> | <span data-ttu-id="0dec3-114">String</span><span class="sxs-lookup"><span data-stu-id="0dec3-114">String</span></span> | <span data-ttu-id="0dec3-p101">サムネイルを提供したアイテムの一意識別子。フォルダーのサムネイルが要求された場合にのみ利用可能です。</span><span class="sxs-lookup"><span data-stu-id="0dec3-p101">The unique identifier of the item that provided the thumbnail. This is only available when a folder thumbnail is requested.</span></span> |
| <span data-ttu-id="0dec3-117">url</span><span class="sxs-lookup"><span data-stu-id="0dec3-117">url</span></span>          | <span data-ttu-id="0dec3-118">String</span><span class="sxs-lookup"><span data-stu-id="0dec3-118">String</span></span> | <span data-ttu-id="0dec3-119">サムネイルのコンテンツをフェッチするために使用する URL。</span><span class="sxs-lookup"><span data-stu-id="0dec3-119">The URL used to fetch the thumbnail content.</span></span>                                                                                |
| <span data-ttu-id="0dec3-120">width</span><span class="sxs-lookup"><span data-stu-id="0dec3-120">width</span></span>        | <span data-ttu-id="0dec3-121">Int32</span><span class="sxs-lookup"><span data-stu-id="0dec3-121">Int32</span></span>  | <span data-ttu-id="0dec3-122">サムネイルの幅 (ピクセル単位)。</span><span class="sxs-lookup"><span data-stu-id="0dec3-122">The width of the thumbnail, in pixels.</span></span>                                                                                      |

## <a name="relationships"></a><span data-ttu-id="0dec3-123">関係</span><span class="sxs-lookup"><span data-stu-id="0dec3-123">Relationships</span></span>

| <span data-ttu-id="0dec3-124">名前</span><span class="sxs-lookup"><span data-stu-id="0dec3-124">Name</span></span>    | <span data-ttu-id="0dec3-125">型</span><span class="sxs-lookup"><span data-stu-id="0dec3-125">Type</span></span>   | <span data-ttu-id="0dec3-126">説明</span><span class="sxs-lookup"><span data-stu-id="0dec3-126">Description</span></span>                           |
| :------ | :----- | :------------------------------------ |
| <span data-ttu-id="0dec3-127">content</span><span class="sxs-lookup"><span data-stu-id="0dec3-127">content</span></span> | <span data-ttu-id="0dec3-128">Stream</span><span class="sxs-lookup"><span data-stu-id="0dec3-128">Stream</span></span> | <span data-ttu-id="0dec3-129">サムネイルのコンテンツ ストリーム。</span><span class="sxs-lookup"><span data-stu-id="0dec3-129">The content stream for the thumbnail.</span></span> |

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Thumbnail resource represents a single thumbnail for an item.",
  "section": "documentation",
  "tocPath": "Resources/Thumbnail"
} -->
