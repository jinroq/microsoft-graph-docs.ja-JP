---
author: rgregg
ms.author: rgregg
ms.date: 09/10/2017
title: SearchResult
ms.openlocfilehash: 33ce07c947d858f05844dd9dc2589379131c9dbb
ms.sourcegitcommit: 7aea7a97e36e6d146214de3a90fdbc71628aadba
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 09/28/2017
---
# <a name="searchresult-resource-type"></a><span data-ttu-id="07ecf-102">SearchResult リソース型</span><span class="sxs-lookup"><span data-stu-id="07ecf-102">SearchResult resource type</span></span>

<span data-ttu-id="07ecf-103">**SearchResult** リソースは、アイテムが検索クエリへの応答であることを示します。</span><span class="sxs-lookup"><span data-stu-id="07ecf-103">The **SearchResult** resource indicates than an item is the response to a search.</span></span>

## <a name="json-representation"></a><span data-ttu-id="07ecf-104">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="07ecf-104">JSON representation</span></span>

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

## <a name="properties"></a><span data-ttu-id="07ecf-105">プロパティ</span><span class="sxs-lookup"><span data-stu-id="07ecf-105">Properties</span></span>

| <span data-ttu-id="07ecf-106">プロパティ</span><span class="sxs-lookup"><span data-stu-id="07ecf-106">Property</span></span>            | <span data-ttu-id="07ecf-107">型</span><span class="sxs-lookup"><span data-stu-id="07ecf-107">Type</span></span>   | <span data-ttu-id="07ecf-108">説明</span><span class="sxs-lookup"><span data-stu-id="07ecf-108">Description</span></span>
|:--------------------|:-------|:----------------------------------------------
| <span data-ttu-id="07ecf-109">onClickTelemetryUrl</span><span class="sxs-lookup"><span data-stu-id="07ecf-109">onClickTelemetryUrl</span></span> | <span data-ttu-id="07ecf-110">String</span><span class="sxs-lookup"><span data-stu-id="07ecf-110">String</span></span> | <span data-ttu-id="07ecf-p101">テレメトリ情報の記録に使用できるコールバックの URL。ユーザーがより正確な結果を得るためにこのアイテムを操作する場合は、アプリケーションからこの URL に対して GET を発行する必要があります。</span><span class="sxs-lookup"><span data-stu-id="07ecf-p101">A callback URL that can be used to record telemetry information. The application should issue a GET on this URL if the user interacts with this item to improve the quality of results.</span></span>

## <a name="remarks"></a><span data-ttu-id="07ecf-113">注釈</span><span class="sxs-lookup"><span data-stu-id="07ecf-113">Remarks</span></span> 

<span data-ttu-id="07ecf-114">DriveItem のファセットの詳細については、「[DriveItem](driveitem.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="07ecf-114">For more information about the facets on a DriveItem, see [DriveItem](driveitem.md).</span></span>

<!-- {
  "type": "#page.annotation",
  "description": "The search result facet indicates an item is from a search.",
  "keywords": "search result facet",
  "section": "documentation",
  "tocPath": "Facets/SearchResult"
} -->
