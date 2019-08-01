---
title: PublicationFacet リソースの種類
description: '**publicationFacet **リソースは、driveItemVersion または driveItem リソースの公開ステータスの詳細情報を提供します。'
localization_priority: Normal
author: ''
ms.prod: ''
doc_type: resourcePageType
ms.openlocfilehash: 5189b578d0a996ceb27014d2c5400e508e1e8a56
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "36034952"
---
# <a name="publicationfacet-resource-type"></a><span data-ttu-id="be60c-103">PublicationFacet リソースの種類</span><span class="sxs-lookup"><span data-stu-id="be60c-103">PublicationFacet resource type</span></span>

<span data-ttu-id="be60c-104">\*\*publicationFacet \*\*リソースは、[driveItemVersion](driveitemversion.md) または [driveItem](driveitem.md) リソースの公開ステータスの詳細情報を提供します。</span><span class="sxs-lookup"><span data-stu-id="be60c-104">The **publicationFacet** resource provides details on the published status of a [driveItemVersion](driveitemversion.md) or [driveItem](driveitem.md) resource.</span></span>

## <a name="json-representation"></a><span data-ttu-id="be60c-105">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="be60c-105">JSON representation</span></span>

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

## <a name="properties"></a><span data-ttu-id="be60c-106">プロパティ</span><span class="sxs-lookup"><span data-stu-id="be60c-106">Properties</span></span>

|   <span data-ttu-id="be60c-107">プロパティ</span><span class="sxs-lookup"><span data-stu-id="be60c-107">Property</span></span>    |  <span data-ttu-id="be60c-108">型</span><span class="sxs-lookup"><span data-stu-id="be60c-108">Type</span></span>  | <span data-ttu-id="be60c-109">説明</span><span class="sxs-lookup"><span data-stu-id="be60c-109">Description</span></span> |
| :------------ | :----- | :---------- |
| <span data-ttu-id="be60c-110">**level**</span><span class="sxs-lookup"><span data-stu-id="be60c-110">**level**</span></span>     | <span data-ttu-id="be60c-111">String</span><span class="sxs-lookup"><span data-stu-id="be60c-111">String</span></span> | <span data-ttu-id="be60c-112">このドキュメントの公開状況。</span><span class="sxs-lookup"><span data-stu-id="be60c-112">The state of publication for this document.</span></span> <span data-ttu-id="be60c-113">`published` または `checkout` のどちらかです。</span><span class="sxs-lookup"><span data-stu-id="be60c-113">Either `published` or `checkout`.</span></span> <span data-ttu-id="be60c-114">読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="be60c-114">Read-only.</span></span>  |
| <span data-ttu-id="be60c-115">**versionId**</span><span class="sxs-lookup"><span data-stu-id="be60c-115">**versionId**</span></span> | <span data-ttu-id="be60c-116">String</span><span class="sxs-lookup"><span data-stu-id="be60c-116">String</span></span> | <span data-ttu-id="be60c-117">現在の呼び出し元に表示されているバージョンの一意識別子です。</span><span class="sxs-lookup"><span data-stu-id="be60c-117">The unique identifier for the version that is visible to the current caller.</span></span> <span data-ttu-id="be60c-118">値の取得のみ可能です。</span><span class="sxs-lookup"><span data-stu-id="be60c-118">Read-only.</span></span>  |


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
