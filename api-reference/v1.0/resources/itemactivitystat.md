---
author: daspek
ms.author: dspektor
title: リソースの種類での itemactiv
description: Itemactivitのオブジェクトは、アイテムに対して行われたアクティビティに関する情報を提供します。
localization_priority: Normal
ms.prod: sharepoint
ms.openlocfilehash: 3af10bba565585341d04cdc47702e18e71d8accd
ms.sourcegitcommit: 52baf24d1d08096214b12f60e7c755291fe03ab5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/13/2019
ms.locfileid: "33970760"
---
# <a name="itemactivitystat-resource-type"></a><span data-ttu-id="46916-103">リソースの種類での itemactiv</span><span class="sxs-lookup"><span data-stu-id="46916-103">itemActivityStat resource type</span></span>

<span data-ttu-id="46916-104">**Itemactivit(** リソース) は、ある期間内に発生したアクティビティに関する情報を提供します。</span><span class="sxs-lookup"><span data-stu-id="46916-104">The **itemActivityStat** resource provides information about activities that took place within an interval of time.</span></span>

## <a name="properties"></a><span data-ttu-id="46916-105">プロパティ</span><span class="sxs-lookup"><span data-stu-id="46916-105">Properties</span></span>

| <span data-ttu-id="46916-106">プロパティ</span><span class="sxs-lookup"><span data-stu-id="46916-106">Property</span></span>         | <span data-ttu-id="46916-107">型</span><span class="sxs-lookup"><span data-stu-id="46916-107">Type</span></span>                    | <span data-ttu-id="46916-108">説明</span><span class="sxs-lookup"><span data-stu-id="46916-108">Description</span></span>
|:-----------------|:------------------------|:----------------------------------------
| <span data-ttu-id="46916-109">incompleteData</span><span class="sxs-lookup"><span data-stu-id="46916-109">incompleteData</span></span>   | <span data-ttu-id="46916-110">[incompleteData][]</span><span class="sxs-lookup"><span data-stu-id="46916-110">[incompleteData][]</span></span>      | <span data-ttu-id="46916-111">この間隔の統計情報が不完全なデータに基づくことを示します。</span><span class="sxs-lookup"><span data-stu-id="46916-111">Indicates that the statistics in this interval are based on incomplete data.</span></span> <span data-ttu-id="46916-112">値の取得のみ可能です。</span><span class="sxs-lookup"><span data-stu-id="46916-112">Read-only.</span></span>
| <span data-ttu-id="46916-113">isTrending</span><span class="sxs-lookup"><span data-stu-id="46916-113">isTrending</span></span>       | <span data-ttu-id="46916-114">Boolean</span><span class="sxs-lookup"><span data-stu-id="46916-114">Boolean</span></span>                 | <span data-ttu-id="46916-115">アイテムが "傾向" であるかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="46916-115">Indicates whether the item is "trending."</span></span> <span data-ttu-id="46916-116">値の取得のみ可能です。</span><span class="sxs-lookup"><span data-stu-id="46916-116">Read-only.</span></span>
| <span data-ttu-id="46916-117">startDateTime</span><span class="sxs-lookup"><span data-stu-id="46916-117">startDateTime</span></span>    | <span data-ttu-id="46916-118">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="46916-118">DateTimeOffset</span></span>          | <span data-ttu-id="46916-119">間隔が開始されたとき。</span><span class="sxs-lookup"><span data-stu-id="46916-119">When the interval starts.</span></span> <span data-ttu-id="46916-120">値の取得のみ可能です。</span><span class="sxs-lookup"><span data-stu-id="46916-120">Read-only.</span></span>
| <span data-ttu-id="46916-121">endDateTime</span><span class="sxs-lookup"><span data-stu-id="46916-121">endDateTime</span></span>      | <span data-ttu-id="46916-122">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="46916-122">DateTimeOffset</span></span>          | <span data-ttu-id="46916-123">間隔が終了したとき。</span><span class="sxs-lookup"><span data-stu-id="46916-123">When the interval ends.</span></span> <span data-ttu-id="46916-124">値の取得のみ可能です。</span><span class="sxs-lookup"><span data-stu-id="46916-124">Read-only.</span></span>
| <span data-ttu-id="46916-125">create</span><span class="sxs-lookup"><span data-stu-id="46916-125">create</span></span>           | <span data-ttu-id="46916-126">[itemActionStat][]</span><span class="sxs-lookup"><span data-stu-id="46916-126">[itemActionStat][]</span></span>      | <span data-ttu-id="46916-127">この間隔における**create**アクションに関する統計。</span><span class="sxs-lookup"><span data-stu-id="46916-127">Statistics about the **create** actions in this interval.</span></span> <span data-ttu-id="46916-128">値の取得のみ可能です。</span><span class="sxs-lookup"><span data-stu-id="46916-128">Read-only.</span></span>
| <span data-ttu-id="46916-129">edit</span><span class="sxs-lookup"><span data-stu-id="46916-129">edit</span></span>             | <span data-ttu-id="46916-130">[itemActionStat][]</span><span class="sxs-lookup"><span data-stu-id="46916-130">[itemActionStat][]</span></span>      | <span data-ttu-id="46916-131">この間隔の**編集**アクションに関する統計。</span><span class="sxs-lookup"><span data-stu-id="46916-131">Statistics about the **edit** actions in this interval.</span></span> <span data-ttu-id="46916-132">値の取得のみ可能です。</span><span class="sxs-lookup"><span data-stu-id="46916-132">Read-only.</span></span>
| <span data-ttu-id="46916-133">delete</span><span class="sxs-lookup"><span data-stu-id="46916-133">delete</span></span>           | <span data-ttu-id="46916-134">[itemActionStat][]</span><span class="sxs-lookup"><span data-stu-id="46916-134">[itemActionStat][]</span></span>      | <span data-ttu-id="46916-135">この間隔の**削除**アクションに関する統計情報。</span><span class="sxs-lookup"><span data-stu-id="46916-135">Statistics about the **delete** actions in this interval.</span></span> <span data-ttu-id="46916-136">値の取得のみ可能です。</span><span class="sxs-lookup"><span data-stu-id="46916-136">Read-only.</span></span>
| <span data-ttu-id="46916-137">move</span><span class="sxs-lookup"><span data-stu-id="46916-137">move</span></span>             | <span data-ttu-id="46916-138">[itemActionStat][]</span><span class="sxs-lookup"><span data-stu-id="46916-138">[itemActionStat][]</span></span>      | <span data-ttu-id="46916-139">この間隔における**移動**アクションに関する統計。</span><span class="sxs-lookup"><span data-stu-id="46916-139">Statistics about the **move** actions in this interval.</span></span> <span data-ttu-id="46916-140">値の取得のみ可能です。</span><span class="sxs-lookup"><span data-stu-id="46916-140">Read-only.</span></span>
| <span data-ttu-id="46916-141">接続</span><span class="sxs-lookup"><span data-stu-id="46916-141">access</span></span>           | <span data-ttu-id="46916-142">[itemActionStat][]</span><span class="sxs-lookup"><span data-stu-id="46916-142">[itemActionStat][]</span></span>      | <span data-ttu-id="46916-143">この間隔における**アクセス**アクションに関する統計情報。</span><span class="sxs-lookup"><span data-stu-id="46916-143">Statistics about the **access** actions in this interval.</span></span> <span data-ttu-id="46916-144">値の取得のみ可能です。</span><span class="sxs-lookup"><span data-stu-id="46916-144">Read-only.</span></span>

[itemActionStat]: itemactionstat.md
[incompleteData]: incompletedata.md

## <a name="relationships"></a><span data-ttu-id="46916-147">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="46916-147">Relationships</span></span>

| <span data-ttu-id="46916-148">リレーションシップ名</span><span class="sxs-lookup"><span data-stu-id="46916-148">Relationship name</span></span> | <span data-ttu-id="46916-149">種類</span><span class="sxs-lookup"><span data-stu-id="46916-149">Type</span></span>                        | <span data-ttu-id="46916-150">説明</span><span class="sxs-lookup"><span data-stu-id="46916-150">Description</span></span>
|:------------------|:----------------------------|:---------------------------
| <span data-ttu-id="46916-151">アクティビティ</span><span class="sxs-lookup"><span data-stu-id="46916-151">activities</span></span>        | <span data-ttu-id="46916-152">[itemActivity][] コレクション</span><span class="sxs-lookup"><span data-stu-id="46916-152">[itemActivity][] collection</span></span> | <span data-ttu-id="46916-153">この**Itemactivitの**リソースで表された**Itemactivities**を公開します。</span><span class="sxs-lookup"><span data-stu-id="46916-153">Exposes the **itemActivities** represented in this **itemActivityStat** resource.</span></span>

[itemActivity]: itemactivity.md

## <a name="json-representation"></a><span data-ttu-id="46916-155">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="46916-155">JSON representation</span></span>

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
