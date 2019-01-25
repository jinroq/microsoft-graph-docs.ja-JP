---
title: フィルター リソースの種類
description: テーブルの列のフィルター処理を管理します。
localization_priority: Normal
ms.openlocfilehash: 6adc4e378b47bcb134a640e77bf54c32a35b3be2
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/24/2019
ms.locfileid: "29518892"
---
# <a name="filter-resource-type"></a><span data-ttu-id="c602d-103">フィルター リソースの種類</span><span class="sxs-lookup"><span data-stu-id="c602d-103">Filter resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="c602d-104">テーブルの列のフィルター処理を管理します。</span><span class="sxs-lookup"><span data-stu-id="c602d-104">Manages the filtering of a table's column.</span></span>


## <a name="methods"></a><span data-ttu-id="c602d-105">メソッド</span><span class="sxs-lookup"><span data-stu-id="c602d-105">Methods</span></span>

| <span data-ttu-id="c602d-106">メソッド</span><span class="sxs-lookup"><span data-stu-id="c602d-106">Method</span></span>           | <span data-ttu-id="c602d-107">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="c602d-107">Return Type</span></span>    |<span data-ttu-id="c602d-108">説明</span><span class="sxs-lookup"><span data-stu-id="c602d-108">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="c602d-109">Apply</span><span class="sxs-lookup"><span data-stu-id="c602d-109">Apply</span></span>](../api/filter-apply.md)|<span data-ttu-id="c602d-110">なし</span><span class="sxs-lookup"><span data-stu-id="c602d-110">None</span></span>|<span data-ttu-id="c602d-111">指定した列に指定されたフィルター条件を適用します。</span><span class="sxs-lookup"><span data-stu-id="c602d-111">Apply the given filter criteria on the given column.</span></span>|
|[<span data-ttu-id="c602d-112">Clear</span><span class="sxs-lookup"><span data-stu-id="c602d-112">Clear</span></span>](../api/filter-clear.md)|<span data-ttu-id="c602d-113">なし</span><span class="sxs-lookup"><span data-stu-id="c602d-113">None</span></span>|<span data-ttu-id="c602d-114">指定した列のフィルターをクリアします。</span><span class="sxs-lookup"><span data-stu-id="c602d-114">Clear the filter on the given column.</span></span>|

## <a name="properties"></a><span data-ttu-id="c602d-115">プロパティ</span><span class="sxs-lookup"><span data-stu-id="c602d-115">Properties</span></span>
<span data-ttu-id="c602d-116">なし</span><span class="sxs-lookup"><span data-stu-id="c602d-116">None</span></span>

## <a name="relationships"></a><span data-ttu-id="c602d-117">関係</span><span class="sxs-lookup"><span data-stu-id="c602d-117">Relationships</span></span>
| <span data-ttu-id="c602d-118">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="c602d-118">Relationship</span></span> | <span data-ttu-id="c602d-119">型</span><span class="sxs-lookup"><span data-stu-id="c602d-119">Type</span></span>   |<span data-ttu-id="c602d-120">説明</span><span class="sxs-lookup"><span data-stu-id="c602d-120">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="c602d-121">criteria</span><span class="sxs-lookup"><span data-stu-id="c602d-121">criteria</span></span>|[<span data-ttu-id="c602d-122">FilterCriteria</span><span class="sxs-lookup"><span data-stu-id="c602d-122">FilterCriteria</span></span>](filtercriteria.md)|<span data-ttu-id="c602d-p101">指定した列に現在適用されているフィルターです。読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="c602d-p101">The currently applied filter on the given column. Read-only.</span></span>|

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Filter resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/filter.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
