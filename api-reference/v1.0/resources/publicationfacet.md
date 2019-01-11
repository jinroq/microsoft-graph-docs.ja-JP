---
title: PublicationFacet リソースの種類
description: '**publicationFacet **リソースは、driveItemVersion または driveItem リソースの公開ステータスの詳細情報を提供します。'
localization_priority: Normal
ms.openlocfilehash: 3d722f56cf1d587483c672fb7a1b7c05abd3671b
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/11/2019
ms.locfileid: "27810529"
---
# <a name="publicationfacet-resource-type"></a><span data-ttu-id="19ad4-103">PublicationFacet リソースの種類</span><span class="sxs-lookup"><span data-stu-id="19ad4-103">PublicationFacet resource type</span></span>

<span data-ttu-id="19ad4-104">\*\*publicationFacet \*\*リソースは、[driveItemVersion](driveitemversion.md) または [driveItem](driveitem.md) リソースの公開ステータスの詳細情報を提供します。</span><span class="sxs-lookup"><span data-stu-id="19ad4-104">The **publicationFacet** resource provides details on the published status of a [driveItemVersion](driveitemversion.md) or [driveItem](driveitem.md) resource.</span></span>

## <a name="json-representation"></a><span data-ttu-id="19ad4-105">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="19ad4-105">JSON representation</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [  ],
  "@odata.type": "microsoft.graph.publicationFacet"
}-->

```json
{
  "level": "published | checkout",
  "versionId": "string"
}
```

## <a name="properties"></a><span data-ttu-id="19ad4-106">プロパティ</span><span class="sxs-lookup"><span data-stu-id="19ad4-106">Properties</span></span>

|   <span data-ttu-id="19ad4-107">プロパティ</span><span class="sxs-lookup"><span data-stu-id="19ad4-107">Property</span></span>    |  <span data-ttu-id="19ad4-108">種類</span><span class="sxs-lookup"><span data-stu-id="19ad4-108">Type</span></span>  | <span data-ttu-id="19ad4-109">説明</span><span class="sxs-lookup"><span data-stu-id="19ad4-109">Description</span></span> |
| :------------ | :----- | :---------- |
| <span data-ttu-id="19ad4-110">**level**</span><span class="sxs-lookup"><span data-stu-id="19ad4-110">**level**</span></span>     | <span data-ttu-id="19ad4-111">String</span><span class="sxs-lookup"><span data-stu-id="19ad4-111">String</span></span> | <span data-ttu-id="19ad4-112">このドキュメントの公開状況。</span><span class="sxs-lookup"><span data-stu-id="19ad4-112">The state of publication for this document.</span></span> <span data-ttu-id="19ad4-113">`published` または `checkout` のどちらかです。</span><span class="sxs-lookup"><span data-stu-id="19ad4-113">Either `published` or `checkout`.</span></span> <span data-ttu-id="19ad4-114">読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="19ad4-114">Read-only.</span></span>  |
| <span data-ttu-id="19ad4-115">**versionId**</span><span class="sxs-lookup"><span data-stu-id="19ad4-115">**versionId**</span></span> | <span data-ttu-id="19ad4-116">String</span><span class="sxs-lookup"><span data-stu-id="19ad4-116">String</span></span> | <span data-ttu-id="19ad4-117">現在の呼び出し元に表示されているバージョンの一意識別子です。</span><span class="sxs-lookup"><span data-stu-id="19ad4-117">The unique identifier for the version that is visible to the current caller.</span></span> <span data-ttu-id="19ad4-118">読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="19ad4-118">Read-only.</span></span>  |


<!-- {
  "type": "#page.annotation",
  "description": "The photo facet provides details about the camera and settings on the camera for photos.",
  "keywords": "camera make,camera model, exposure, f-stop, iso",
  "section": "documentation",
  "suppressions": [
    " Warning: /api-reference/v1.0/resources/publicationfacet.md:
      Found potential enums in resource example that weren't defined in a table:(published,checkout) are in resource, but () are in table"
  ],
  "tocPath": "Facets/Photo"
} -->
