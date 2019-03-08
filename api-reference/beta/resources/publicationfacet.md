---
author: JeremyKelley
ms.author: JeremyKelley
ms.date: 09/10/2017
title: PublicationFacet
localization_priority: Normal
ms.openlocfilehash: 66e12c3240d1cade57d377e43403b33102fe166e
ms.sourcegitcommit: b877a8dc9aeaf74f975ca495b401ffff001d7699
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 03/08/2019
ms.locfileid: "30482064"
---
# <a name="publicationfacet-resource-type"></a><span data-ttu-id="e1d72-102">PublicationFacet リソースの種類</span><span class="sxs-lookup"><span data-stu-id="e1d72-102">PublicationFacet resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="e1d72-103">\*\*publicationFacet \*\*リソースは、[driveItemVersion](driveitemversion.md) または [driveItem](driveitem.md) リソースの公開ステータスの詳細情報を提供します。</span><span class="sxs-lookup"><span data-stu-id="e1d72-103">The **publicationFacet** resource provides details on the published status of a [driveItemVersion](driveitemversion.md) or [driveItem](driveitem.md) resource.</span></span>

## <a name="json-representation"></a><span data-ttu-id="e1d72-104">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="e1d72-104">JSON representation</span></span>

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

## <a name="properties"></a><span data-ttu-id="e1d72-105">プロパティ</span><span class="sxs-lookup"><span data-stu-id="e1d72-105">Properties</span></span>

|   <span data-ttu-id="e1d72-106">プロパティ</span><span class="sxs-lookup"><span data-stu-id="e1d72-106">Property</span></span>    |  <span data-ttu-id="e1d72-107">種類</span><span class="sxs-lookup"><span data-stu-id="e1d72-107">Type</span></span>  | <span data-ttu-id="e1d72-108">説明</span><span class="sxs-lookup"><span data-stu-id="e1d72-108">Description</span></span> |
| :------------ | :----- | :---------- |
| <span data-ttu-id="e1d72-109">**level**</span><span class="sxs-lookup"><span data-stu-id="e1d72-109">**level**</span></span>     | <span data-ttu-id="e1d72-110">String
</span><span class="sxs-lookup"><span data-stu-id="e1d72-110">String</span></span> | <span data-ttu-id="e1d72-111">このドキュメントの公開状況。</span><span class="sxs-lookup"><span data-stu-id="e1d72-111">The state of publication for this document.</span></span> <span data-ttu-id="e1d72-112">`published` または `checkout` のどちらかです。</span><span class="sxs-lookup"><span data-stu-id="e1d72-112">Either `published` or `checkout`.</span></span> <span data-ttu-id="e1d72-113">読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="e1d72-113">Read-only.</span></span>  |
| <span data-ttu-id="e1d72-114">**versionId**</span><span class="sxs-lookup"><span data-stu-id="e1d72-114">**versionId**</span></span> | <span data-ttu-id="e1d72-115">String</span><span class="sxs-lookup"><span data-stu-id="e1d72-115">String</span></span> | <span data-ttu-id="e1d72-116">現在の呼び出し元に表示されているバージョンの一意識別子です。</span><span class="sxs-lookup"><span data-stu-id="e1d72-116">The unique identifier for the version that is visible to the current caller.</span></span> <span data-ttu-id="e1d72-117">値の取得のみ可能です。</span><span class="sxs-lookup"><span data-stu-id="e1d72-117">Read-only.</span></span>  |


<!--
{
  "type": "#page.annotation",
  "description": "The photo facet provides details about the camera and settings on the camera for photos.",
  "keywords": "camera make,camera model, exposure, f-stop, iso",
  "section": "documentation",
  "tocPath": "Facets/Photo",
  "suppressions": [
    "Error: /api-reference/beta/resources/publicationfacet.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
