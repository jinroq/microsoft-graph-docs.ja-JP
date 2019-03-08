---
author: JeremyKelley
ms.author: JeremyKelley
ms.date: 09/10/2017
title: searchresult.xml
localization_priority: Normal
ms.openlocfilehash: ee6825860f5c1ed82c368b53eb3510175e7d3a11
ms.sourcegitcommit: b877a8dc9aeaf74f975ca495b401ffff001d7699
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 03/08/2019
ms.locfileid: "30481231"
---
# <a name="searchresult-resource-type"></a><span data-ttu-id="7d93f-102">SearchResult リソースの種類</span><span class="sxs-lookup"><span data-stu-id="7d93f-102">SearchResult resource type</span></span>

<span data-ttu-id="7d93f-103">**SearchResult** リソースは、アイテムが検索クエリへの応答であることを示します。</span><span class="sxs-lookup"><span data-stu-id="7d93f-103">The **SearchResult** resource indicates than an item is the response to a search query.</span></span>

## <a name="json-representation"></a><span data-ttu-id="7d93f-104">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="7d93f-104">JSON representation</span></span>

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

## <a name="properties"></a><span data-ttu-id="7d93f-105">プロパティ</span><span class="sxs-lookup"><span data-stu-id="7d93f-105">Properties</span></span>

| <span data-ttu-id="7d93f-106">プロパティ</span><span class="sxs-lookup"><span data-stu-id="7d93f-106">Property</span></span>            | <span data-ttu-id="7d93f-107">種類</span><span class="sxs-lookup"><span data-stu-id="7d93f-107">Type</span></span>   | <span data-ttu-id="7d93f-108">説明</span><span class="sxs-lookup"><span data-stu-id="7d93f-108">Description</span></span>
|:--------------------|:-------|:----------------------------------------------
| <span data-ttu-id="7d93f-109">onClickTelemetryUrl</span><span class="sxs-lookup"><span data-stu-id="7d93f-109">onClickTelemetryUrl</span></span> | <span data-ttu-id="7d93f-110">String</span><span class="sxs-lookup"><span data-stu-id="7d93f-110">String</span></span> | <span data-ttu-id="7d93f-p101">テレメトリ情報の記録に使用できるコールバックの URL。ユーザーがより正確な結果を得るためにこのアイテムを操作する場合は、アプリケーションからこの URL に対して GET を発行する必要があります。</span><span class="sxs-lookup"><span data-stu-id="7d93f-p101">A callback URL that can be used to record telemetry information. The application should issue a GET on this URL if the user interacts with this item to improve the quality of results.</span></span>

## <a name="remarks"></a><span data-ttu-id="7d93f-113">注釈</span><span class="sxs-lookup"><span data-stu-id="7d93f-113">Remarks</span></span> 

<span data-ttu-id="7d93f-114">DriveItem のファセットの詳細については、「[DriveItem](driveitem.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="7d93f-114">For more information about the facets on a DriveItem, see [DriveItem](driveitem.md).</span></span>

<!-- {
  "type": "#page.annotation",
  "description": "The search result facet indicates an item is from a search.",
  "keywords": "search result facet",
  "section": "documentation",
  "tocPath": "Facets/SearchResult"
} -->
