---
author: rgregg
ms.author: rgregg
ms.date: 09/10/2017
title: SearchResult
ms.openlocfilehash: 7e6bd6e6ff48ae34e197955d16a3df1d539a3c05
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27071799"
---
# <a name="searchresult-resource-type"></a><span data-ttu-id="a9fb3-102">SearchResult リソースの種類</span><span class="sxs-lookup"><span data-stu-id="a9fb3-102">SearchResult resource type</span></span>

> <span data-ttu-id="a9fb3-103">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="a9fb3-103">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="a9fb3-104">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="a9fb3-104">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="a9fb3-105">**SearchResult** リソースは、アイテムが検索クエリへの応答であることを示します。</span><span class="sxs-lookup"><span data-stu-id="a9fb3-105">The **SearchResult** resource indicates than an item is the response to a search query.</span></span>

## <a name="json-representation"></a><span data-ttu-id="a9fb3-106">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="a9fb3-106">JSON representation</span></span>

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

## <a name="properties"></a><span data-ttu-id="a9fb3-107">プロパティ</span><span class="sxs-lookup"><span data-stu-id="a9fb3-107">Properties</span></span>

| <span data-ttu-id="a9fb3-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="a9fb3-108">Property</span></span>            | <span data-ttu-id="a9fb3-109">型</span><span class="sxs-lookup"><span data-stu-id="a9fb3-109">Type</span></span>   | <span data-ttu-id="a9fb3-110">説明</span><span class="sxs-lookup"><span data-stu-id="a9fb3-110">Description</span></span>
|:--------------------|:-------|:----------------------------------------------
| <span data-ttu-id="a9fb3-111">onClickTelemetryUrl</span><span class="sxs-lookup"><span data-stu-id="a9fb3-111">onClickTelemetryUrl</span></span> | <span data-ttu-id="a9fb3-112">String</span><span class="sxs-lookup"><span data-stu-id="a9fb3-112">String</span></span> | <span data-ttu-id="a9fb3-p102">テレメトリ情報の記録に使用できるコールバックの URL。ユーザーがより正確な結果を得るためにこのアイテムを操作する場合は、アプリケーションからこの URL に対して GET を発行する必要があります。</span><span class="sxs-lookup"><span data-stu-id="a9fb3-p102">A callback URL that can be used to record telemetry information. The application should issue a GET on this URL if the user interacts with this item to improve the quality of results.</span></span>

## <a name="remarks"></a><span data-ttu-id="a9fb3-115">注釈</span><span class="sxs-lookup"><span data-stu-id="a9fb3-115">Remarks</span></span> 

<span data-ttu-id="a9fb3-116">DriveItem のファセットの詳細については、「[DriveItem](driveitem.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="a9fb3-116">For more information about the facets on a DriveItem, see [DriveItem](driveitem.md).</span></span>

<!-- {
  "type": "#page.annotation",
  "description": "The search result facet indicates an item is from a search.",
  "keywords": "search result facet",
  "section": "documentation",
  "tocPath": "Facets/SearchResult"
} -->
