---
author: rgregg
ms.author: rgregg
ms.date: 09/10/2017
title: ThumbnailSet
ms.openlocfilehash: c8f8d9c2232b845c746a6a215c81194e97c0431d
ms.sourcegitcommit: 7aea7a97e36e6d146214de3a90fdbc71628aadba
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 09/28/2017
---
# <a name="thumbnailset-resource-type"></a><span data-ttu-id="b95ea-102">ThumbnailSet リソース型</span><span class="sxs-lookup"><span data-stu-id="b95ea-102">ThumbnailSet resource type</span></span>

<span data-ttu-id="b95ea-p101">**ThumbnailSet** リソースは、[サムネイル](thumbnail.md) リソースのキー付きコレクションです。DriveItem に関連付けられているサムネイルのセットを表すために使用されます。</span><span class="sxs-lookup"><span data-stu-id="b95ea-p101">The **ThumbnailSet** resource is a keyed collection of [thumbnail](thumbnail.md) resources. It is used to represent a set of thumbnails associated with a DriveItem.</span></span>

## <a name="json-representation"></a><span data-ttu-id="b95ea-105">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="b95ea-105">JSON representation</span></span>

<span data-ttu-id="b95ea-106">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="b95ea-106">Here is a JSON representation of the resource.</span></span>

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

## <a name="properties"></a><span data-ttu-id="b95ea-107">プロパティ</span><span class="sxs-lookup"><span data-stu-id="b95ea-107">Properties</span></span>

| <span data-ttu-id="b95ea-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="b95ea-108">Property</span></span> | <span data-ttu-id="b95ea-109">型</span><span class="sxs-lookup"><span data-stu-id="b95ea-109">Type</span></span>                      | <span data-ttu-id="b95ea-110">説明</span><span class="sxs-lookup"><span data-stu-id="b95ea-110">Description</span></span>                                                                       |
|:---------|:--------------------------|:----------------------------------------------------------------------------------|
| <span data-ttu-id="b95ea-111">id</span><span class="sxs-lookup"><span data-stu-id="b95ea-111">id</span></span>       | <span data-ttu-id="b95ea-112">String</span><span class="sxs-lookup"><span data-stu-id="b95ea-112">String</span></span>                    | <span data-ttu-id="b95ea-p102">アイテム内の ID。読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="b95ea-p102">The id within the item. Read-only.</span></span>                                                |
| <span data-ttu-id="b95ea-115">large</span><span class="sxs-lookup"><span data-stu-id="b95ea-115">large</span></span>    | [<span data-ttu-id="b95ea-116">Thumbnail</span><span class="sxs-lookup"><span data-stu-id="b95ea-116">Thumbnail</span></span>](thumbnail.md) | <span data-ttu-id="b95ea-117">1920 x 1920 にスケーリングされたサムネイル。</span><span class="sxs-lookup"><span data-stu-id="b95ea-117">A 1920x1920 scaled thumbnail.</span></span>                                                     |
| <span data-ttu-id="b95ea-118">medium</span><span class="sxs-lookup"><span data-stu-id="b95ea-118">medium</span></span>   | [<span data-ttu-id="b95ea-119">Thumbnail</span><span class="sxs-lookup"><span data-stu-id="b95ea-119">Thumbnail</span></span>](thumbnail.md) | <span data-ttu-id="b95ea-120">176x176 にスケーリングされたサムネイル。</span><span class="sxs-lookup"><span data-stu-id="b95ea-120">A 176x176 scaled thumbnail.</span></span>                                                       |
| <span data-ttu-id="b95ea-121">small</span><span class="sxs-lookup"><span data-stu-id="b95ea-121">small</span></span>    | [<span data-ttu-id="b95ea-122">Thumbnail</span><span class="sxs-lookup"><span data-stu-id="b95ea-122">Thumbnail</span></span>](thumbnail.md) | <span data-ttu-id="b95ea-123">48 x 48 にトリミングされたサムネイル。</span><span class="sxs-lookup"><span data-stu-id="b95ea-123">A 48x48 cropped thumbnail.</span></span>                                                        |
| <span data-ttu-id="b95ea-124">source</span><span class="sxs-lookup"><span data-stu-id="b95ea-124">source</span></span>   | [<span data-ttu-id="b95ea-125">Thumbnail</span><span class="sxs-lookup"><span data-stu-id="b95ea-125">Thumbnail</span></span>](thumbnail.md) | <span data-ttu-id="b95ea-126">カスタムのサムネイル イメージ、または他のサムネイルを生成するために使用する元のイメージ。</span><span class="sxs-lookup"><span data-stu-id="b95ea-126">A custom thumbnail image or the original image used to generate other thumbnails.</span></span> |

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "ThumbnailSet enables access to thumbnails of different sizes",
  "section": "documentation",
  "tocPath": "Resources/ThumbnailSet"
} -->
