---
author: rgregg
ms.author: rgregg
ms.date: 09/10/2017
title: ThumbnailSet
ms.openlocfilehash: d88e19242ea6c271e206a4c1a582fdbbfac8877b
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27067702"
---
# <a name="thumbnailset-resource-type"></a><span data-ttu-id="d89d6-102">ThumbnailSet リソースの種類</span><span class="sxs-lookup"><span data-stu-id="d89d6-102">ThumbnailSet resource type</span></span>

> <span data-ttu-id="d89d6-103">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="d89d6-103">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="d89d6-104">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="d89d6-104">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="d89d6-p102">**ThumbnailSet** リソースは、[サムネイル](thumbnail.md) リソースのキー付きコレクションです。DriveItem に関連付けられているサムネイルのセットを表すために使用されます。</span><span class="sxs-lookup"><span data-stu-id="d89d6-p102">The **ThumbnailSet** resource is a keyed collection of [thumbnail](thumbnail.md) resources. It is used to represent a set of thumbnails associated with a DriveItem.</span></span>

## <a name="json-representation"></a><span data-ttu-id="d89d6-107">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="d89d6-107">JSON representation</span></span>

<span data-ttu-id="d89d6-108">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="d89d6-108">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": ["source", "small", "medium", "large"],
  "openType": true,
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.thumbnailSet"
} -->

```json
{
  "id": "string (identifier)",
  "large": { "@odata.type": "microsoft.graph.thumbnail" },
  "medium": { "@odata.type": "microsoft.graph.thumbnail" },
  "small": { "@odata.type": "microsoft.graph.thumbnail" },
  "source": { "@odata.type": "microsoft.graph.thumbnail" }
}
```

## <a name="properties"></a><span data-ttu-id="d89d6-109">プロパティ</span><span class="sxs-lookup"><span data-stu-id="d89d6-109">Properties</span></span>

| <span data-ttu-id="d89d6-110">プロパティ</span><span class="sxs-lookup"><span data-stu-id="d89d6-110">Property</span></span> | <span data-ttu-id="d89d6-111">型</span><span class="sxs-lookup"><span data-stu-id="d89d6-111">Type</span></span>                      | <span data-ttu-id="d89d6-112">説明</span><span class="sxs-lookup"><span data-stu-id="d89d6-112">Description</span></span>                                                                       |
|:---------|:--------------------------|:----------------------------------------------------------------------------------|
| <span data-ttu-id="d89d6-113">id</span><span class="sxs-lookup"><span data-stu-id="d89d6-113">id</span></span>       | <span data-ttu-id="d89d6-114">String</span><span class="sxs-lookup"><span data-stu-id="d89d6-114">String</span></span>                    | <span data-ttu-id="d89d6-p103">アイテム内の ID。読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="d89d6-p103">The id within the item. Read-only.</span></span>                                                |
| <span data-ttu-id="d89d6-117">large</span><span class="sxs-lookup"><span data-stu-id="d89d6-117">large</span></span>    | [<span data-ttu-id="d89d6-118">Thumbnail</span><span class="sxs-lookup"><span data-stu-id="d89d6-118">Thumbnail</span></span>](thumbnail.md) | <span data-ttu-id="d89d6-119">1920 x 1920 にスケーリングされたサムネイル。</span><span class="sxs-lookup"><span data-stu-id="d89d6-119">A 1920x1920 scaled thumbnail.</span></span>                                                     |
| <span data-ttu-id="d89d6-120">medium</span><span class="sxs-lookup"><span data-stu-id="d89d6-120">medium</span></span>   | [<span data-ttu-id="d89d6-121">Thumbnail</span><span class="sxs-lookup"><span data-stu-id="d89d6-121">Thumbnail</span></span>](thumbnail.md) | <span data-ttu-id="d89d6-122">176x176 にスケーリングされたサムネイル。</span><span class="sxs-lookup"><span data-stu-id="d89d6-122">A 176x176 scaled thumbnail.</span></span>                                                       |
| <span data-ttu-id="d89d6-123">small</span><span class="sxs-lookup"><span data-stu-id="d89d6-123">small</span></span>    | [<span data-ttu-id="d89d6-124">Thumbnail</span><span class="sxs-lookup"><span data-stu-id="d89d6-124">Thumbnail</span></span>](thumbnail.md) | <span data-ttu-id="d89d6-125">48 x 48 にトリミングされたサムネイル。</span><span class="sxs-lookup"><span data-stu-id="d89d6-125">A 48x48 cropped thumbnail.</span></span>                                                        |
| <span data-ttu-id="d89d6-126">source</span><span class="sxs-lookup"><span data-stu-id="d89d6-126">source</span></span>   | [<span data-ttu-id="d89d6-127">Thumbnail</span><span class="sxs-lookup"><span data-stu-id="d89d6-127">Thumbnail</span></span>](thumbnail.md) | <span data-ttu-id="d89d6-128">カスタムのサムネイル イメージ、または他のサムネイルを生成するために使用する元のイメージ。</span><span class="sxs-lookup"><span data-stu-id="d89d6-128">A custom thumbnail image or the original image used to generate other thumbnails.</span></span> |

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "ThumbnailSet enables access to thumbnails of different sizes",
  "section": "documentation",
  "tocPath": "Resources/ThumbnailSet"
} -->
