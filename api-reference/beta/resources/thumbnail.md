---
author: rgregg
ms.author: rgregg
ms.date: 09/10/2017
title: サムネイル
ms.openlocfilehash: 8e56612185028891cf380d3240c999af78ff4740
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27069980"
---
# <a name="thumbnail-resource-type"></a><span data-ttu-id="379c9-102">サムネイル リソースの種類</span><span class="sxs-lookup"><span data-stu-id="379c9-102">Thumbnail resource type</span></span>

> <span data-ttu-id="379c9-103">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="379c9-103">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="379c9-104">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="379c9-104">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="379c9-105">**サムネイル** リソースの種類は、ビットマップ表示を含む画像、ビデオ、ドキュメント、任意のアイテムのサムネイルを表します。</span><span class="sxs-lookup"><span data-stu-id="379c9-105">The **thumbnail** resource type represents a thumbnail for an image, video, document, or any item that has a bitmap representation.</span></span>

## <a name="json-representation"></a><span data-ttu-id="379c9-106">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="379c9-106">JSON representation</span></span>

<span data-ttu-id="379c9-107">以下は、**サムネイル** リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="379c9-107">Here is a JSON representation of the **thumbnail** resource.</span></span>

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

## <a name="properties"></a><span data-ttu-id="379c9-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="379c9-108">Properties</span></span>

| <span data-ttu-id="379c9-109">プロパティ</span><span class="sxs-lookup"><span data-stu-id="379c9-109">Property</span></span>     | <span data-ttu-id="379c9-110">型</span><span class="sxs-lookup"><span data-stu-id="379c9-110">Type</span></span>   | <span data-ttu-id="379c9-111">説明</span><span class="sxs-lookup"><span data-stu-id="379c9-111">Description</span></span>                                                                                                                 |
| :----------- | :----- | :-------------------------------------------------------------------------------------------------------------------------- |
| <span data-ttu-id="379c9-112">height</span><span class="sxs-lookup"><span data-stu-id="379c9-112">height</span></span>       | <span data-ttu-id="379c9-113">Int32</span><span class="sxs-lookup"><span data-stu-id="379c9-113">Int32</span></span>  | <span data-ttu-id="379c9-114">サムネイルの高さ (ピクセル単位)。</span><span class="sxs-lookup"><span data-stu-id="379c9-114">The height of the thumbnail, in pixels.</span></span>                                                                                     |
| <span data-ttu-id="379c9-115">sourceItemId</span><span class="sxs-lookup"><span data-stu-id="379c9-115">sourceItemId</span></span> | <span data-ttu-id="379c9-116">String</span><span class="sxs-lookup"><span data-stu-id="379c9-116">String</span></span> | <span data-ttu-id="379c9-p102">サムネイルを提供したアイテムの一意識別子。フォルダーのサムネイルが要求された場合にのみ利用可能です。</span><span class="sxs-lookup"><span data-stu-id="379c9-p102">The unique identifier of the item that provided the thumbnail. This is only available when a folder thumbnail is requested.</span></span> |
| <span data-ttu-id="379c9-119">url</span><span class="sxs-lookup"><span data-stu-id="379c9-119">url</span></span>          | <span data-ttu-id="379c9-120">String</span><span class="sxs-lookup"><span data-stu-id="379c9-120">String</span></span> | <span data-ttu-id="379c9-121">サムネイルのコンテンツをフェッチするために使用する URL。</span><span class="sxs-lookup"><span data-stu-id="379c9-121">The URL used to fetch the thumbnail content.</span></span>                                                                                |
| <span data-ttu-id="379c9-122">width</span><span class="sxs-lookup"><span data-stu-id="379c9-122">width</span></span>        | <span data-ttu-id="379c9-123">Int32</span><span class="sxs-lookup"><span data-stu-id="379c9-123">Int32</span></span>  | <span data-ttu-id="379c9-124">サムネイルの幅 (ピクセル単位)。</span><span class="sxs-lookup"><span data-stu-id="379c9-124">The width of the thumbnail, in pixels.</span></span>                                                                                      |

## <a name="relationships"></a><span data-ttu-id="379c9-125">関係</span><span class="sxs-lookup"><span data-stu-id="379c9-125">Relationships</span></span>

| <span data-ttu-id="379c9-126">名前</span><span class="sxs-lookup"><span data-stu-id="379c9-126">Name</span></span>    | <span data-ttu-id="379c9-127">型</span><span class="sxs-lookup"><span data-stu-id="379c9-127">Type</span></span>   | <span data-ttu-id="379c9-128">説明</span><span class="sxs-lookup"><span data-stu-id="379c9-128">Description</span></span>                           |
| :------ | :----- | :------------------------------------ |
| <span data-ttu-id="379c9-129">content</span><span class="sxs-lookup"><span data-stu-id="379c9-129">content</span></span> | <span data-ttu-id="379c9-130">Stream</span><span class="sxs-lookup"><span data-stu-id="379c9-130">Stream</span></span> | <span data-ttu-id="379c9-131">サムネイルのコンテンツ ストリーム。</span><span class="sxs-lookup"><span data-stu-id="379c9-131">The content stream for the thumbnail.</span></span> |

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Thumbnail resource represents a single thumbnail for an item.",
  "section": "documentation",
  "tocPath": "Resources/Thumbnail"
} -->
