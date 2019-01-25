---
author: rgregg
ms.author: rgregg
ms.date: 09/10/2017
title: SearchResult
localization_priority: Normal
ms.openlocfilehash: c50f90787627732843e152a37a469c03340aa370
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/24/2019
ms.locfileid: "29511073"
---
# <a name="searchresult-resource-type"></a><span data-ttu-id="c9c9c-102">SearchResult リソースの種類</span><span class="sxs-lookup"><span data-stu-id="c9c9c-102">SearchResult resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="c9c9c-103">**SearchResult** リソースは、アイテムが検索クエリへの応答であることを示します。</span><span class="sxs-lookup"><span data-stu-id="c9c9c-103">The **SearchResult** resource indicates than an item is the response to a search query.</span></span>

## <a name="json-representation"></a><span data-ttu-id="c9c9c-104">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="c9c9c-104">JSON representation</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [ "onClickTelemtryUrl" ],
  "@odata.type": "microsoft.graph.searchResult"
}-->

```json
{
  "onClickTelemetryUrl": "url"
}
```

## <a name="properties"></a><span data-ttu-id="c9c9c-105">プロパティ</span><span class="sxs-lookup"><span data-stu-id="c9c9c-105">Properties</span></span>

| <span data-ttu-id="c9c9c-106">プロパティ</span><span class="sxs-lookup"><span data-stu-id="c9c9c-106">Property</span></span>            | <span data-ttu-id="c9c9c-107">型</span><span class="sxs-lookup"><span data-stu-id="c9c9c-107">Type</span></span>   | <span data-ttu-id="c9c9c-108">説明</span><span class="sxs-lookup"><span data-stu-id="c9c9c-108">Description</span></span>
|:--------------------|:-------|:----------------------------------------------
| <span data-ttu-id="c9c9c-109">onClickTelemetryUrl</span><span class="sxs-lookup"><span data-stu-id="c9c9c-109">onClickTelemetryUrl</span></span> | <span data-ttu-id="c9c9c-110">String</span><span class="sxs-lookup"><span data-stu-id="c9c9c-110">String</span></span> | <span data-ttu-id="c9c9c-p101">テレメトリ情報の記録に使用できるコールバックの URL。ユーザーがより正確な結果を得るためにこのアイテムを操作する場合は、アプリケーションからこの URL に対して GET を発行する必要があります。</span><span class="sxs-lookup"><span data-stu-id="c9c9c-p101">A callback URL that can be used to record telemetry information. The application should issue a GET on this URL if the user interacts with this item to improve the quality of results.</span></span>

## <a name="remarks"></a><span data-ttu-id="c9c9c-113">注釈</span><span class="sxs-lookup"><span data-stu-id="c9c9c-113">Remarks</span></span> 

<span data-ttu-id="c9c9c-114">DriveItem のファセットの詳細については、「[DriveItem](driveitem.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="c9c9c-114">For more information about the facets on a DriveItem, see [DriveItem](driveitem.md).</span></span>

<!--
{
  "type": "#page.annotation",
  "description": "The search result facet indicates an item is from a search.",
  "keywords": "search result facet",
  "section": "documentation",
  "tocPath": "Facets/SearchResult",
  "suppressions": [
    "Error: /api-reference/beta/resources/searchresult.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
