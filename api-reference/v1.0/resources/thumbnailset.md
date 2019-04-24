---
author: JeremyKelley
ms.author: JeremyKelley
ms.date: 09/10/2017
title: ThumbnailSet
localization_priority: Normal
ms.openlocfilehash: a9d92d84c8495b8c138c34f752700ccd0aad64fd
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32457019"
---
# <a name="thumbnailset-resource-type"></a><span data-ttu-id="95de4-102">ThumbnailSet リソースの種類</span><span class="sxs-lookup"><span data-stu-id="95de4-102">ThumbnailSet resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="95de4-p101">**ThumbnailSet** リソースは、[サムネイル](thumbnail.md) リソースのキー付きコレクションです。DriveItem に関連付けられているサムネイルのセットを表すために使用されます。</span><span class="sxs-lookup"><span data-stu-id="95de4-p101">The **ThumbnailSet** resource is a keyed collection of [thumbnail](thumbnail.md) resources. It is used to represent a set of thumbnails associated with a DriveItem.</span></span>

## <a name="json-representation"></a><span data-ttu-id="95de4-105">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="95de4-105">JSON representation</span></span>

<span data-ttu-id="95de4-106">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="95de4-106">Here is a JSON representation of the resource.</span></span>

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

## <a name="properties"></a><span data-ttu-id="95de4-107">プロパティ</span><span class="sxs-lookup"><span data-stu-id="95de4-107">Properties</span></span>

| <span data-ttu-id="95de4-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="95de4-108">Property</span></span> | <span data-ttu-id="95de4-109">型</span><span class="sxs-lookup"><span data-stu-id="95de4-109">Type</span></span>                      | <span data-ttu-id="95de4-110">説明</span><span class="sxs-lookup"><span data-stu-id="95de4-110">Description</span></span>                                                                       |
|:---------|:--------------------------|:----------------------------------------------------------------------------------|
| <span data-ttu-id="95de4-111">id</span><span class="sxs-lookup"><span data-stu-id="95de4-111">id</span></span>       | <span data-ttu-id="95de4-112">String</span><span class="sxs-lookup"><span data-stu-id="95de4-112">String</span></span>                    | <span data-ttu-id="95de4-p102">アイテム内の ID。読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="95de4-p102">The id within the item. Read-only.</span></span>                                                |
| <span data-ttu-id="95de4-115">large</span><span class="sxs-lookup"><span data-stu-id="95de4-115">large</span></span>    | [<span data-ttu-id="95de4-116">Thumbnail</span><span class="sxs-lookup"><span data-stu-id="95de4-116">Thumbnail</span></span>](thumbnail.md) | <span data-ttu-id="95de4-117">1920 x 1920 にスケーリングされたサムネイル。</span><span class="sxs-lookup"><span data-stu-id="95de4-117">A 1920x1920 scaled thumbnail.</span></span>                                                     |
| <span data-ttu-id="95de4-118">medium</span><span class="sxs-lookup"><span data-stu-id="95de4-118">medium</span></span>   | [<span data-ttu-id="95de4-119">Thumbnail</span><span class="sxs-lookup"><span data-stu-id="95de4-119">Thumbnail</span></span>](thumbnail.md) | <span data-ttu-id="95de4-120">176x176 にスケーリングされたサムネイル。</span><span class="sxs-lookup"><span data-stu-id="95de4-120">A 176x176 scaled thumbnail.</span></span>                                                       |
| <span data-ttu-id="95de4-121">small</span><span class="sxs-lookup"><span data-stu-id="95de4-121">small</span></span>    | [<span data-ttu-id="95de4-122">Thumbnail</span><span class="sxs-lookup"><span data-stu-id="95de4-122">Thumbnail</span></span>](thumbnail.md) | <span data-ttu-id="95de4-123">48 x 48 にトリミングされたサムネイル。</span><span class="sxs-lookup"><span data-stu-id="95de4-123">A 48x48 cropped thumbnail.</span></span>                                                        |
| <span data-ttu-id="95de4-124">source</span><span class="sxs-lookup"><span data-stu-id="95de4-124">source</span></span>   | [<span data-ttu-id="95de4-125">Thumbnail</span><span class="sxs-lookup"><span data-stu-id="95de4-125">Thumbnail</span></span>](thumbnail.md) | <span data-ttu-id="95de4-126">カスタムのサムネイル イメージ、または他のサムネイルを生成するために使用する元のイメージ。</span><span class="sxs-lookup"><span data-stu-id="95de4-126">A custom thumbnail image or the original image used to generate other thumbnails.</span></span> |

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "ThumbnailSet enables access to thumbnails of different sizes",
  "section": "documentation",
  "tocPath": "Resources/ThumbnailSet",
  "suppressions": [
    "Error: /api-reference/beta/resources/thumbnailset.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
