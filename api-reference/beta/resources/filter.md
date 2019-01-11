---
title: フィルター リソースの種類
description: テーブルの列のフィルター処理を管理します。
localization_priority: Normal
ms.openlocfilehash: 5bbc4eff85f40e116ea513c27fa2966dd28a5493
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/11/2019
ms.locfileid: "27852788"
---
# <a name="filter-resource-type"></a><span data-ttu-id="ef04a-103">フィルター リソースの種類</span><span class="sxs-lookup"><span data-stu-id="ef04a-103">Filter resource type</span></span>

> <span data-ttu-id="ef04a-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="ef04a-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="ef04a-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="ef04a-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="ef04a-106">テーブルの列のフィルター処理を管理します。</span><span class="sxs-lookup"><span data-stu-id="ef04a-106">Manages the filtering of a table's column.</span></span>


## <a name="methods"></a><span data-ttu-id="ef04a-107">メソッド</span><span class="sxs-lookup"><span data-stu-id="ef04a-107">Methods</span></span>

| <span data-ttu-id="ef04a-108">メソッド</span><span class="sxs-lookup"><span data-stu-id="ef04a-108">Method</span></span>           | <span data-ttu-id="ef04a-109">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="ef04a-109">Return Type</span></span>    |<span data-ttu-id="ef04a-110">説明</span><span class="sxs-lookup"><span data-stu-id="ef04a-110">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="ef04a-111">Apply</span><span class="sxs-lookup"><span data-stu-id="ef04a-111">Apply</span></span>](../api/filter-apply.md)|<span data-ttu-id="ef04a-112">なし</span><span class="sxs-lookup"><span data-stu-id="ef04a-112">None</span></span>|<span data-ttu-id="ef04a-113">指定した列に指定されたフィルター条件を適用します。</span><span class="sxs-lookup"><span data-stu-id="ef04a-113">Apply the given filter criteria on the given column.</span></span>|
|[<span data-ttu-id="ef04a-114">Clear</span><span class="sxs-lookup"><span data-stu-id="ef04a-114">Clear</span></span>](../api/filter-clear.md)|<span data-ttu-id="ef04a-115">なし</span><span class="sxs-lookup"><span data-stu-id="ef04a-115">None</span></span>|<span data-ttu-id="ef04a-116">指定した列のフィルターをクリアします。</span><span class="sxs-lookup"><span data-stu-id="ef04a-116">Clear the filter on the given column.</span></span>|

## <a name="properties"></a><span data-ttu-id="ef04a-117">プロパティ</span><span class="sxs-lookup"><span data-stu-id="ef04a-117">Properties</span></span>
<span data-ttu-id="ef04a-118">なし</span><span class="sxs-lookup"><span data-stu-id="ef04a-118">None</span></span>

## <a name="relationships"></a><span data-ttu-id="ef04a-119">関係</span><span class="sxs-lookup"><span data-stu-id="ef04a-119">Relationships</span></span>
| <span data-ttu-id="ef04a-120">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="ef04a-120">Relationship</span></span> | <span data-ttu-id="ef04a-121">型</span><span class="sxs-lookup"><span data-stu-id="ef04a-121">Type</span></span>   |<span data-ttu-id="ef04a-122">説明</span><span class="sxs-lookup"><span data-stu-id="ef04a-122">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="ef04a-123">criteria</span><span class="sxs-lookup"><span data-stu-id="ef04a-123">criteria</span></span>|[<span data-ttu-id="ef04a-124">FilterCriteria</span><span class="sxs-lookup"><span data-stu-id="ef04a-124">FilterCriteria</span></span>](filtercriteria.md)|<span data-ttu-id="ef04a-p102">指定した列に現在適用されているフィルターです。読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="ef04a-p102">The currently applied filter on the given column. Read-only.</span></span>|

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Filter resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
