---
author: rgregg
ms.author: rgregg
ms.date: 09/10/2017
title: サムネイル
ms.openlocfilehash: ff111f44101bb03b3d8475e2567d6e1b2b4a753d
ms.sourcegitcommit: abf4b739257e3ffd9d045f783ec595d846172590
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/21/2018
ms.locfileid: "23264974"
---
# <a name="thumbnail-resource-type"></a><span data-ttu-id="89fba-102">サムネイル リソースの種類</span><span class="sxs-lookup"><span data-stu-id="89fba-102">Thumbnail resource type</span></span>

<span data-ttu-id="89fba-103">**サムネイル** リソースの種類は、ビットマップ表示を含む画像、ビデオ、ドキュメント、任意のアイテムのサムネイルを表します。</span><span class="sxs-lookup"><span data-stu-id="89fba-103">The **thumbnail** resource type represents a thumbnail for an image, video, document, or any item that has a bitmap representation.</span></span>

## <a name="json-representation"></a><span data-ttu-id="89fba-104">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="89fba-104">JSON representation</span></span>

<span data-ttu-id="89fba-105">以下は、**サムネイル** リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="89fba-105">Here is a JSON representation of the **thumbnail** resource.</span></span>

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

## <a name="properties"></a><span data-ttu-id="89fba-106">プロパティ</span><span class="sxs-lookup"><span data-stu-id="89fba-106">Properties</span></span>

| <span data-ttu-id="89fba-107">プロパティ</span><span class="sxs-lookup"><span data-stu-id="89fba-107">Property</span></span>     | <span data-ttu-id="89fba-108">型</span><span class="sxs-lookup"><span data-stu-id="89fba-108">Type</span></span>   | <span data-ttu-id="89fba-109">説明</span><span class="sxs-lookup"><span data-stu-id="89fba-109">Description</span></span>
| :----------- | :----- | :----------------------------------------------------
| <span data-ttu-id="89fba-110">高さ</span><span class="sxs-lookup"><span data-stu-id="89fba-110">height</span></span>       | <span data-ttu-id="89fba-111">Int32</span><span class="sxs-lookup"><span data-stu-id="89fba-111">Int32</span></span>  | <span data-ttu-id="89fba-112">サムネイルの高さ (ピクセル単位)。</span><span class="sxs-lookup"><span data-stu-id="89fba-112">The height of the thumbnail, in pixels.</span></span>
| <span data-ttu-id="89fba-113">sourceItemId</span><span class="sxs-lookup"><span data-stu-id="89fba-113">sourceItemId</span></span> | <span data-ttu-id="89fba-114">文字列</span><span class="sxs-lookup"><span data-stu-id="89fba-114">String</span></span> | <span data-ttu-id="89fba-p101">サムネイルを提供したアイテムの一意識別子。フォルダーのサムネイルが要求された場合にのみ利用可能です。</span><span class="sxs-lookup"><span data-stu-id="89fba-p101">The unique identifier of the item that provided the thumbnail. This is only available when a folder thumbnail is requested.</span></span>
| <span data-ttu-id="89fba-117">url</span><span class="sxs-lookup"><span data-stu-id="89fba-117">url</span></span>          | <span data-ttu-id="89fba-118">文字列</span><span class="sxs-lookup"><span data-stu-id="89fba-118">String</span></span> | <span data-ttu-id="89fba-119">サムネイルのコンテンツをフェッチするために使用する URL。</span><span class="sxs-lookup"><span data-stu-id="89fba-119">The URL used to fetch the thumbnail content.</span></span>
| <span data-ttu-id="89fba-120">width</span><span class="sxs-lookup"><span data-stu-id="89fba-120">width</span></span>        | <span data-ttu-id="89fba-121">Int32</span><span class="sxs-lookup"><span data-stu-id="89fba-121">Int32</span></span>  | <span data-ttu-id="89fba-122">サムネイルの幅 (ピクセル単位)。</span><span class="sxs-lookup"><span data-stu-id="89fba-122">The width of the thumbnail, in pixels.</span></span>
| <span data-ttu-id="89fba-123">コンテンツ</span><span class="sxs-lookup"><span data-stu-id="89fba-123">content</span></span>      | <span data-ttu-id="89fba-124">ストリーム</span><span class="sxs-lookup"><span data-stu-id="89fba-124">Stream</span></span> | <span data-ttu-id="89fba-125">サムネイルのコンテンツ ストリーム。</span><span class="sxs-lookup"><span data-stu-id="89fba-125">The content stream for the thumbnail.</span></span>

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Thumbnail resource represents a single thumbnail for an item.",
  "section": "documentation",
  "tocPath": "Resources/Thumbnail"
} -->
