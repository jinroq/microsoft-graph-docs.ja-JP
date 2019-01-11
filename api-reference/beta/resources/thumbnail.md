---
author: rgregg
ms.author: rgregg
ms.date: 09/10/2017
title: サムネイル
localization_priority: Normal
ms.openlocfilehash: 22602d534c3fd1f308a5e2bb67992bd76086c4fe
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/11/2019
ms.locfileid: "27863225"
---
# <a name="thumbnail-resource-type"></a><span data-ttu-id="40049-102">サムネイル リソースの種類</span><span class="sxs-lookup"><span data-stu-id="40049-102">Thumbnail resource type</span></span>

> <span data-ttu-id="40049-103">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="40049-103">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="40049-104">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="40049-104">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="40049-105">**サムネイル** リソースの種類は、ビットマップ表示を含む画像、ビデオ、ドキュメント、任意のアイテムのサムネイルを表します。</span><span class="sxs-lookup"><span data-stu-id="40049-105">The **thumbnail** resource type represents a thumbnail for an image, video, document, or any item that has a bitmap representation.</span></span>

## <a name="json-representation"></a><span data-ttu-id="40049-106">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="40049-106">JSON representation</span></span>

<span data-ttu-id="40049-107">以下は、**サムネイル** リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="40049-107">Here is a JSON representation of the **thumbnail** resource.</span></span>

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

## <a name="properties"></a><span data-ttu-id="40049-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="40049-108">Properties</span></span>

| <span data-ttu-id="40049-109">プロパティ</span><span class="sxs-lookup"><span data-stu-id="40049-109">Property</span></span>     | <span data-ttu-id="40049-110">種類</span><span class="sxs-lookup"><span data-stu-id="40049-110">Type</span></span>   | <span data-ttu-id="40049-111">説明</span><span class="sxs-lookup"><span data-stu-id="40049-111">Description</span></span>                                                                                                                 |
| :----------- | :----- | :-------------------------------------------------------------------------------------------------------------------------- |
| <span data-ttu-id="40049-112">height</span><span class="sxs-lookup"><span data-stu-id="40049-112">height</span></span>       | <span data-ttu-id="40049-113">Int32</span><span class="sxs-lookup"><span data-stu-id="40049-113">Int32</span></span>  | <span data-ttu-id="40049-114">サムネイルの高さ (ピクセル単位)。</span><span class="sxs-lookup"><span data-stu-id="40049-114">The height of the thumbnail, in pixels.</span></span>                                                                                     |
| <span data-ttu-id="40049-115">sourceItemId</span><span class="sxs-lookup"><span data-stu-id="40049-115">sourceItemId</span></span> | <span data-ttu-id="40049-116">String</span><span class="sxs-lookup"><span data-stu-id="40049-116">String</span></span> | <span data-ttu-id="40049-p102">サムネイルを提供したアイテムの一意識別子。フォルダーのサムネイルが要求された場合にのみ利用可能です。</span><span class="sxs-lookup"><span data-stu-id="40049-p102">The unique identifier of the item that provided the thumbnail. This is only available when a folder thumbnail is requested.</span></span> |
| <span data-ttu-id="40049-119">url</span><span class="sxs-lookup"><span data-stu-id="40049-119">url</span></span>          | <span data-ttu-id="40049-120">String</span><span class="sxs-lookup"><span data-stu-id="40049-120">String</span></span> | <span data-ttu-id="40049-121">サムネイルのコンテンツをフェッチするために使用する URL。</span><span class="sxs-lookup"><span data-stu-id="40049-121">The URL used to fetch the thumbnail content.</span></span>                                                                                |
| <span data-ttu-id="40049-122">width</span><span class="sxs-lookup"><span data-stu-id="40049-122">width</span></span>        | <span data-ttu-id="40049-123">Int32</span><span class="sxs-lookup"><span data-stu-id="40049-123">Int32</span></span>  | <span data-ttu-id="40049-124">サムネイルの幅 (ピクセル単位)。</span><span class="sxs-lookup"><span data-stu-id="40049-124">The width of the thumbnail, in pixels.</span></span>                                                                                      |

## <a name="relationships"></a><span data-ttu-id="40049-125">関係</span><span class="sxs-lookup"><span data-stu-id="40049-125">Relationships</span></span>

| <span data-ttu-id="40049-126">名前</span><span class="sxs-lookup"><span data-stu-id="40049-126">Name</span></span>    | <span data-ttu-id="40049-127">種類</span><span class="sxs-lookup"><span data-stu-id="40049-127">Type</span></span>   | <span data-ttu-id="40049-128">説明</span><span class="sxs-lookup"><span data-stu-id="40049-128">Description</span></span>                           |
| :------ | :----- | :------------------------------------ |
| <span data-ttu-id="40049-129">content</span><span class="sxs-lookup"><span data-stu-id="40049-129">content</span></span> | <span data-ttu-id="40049-130">Stream</span><span class="sxs-lookup"><span data-stu-id="40049-130">Stream</span></span> | <span data-ttu-id="40049-131">サムネイルのコンテンツ ストリーム。</span><span class="sxs-lookup"><span data-stu-id="40049-131">The content stream for the thumbnail.</span></span> |

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Thumbnail resource represents a single thumbnail for an item.",
  "section": "documentation",
  "tocPath": "Resources/Thumbnail"
} -->
