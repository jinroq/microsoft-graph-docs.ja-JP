---
author: JeremyKelley
ms.author: JeremyKelley
ms.date: 09/10/2017
title: Searchresult.xml
localization_priority: Normal
description: SearchResult リソースは、アイテムが検索クエリへの応答であることを示します。
ms.prod: ''
doc_type: resourcePageType
ms.openlocfilehash: e6c0c458d9e6e3d31060cec49419b6b2438d5b00
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "36034574"
---
# <a name="searchresult-resource-type"></a><span data-ttu-id="b9bcc-103">SearchResult リソースの種類</span><span class="sxs-lookup"><span data-stu-id="b9bcc-103">SearchResult resource type</span></span>

<span data-ttu-id="b9bcc-104">**SearchResult** リソースは、アイテムが検索クエリへの応答であることを示します。</span><span class="sxs-lookup"><span data-stu-id="b9bcc-104">The **SearchResult** resource indicates than an item is the response to a search query.</span></span>

## <a name="json-representation"></a><span data-ttu-id="b9bcc-105">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="b9bcc-105">JSON representation</span></span>

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

## <a name="properties"></a><span data-ttu-id="b9bcc-106">プロパティ</span><span class="sxs-lookup"><span data-stu-id="b9bcc-106">Properties</span></span>

| <span data-ttu-id="b9bcc-107">プロパティ</span><span class="sxs-lookup"><span data-stu-id="b9bcc-107">Property</span></span>            | <span data-ttu-id="b9bcc-108">型</span><span class="sxs-lookup"><span data-stu-id="b9bcc-108">Type</span></span>   | <span data-ttu-id="b9bcc-109">説明</span><span class="sxs-lookup"><span data-stu-id="b9bcc-109">Description</span></span>
|:--------------------|:-------|:----------------------------------------------
| <span data-ttu-id="b9bcc-110">onClickTelemetryUrl</span><span class="sxs-lookup"><span data-stu-id="b9bcc-110">onClickTelemetryUrl</span></span> | <span data-ttu-id="b9bcc-111">String</span><span class="sxs-lookup"><span data-stu-id="b9bcc-111">String</span></span> | <span data-ttu-id="b9bcc-p101">テレメトリ情報の記録に使用できるコールバックの URL。ユーザーがより正確な結果を得るためにこのアイテムを操作する場合は、アプリケーションからこの URL に対して GET を発行する必要があります。</span><span class="sxs-lookup"><span data-stu-id="b9bcc-p101">A callback URL that can be used to record telemetry information. The application should issue a GET on this URL if the user interacts with this item to improve the quality of results.</span></span>

## <a name="remarks"></a><span data-ttu-id="b9bcc-114">注釈</span><span class="sxs-lookup"><span data-stu-id="b9bcc-114">Remarks</span></span> 

<span data-ttu-id="b9bcc-115">DriveItem のファセットの詳細については、「[DriveItem](driveitem.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="b9bcc-115">For more information about the facets on a DriveItem, see [DriveItem](driveitem.md).</span></span>

<!-- {
  "type": "#page.annotation",
  "description": "The search result facet indicates an item is from a search.",
  "keywords": "search result facet",
  "section": "documentation",
  "tocPath": "Facets/SearchResult"
} -->
