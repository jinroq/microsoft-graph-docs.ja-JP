---
author: daspek
description: Itemactivit(リソース) は、ある期間内に発生したアクティビティに関する情報を提供します。
ms.date: 09/14/2017
title: Itemactiv
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
ms.openlocfilehash: 61c410d807869615ed35365743d1ae87b5b6e890
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "35967100"
---
# <a name="itemactivitystat-resource-type"></a><span data-ttu-id="7c00d-103">リソースの種類での itemactiv</span><span class="sxs-lookup"><span data-stu-id="7c00d-103">itemActivityStat resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="7c00d-104">**Itemactivit(** リソース) は、ある期間内に発生したアクティビティに関する情報を提供します。</span><span class="sxs-lookup"><span data-stu-id="7c00d-104">The **itemActivityStat** resource provides information about activities that took place within an interval of time.</span></span>

## <a name="json-representation"></a><span data-ttu-id="7c00d-105">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="7c00d-105">JSON representation</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [ ],
  "baseType": "microsoft.graph.entity",
  "@type": "microsoft.graph.itemActivityStat",
}-->

```json
{
  "activities": [{"@odata.type": "microsoft.graph.itemActivity"}],
  "incompleteData": {"@odata.type": "microsoft.graph.incompleteData"},
  "isTrending": true,
  "startDateTime": "String (timestamp)",
  "endDateTime": "String (timestamp)",
  "create": {"@odata.type": "microsoft.graph.itemActionStat"},
  "delete": {"@odata.type": "microsoft.graph.itemActionStat"},
  "edit": {"@odata.type": "microsoft.graph.itemActionStat"},
  "move": {"@odata.type": "microsoft.graph.itemActionStat"},
  "access": {"@odata.type": "microsoft.graph.itemActionStat"}
}
```

## <a name="properties"></a><span data-ttu-id="7c00d-106">プロパティ</span><span class="sxs-lookup"><span data-stu-id="7c00d-106">Properties</span></span>

| <span data-ttu-id="7c00d-107">プロパティ</span><span class="sxs-lookup"><span data-stu-id="7c00d-107">Property</span></span>         | <span data-ttu-id="7c00d-108">型</span><span class="sxs-lookup"><span data-stu-id="7c00d-108">Type</span></span>                    | <span data-ttu-id="7c00d-109">説明</span><span class="sxs-lookup"><span data-stu-id="7c00d-109">Description</span></span>
|:-----------------|:------------------------|:----------------------------------------
| <span data-ttu-id="7c00d-110">incompleteData</span><span class="sxs-lookup"><span data-stu-id="7c00d-110">incompleteData</span></span>   | <span data-ttu-id="7c00d-111">[incompleteData][]</span><span class="sxs-lookup"><span data-stu-id="7c00d-111">[incompleteData][]</span></span>      | <span data-ttu-id="7c00d-112">この間隔の統計情報が不完全なデータに基づくことを示します。</span><span class="sxs-lookup"><span data-stu-id="7c00d-112">Indicates that the statistics in this interval are based on incomplete data.</span></span> <span data-ttu-id="7c00d-113">読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="7c00d-113">Read-only.</span></span>
| <span data-ttu-id="7c00d-114">isTrending</span><span class="sxs-lookup"><span data-stu-id="7c00d-114">isTrending</span></span>       | <span data-ttu-id="7c00d-115">Boolean</span><span class="sxs-lookup"><span data-stu-id="7c00d-115">Boolean</span></span>                 | <span data-ttu-id="7c00d-116">アイテムが "傾向" であるかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="7c00d-116">Indicates whether the item is "trending."</span></span> <span data-ttu-id="7c00d-117">読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="7c00d-117">Read-only.</span></span>
| <span data-ttu-id="7c00d-118">startDateTime</span><span class="sxs-lookup"><span data-stu-id="7c00d-118">startDateTime</span></span>    | <span data-ttu-id="7c00d-119">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="7c00d-119">DateTimeOffset</span></span>          | <span data-ttu-id="7c00d-120">間隔が開始されたとき。</span><span class="sxs-lookup"><span data-stu-id="7c00d-120">When the interval starts.</span></span> <span data-ttu-id="7c00d-121">読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="7c00d-121">Read-only.</span></span>
| <span data-ttu-id="7c00d-122">endDateTime</span><span class="sxs-lookup"><span data-stu-id="7c00d-122">endDateTime</span></span>      | <span data-ttu-id="7c00d-123">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="7c00d-123">DateTimeOffset</span></span>          | <span data-ttu-id="7c00d-124">間隔が終了したとき。</span><span class="sxs-lookup"><span data-stu-id="7c00d-124">When the interval ends.</span></span> <span data-ttu-id="7c00d-125">読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="7c00d-125">Read-only.</span></span>
| <span data-ttu-id="7c00d-126">create</span><span class="sxs-lookup"><span data-stu-id="7c00d-126">create</span></span>           | <span data-ttu-id="7c00d-127">[itemActionStat][]</span><span class="sxs-lookup"><span data-stu-id="7c00d-127">[itemActionStat][]</span></span>      | <span data-ttu-id="7c00d-128">この間隔における**create**アクションに関する統計。</span><span class="sxs-lookup"><span data-stu-id="7c00d-128">Statistics about the **create** actions in this interval.</span></span> <span data-ttu-id="7c00d-129">読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="7c00d-129">Read-only.</span></span>
| <span data-ttu-id="7c00d-130">edit</span><span class="sxs-lookup"><span data-stu-id="7c00d-130">edit</span></span>             | <span data-ttu-id="7c00d-131">[itemActionStat][]</span><span class="sxs-lookup"><span data-stu-id="7c00d-131">[itemActionStat][]</span></span>      | <span data-ttu-id="7c00d-132">この間隔の**編集**アクションに関する統計。</span><span class="sxs-lookup"><span data-stu-id="7c00d-132">Statistics about the **edit** actions in this interval.</span></span> <span data-ttu-id="7c00d-133">読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="7c00d-133">Read-only.</span></span>
| <span data-ttu-id="7c00d-134">delete</span><span class="sxs-lookup"><span data-stu-id="7c00d-134">delete</span></span>           | <span data-ttu-id="7c00d-135">[itemActionStat][]</span><span class="sxs-lookup"><span data-stu-id="7c00d-135">[itemActionStat][]</span></span>      | <span data-ttu-id="7c00d-136">この間隔の**削除**アクションに関する統計情報。</span><span class="sxs-lookup"><span data-stu-id="7c00d-136">Statistics about the **delete** actions in this interval.</span></span> <span data-ttu-id="7c00d-137">読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="7c00d-137">Read-only.</span></span>
| <span data-ttu-id="7c00d-138">move</span><span class="sxs-lookup"><span data-stu-id="7c00d-138">move</span></span>             | <span data-ttu-id="7c00d-139">[itemActionStat][]</span><span class="sxs-lookup"><span data-stu-id="7c00d-139">[itemActionStat][]</span></span>      | <span data-ttu-id="7c00d-140">この間隔における**移動**アクションに関する統計。</span><span class="sxs-lookup"><span data-stu-id="7c00d-140">Statistics about the **move** actions in this interval.</span></span> <span data-ttu-id="7c00d-141">読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="7c00d-141">Read-only.</span></span>
| <span data-ttu-id="7c00d-142">接続</span><span class="sxs-lookup"><span data-stu-id="7c00d-142">access</span></span>           | <span data-ttu-id="7c00d-143">[itemActionStat][]</span><span class="sxs-lookup"><span data-stu-id="7c00d-143">[itemActionStat][]</span></span>      | <span data-ttu-id="7c00d-144">この間隔における**アクセス**アクションに関する統計情報。</span><span class="sxs-lookup"><span data-stu-id="7c00d-144">Statistics about the **access** actions in this interval.</span></span> <span data-ttu-id="7c00d-145">読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="7c00d-145">Read-only.</span></span>

[itemActionStat]: itemactionstat.md
[incompleteData]: incompletedata.md

## <a name="relationships"></a><span data-ttu-id="7c00d-148">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="7c00d-148">Relationships</span></span>

| <span data-ttu-id="7c00d-149">リレーションシップ名</span><span class="sxs-lookup"><span data-stu-id="7c00d-149">Relationship name</span></span> | <span data-ttu-id="7c00d-150">種類</span><span class="sxs-lookup"><span data-stu-id="7c00d-150">Type</span></span>                        | <span data-ttu-id="7c00d-151">説明</span><span class="sxs-lookup"><span data-stu-id="7c00d-151">Description</span></span>
|:------------------|:----------------------------|:---------------------------
| <span data-ttu-id="7c00d-152">アクティビティ</span><span class="sxs-lookup"><span data-stu-id="7c00d-152">activities</span></span>        | <span data-ttu-id="7c00d-153">[itemActivity][] コレクション</span><span class="sxs-lookup"><span data-stu-id="7c00d-153">[itemActivity][] collection</span></span> | <span data-ttu-id="7c00d-154">この**Itemactivitの**リソースで表された**itemactivities**を公開します。</span><span class="sxs-lookup"><span data-stu-id="7c00d-154">Exposes the **itemActivities** represented in this **itemActivityStat** resource.</span></span>

[itemActivity]: itemactivity.md

## <a name="remarks"></a><span data-ttu-id="7c00d-156">備考</span><span class="sxs-lookup"><span data-stu-id="7c00d-156">Remarks</span></span>

<!--
{
  "type": "#page.annotation",
  "description": "The ItemActivityStat object provides information about activities that took place on an item.",
  "keywords": "activities,activity,action,analytics",
  "section": "documentation",
  "tocPath": "Resources/ItemActivityStat",
  "suppressions": []
}
-->
