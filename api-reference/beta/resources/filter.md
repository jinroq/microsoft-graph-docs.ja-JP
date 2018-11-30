---
title: フィルター リソースの種類
description: テーブルの列のフィルター処理を管理します。
ms.openlocfilehash: df896d10b1e8734015d38b92b5824e3e3652e3a6
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27071070"
---
# <a name="filter-resource-type"></a><span data-ttu-id="16f7b-103">フィルター リソースの種類</span><span class="sxs-lookup"><span data-stu-id="16f7b-103">Filter resource type</span></span>

> <span data-ttu-id="16f7b-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="16f7b-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="16f7b-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="16f7b-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="16f7b-106">テーブルの列のフィルター処理を管理します。</span><span class="sxs-lookup"><span data-stu-id="16f7b-106">Manages the filtering of a table's column.</span></span>


## <a name="methods"></a><span data-ttu-id="16f7b-107">メソッド</span><span class="sxs-lookup"><span data-stu-id="16f7b-107">Methods</span></span>

| <span data-ttu-id="16f7b-108">メソッド</span><span class="sxs-lookup"><span data-stu-id="16f7b-108">Method</span></span>           | <span data-ttu-id="16f7b-109">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="16f7b-109">Return Type</span></span>    |<span data-ttu-id="16f7b-110">説明</span><span class="sxs-lookup"><span data-stu-id="16f7b-110">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="16f7b-111">適用</span><span class="sxs-lookup"><span data-stu-id="16f7b-111">Apply</span></span>](../api/filter-apply.md)|<span data-ttu-id="16f7b-112">なし</span><span class="sxs-lookup"><span data-stu-id="16f7b-112">None</span></span>|<span data-ttu-id="16f7b-113">指定した列に指定されたフィルター条件を適用します。</span><span class="sxs-lookup"><span data-stu-id="16f7b-113">Apply the given filter criteria on the given column.</span></span>|
|[<span data-ttu-id="16f7b-114">クリア</span><span class="sxs-lookup"><span data-stu-id="16f7b-114">Clear</span></span>](../api/filter-clear.md)|<span data-ttu-id="16f7b-115">なし</span><span class="sxs-lookup"><span data-stu-id="16f7b-115">None</span></span>|<span data-ttu-id="16f7b-116">指定した列のフィルターをクリアします。</span><span class="sxs-lookup"><span data-stu-id="16f7b-116">Clear the filter on the given column.</span></span>|

## <a name="properties"></a><span data-ttu-id="16f7b-117">プロパティ</span><span class="sxs-lookup"><span data-stu-id="16f7b-117">Properties</span></span>
<span data-ttu-id="16f7b-118">なし</span><span class="sxs-lookup"><span data-stu-id="16f7b-118">None</span></span>

## <a name="relationships"></a><span data-ttu-id="16f7b-119">関係</span><span class="sxs-lookup"><span data-stu-id="16f7b-119">Relationships</span></span>
| <span data-ttu-id="16f7b-120">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="16f7b-120">Relationship</span></span> | <span data-ttu-id="16f7b-121">型</span><span class="sxs-lookup"><span data-stu-id="16f7b-121">Type</span></span>   |<span data-ttu-id="16f7b-122">説明</span><span class="sxs-lookup"><span data-stu-id="16f7b-122">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="16f7b-123">criteria</span><span class="sxs-lookup"><span data-stu-id="16f7b-123">criteria</span></span>|[<span data-ttu-id="16f7b-124">FilterCriteria</span><span class="sxs-lookup"><span data-stu-id="16f7b-124">FilterCriteria</span></span>](filtercriteria.md)|<span data-ttu-id="16f7b-p102">指定した列に現在適用されているフィルターです。読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="16f7b-p102">The currently applied filter on the given column. Read-only.</span></span>|

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Filter resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->