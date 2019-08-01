---
author: JeremyKelley
ms.author: JeremyKelley
ms.date: 09/10/2017
title: ThumbnailSet
localization_priority: Normal
description: ThumbnailSet リソースは、サムネイル リソースのキー付きコレクションです。
ms.prod: ''
doc_type: resourcePageType
ms.openlocfilehash: 1dbd9ec5698fd3a9aac21e2f1463ce4364946e69
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "36033629"
---
# <a name="thumbnailset-resource-type"></a><span data-ttu-id="5f3f7-103">ThumbnailSet リソースの種類</span><span class="sxs-lookup"><span data-stu-id="5f3f7-103">ThumbnailSet resource type</span></span>

<span data-ttu-id="5f3f7-p101">**ThumbnailSet** リソースは、[サムネイル](thumbnail.md) リソースのキー付きコレクションです。DriveItem に関連付けられているサムネイルのセットを表すために使用されます。</span><span class="sxs-lookup"><span data-stu-id="5f3f7-p101">The **ThumbnailSet** resource is a keyed collection of [thumbnail](thumbnail.md) resources. It is used to represent a set of thumbnails associated with a DriveItem.</span></span>

## <a name="json-representation"></a><span data-ttu-id="5f3f7-106">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="5f3f7-106">JSON representation</span></span>

<span data-ttu-id="5f3f7-107">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="5f3f7-107">Here is a JSON representation of the resource.</span></span>

<!--{
  "blockType": "resource",
  "optionalProperties": [
    "source",
    "small",
    "medium",
    "large"
  ],
  "keyProperty": "id",
  "baseType": "microsoft.graph.entity",
  "@odata.type": "microsoft.graph.thumbnailSet",
  "openType": true
}-->

```json
{
  "id": "string (identifier)",
  "large": { "@odata.type": "microsoft.graph.thumbnail" },
  "medium": { "@odata.type": "microsoft.graph.thumbnail" },
  "small": { "@odata.type": "microsoft.graph.thumbnail" },
  "source": { "@odata.type": "microsoft.graph.thumbnail" }
}
```

## <a name="properties"></a><span data-ttu-id="5f3f7-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="5f3f7-108">Properties</span></span>

| <span data-ttu-id="5f3f7-109">プロパティ</span><span class="sxs-lookup"><span data-stu-id="5f3f7-109">Property</span></span> | <span data-ttu-id="5f3f7-110">型</span><span class="sxs-lookup"><span data-stu-id="5f3f7-110">Type</span></span>                      | <span data-ttu-id="5f3f7-111">説明</span><span class="sxs-lookup"><span data-stu-id="5f3f7-111">Description</span></span>                                                                       |
|:---------|:--------------------------|:----------------------------------------------------------------------------------|
| <span data-ttu-id="5f3f7-112">id</span><span class="sxs-lookup"><span data-stu-id="5f3f7-112">id</span></span>       | <span data-ttu-id="5f3f7-113">String</span><span class="sxs-lookup"><span data-stu-id="5f3f7-113">String</span></span>                    | <span data-ttu-id="5f3f7-p102">アイテム内の ID。読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="5f3f7-p102">The id within the item. Read-only.</span></span>                                                |
| <span data-ttu-id="5f3f7-116">large</span><span class="sxs-lookup"><span data-stu-id="5f3f7-116">large</span></span>    | [<span data-ttu-id="5f3f7-117">Thumbnail</span><span class="sxs-lookup"><span data-stu-id="5f3f7-117">Thumbnail</span></span>](thumbnail.md) | <span data-ttu-id="5f3f7-118">1920 x 1920 にスケーリングされたサムネイル。</span><span class="sxs-lookup"><span data-stu-id="5f3f7-118">A 1920x1920 scaled thumbnail.</span></span>                                                     |
| <span data-ttu-id="5f3f7-119">medium</span><span class="sxs-lookup"><span data-stu-id="5f3f7-119">medium</span></span>   | [<span data-ttu-id="5f3f7-120">Thumbnail</span><span class="sxs-lookup"><span data-stu-id="5f3f7-120">Thumbnail</span></span>](thumbnail.md) | <span data-ttu-id="5f3f7-121">176x176 にスケーリングされたサムネイル。</span><span class="sxs-lookup"><span data-stu-id="5f3f7-121">A 176x176 scaled thumbnail.</span></span>                                                       |
| <span data-ttu-id="5f3f7-122">small</span><span class="sxs-lookup"><span data-stu-id="5f3f7-122">small</span></span>    | [<span data-ttu-id="5f3f7-123">Thumbnail</span><span class="sxs-lookup"><span data-stu-id="5f3f7-123">Thumbnail</span></span>](thumbnail.md) | <span data-ttu-id="5f3f7-124">48 x 48 にトリミングされたサムネイル。</span><span class="sxs-lookup"><span data-stu-id="5f3f7-124">A 48x48 cropped thumbnail.</span></span>                                                        |
| <span data-ttu-id="5f3f7-125">source</span><span class="sxs-lookup"><span data-stu-id="5f3f7-125">source</span></span>   | [<span data-ttu-id="5f3f7-126">Thumbnail</span><span class="sxs-lookup"><span data-stu-id="5f3f7-126">Thumbnail</span></span>](thumbnail.md) | <span data-ttu-id="5f3f7-127">カスタムのサムネイル イメージ、または他のサムネイルを生成するために使用する元のイメージ。</span><span class="sxs-lookup"><span data-stu-id="5f3f7-127">A custom thumbnail image or the original image used to generate other thumbnails.</span></span> |

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "ThumbnailSet enables access to thumbnails of different sizes",
  "section": "documentation",
  "tocPath": "Resources/ThumbnailSet"
} -->
