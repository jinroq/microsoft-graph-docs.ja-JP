---
author: daspek
ms.author: dspektor
title: リソースの種類での itemactiv
description: Itemactivitのオブジェクトは、アイテムに対して行われたアクティビティに関する情報を提供します。
localization_priority: Normal
ms.prod: sharepoint
doc_type: resourcePageType
ms.openlocfilehash: bf4396e6da5c56b19d33d7a914d864cb6dd54592
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "36036674"
---
# <a name="itemactivitystat-resource-type"></a><span data-ttu-id="f96b2-103">リソースの種類での itemactiv</span><span class="sxs-lookup"><span data-stu-id="f96b2-103">itemActivityStat resource type</span></span>

<span data-ttu-id="f96b2-104">**Itemactivit(** リソース) は、ある期間内に発生したアクティビティに関する情報を提供します。</span><span class="sxs-lookup"><span data-stu-id="f96b2-104">The **itemActivityStat** resource provides information about activities that took place within an interval of time.</span></span>

## <a name="properties"></a><span data-ttu-id="f96b2-105">プロパティ</span><span class="sxs-lookup"><span data-stu-id="f96b2-105">Properties</span></span>

| <span data-ttu-id="f96b2-106">プロパティ</span><span class="sxs-lookup"><span data-stu-id="f96b2-106">Property</span></span>         | <span data-ttu-id="f96b2-107">型</span><span class="sxs-lookup"><span data-stu-id="f96b2-107">Type</span></span>                    | <span data-ttu-id="f96b2-108">説明</span><span class="sxs-lookup"><span data-stu-id="f96b2-108">Description</span></span>
|:-----------------|:------------------------|:----------------------------------------
| <span data-ttu-id="f96b2-109">incompleteData</span><span class="sxs-lookup"><span data-stu-id="f96b2-109">incompleteData</span></span>   | <span data-ttu-id="f96b2-110">[incompleteData][]</span><span class="sxs-lookup"><span data-stu-id="f96b2-110">[incompleteData][]</span></span>      | <span data-ttu-id="f96b2-111">この間隔の統計情報が不完全なデータに基づくことを示します。</span><span class="sxs-lookup"><span data-stu-id="f96b2-111">Indicates that the statistics in this interval are based on incomplete data.</span></span> <span data-ttu-id="f96b2-112">読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="f96b2-112">Read-only.</span></span>
| <span data-ttu-id="f96b2-113">isTrending</span><span class="sxs-lookup"><span data-stu-id="f96b2-113">isTrending</span></span>       | <span data-ttu-id="f96b2-114">Boolean</span><span class="sxs-lookup"><span data-stu-id="f96b2-114">Boolean</span></span>                 | <span data-ttu-id="f96b2-115">アイテムが "傾向" であるかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="f96b2-115">Indicates whether the item is "trending."</span></span> <span data-ttu-id="f96b2-116">読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="f96b2-116">Read-only.</span></span>
| <span data-ttu-id="f96b2-117">startDateTime</span><span class="sxs-lookup"><span data-stu-id="f96b2-117">startDateTime</span></span>    | <span data-ttu-id="f96b2-118">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="f96b2-118">DateTimeOffset</span></span>          | <span data-ttu-id="f96b2-119">間隔が開始されたとき。</span><span class="sxs-lookup"><span data-stu-id="f96b2-119">When the interval starts.</span></span> <span data-ttu-id="f96b2-120">読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="f96b2-120">Read-only.</span></span>
| <span data-ttu-id="f96b2-121">endDateTime</span><span class="sxs-lookup"><span data-stu-id="f96b2-121">endDateTime</span></span>      | <span data-ttu-id="f96b2-122">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="f96b2-122">DateTimeOffset</span></span>          | <span data-ttu-id="f96b2-123">間隔が終了したとき。</span><span class="sxs-lookup"><span data-stu-id="f96b2-123">When the interval ends.</span></span> <span data-ttu-id="f96b2-124">読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="f96b2-124">Read-only.</span></span>
| <span data-ttu-id="f96b2-125">create</span><span class="sxs-lookup"><span data-stu-id="f96b2-125">create</span></span>           | <span data-ttu-id="f96b2-126">[itemActionStat][]</span><span class="sxs-lookup"><span data-stu-id="f96b2-126">[itemActionStat][]</span></span>      | <span data-ttu-id="f96b2-127">この間隔における**create**アクションに関する統計。</span><span class="sxs-lookup"><span data-stu-id="f96b2-127">Statistics about the **create** actions in this interval.</span></span> <span data-ttu-id="f96b2-128">読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="f96b2-128">Read-only.</span></span>
| <span data-ttu-id="f96b2-129">edit</span><span class="sxs-lookup"><span data-stu-id="f96b2-129">edit</span></span>             | <span data-ttu-id="f96b2-130">[itemActionStat][]</span><span class="sxs-lookup"><span data-stu-id="f96b2-130">[itemActionStat][]</span></span>      | <span data-ttu-id="f96b2-131">この間隔の**編集**アクションに関する統計。</span><span class="sxs-lookup"><span data-stu-id="f96b2-131">Statistics about the **edit** actions in this interval.</span></span> <span data-ttu-id="f96b2-132">読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="f96b2-132">Read-only.</span></span>
| <span data-ttu-id="f96b2-133">delete</span><span class="sxs-lookup"><span data-stu-id="f96b2-133">delete</span></span>           | <span data-ttu-id="f96b2-134">[itemActionStat][]</span><span class="sxs-lookup"><span data-stu-id="f96b2-134">[itemActionStat][]</span></span>      | <span data-ttu-id="f96b2-135">この間隔の**削除**アクションに関する統計情報。</span><span class="sxs-lookup"><span data-stu-id="f96b2-135">Statistics about the **delete** actions in this interval.</span></span> <span data-ttu-id="f96b2-136">読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="f96b2-136">Read-only.</span></span>
| <span data-ttu-id="f96b2-137">move</span><span class="sxs-lookup"><span data-stu-id="f96b2-137">move</span></span>             | <span data-ttu-id="f96b2-138">[itemActionStat][]</span><span class="sxs-lookup"><span data-stu-id="f96b2-138">[itemActionStat][]</span></span>      | <span data-ttu-id="f96b2-139">この間隔における**移動**アクションに関する統計。</span><span class="sxs-lookup"><span data-stu-id="f96b2-139">Statistics about the **move** actions in this interval.</span></span> <span data-ttu-id="f96b2-140">読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="f96b2-140">Read-only.</span></span>
| <span data-ttu-id="f96b2-141">接続</span><span class="sxs-lookup"><span data-stu-id="f96b2-141">access</span></span>           | <span data-ttu-id="f96b2-142">[itemActionStat][]</span><span class="sxs-lookup"><span data-stu-id="f96b2-142">[itemActionStat][]</span></span>      | <span data-ttu-id="f96b2-143">この間隔における**アクセス**アクションに関する統計情報。</span><span class="sxs-lookup"><span data-stu-id="f96b2-143">Statistics about the **access** actions in this interval.</span></span> <span data-ttu-id="f96b2-144">読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="f96b2-144">Read-only.</span></span>

[itemActionStat]: itemactionstat.md
[incompleteData]: incompletedata.md

## <a name="relationships"></a><span data-ttu-id="f96b2-147">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="f96b2-147">Relationships</span></span>

| <span data-ttu-id="f96b2-148">リレーションシップ名</span><span class="sxs-lookup"><span data-stu-id="f96b2-148">Relationship name</span></span> | <span data-ttu-id="f96b2-149">種類</span><span class="sxs-lookup"><span data-stu-id="f96b2-149">Type</span></span>                        | <span data-ttu-id="f96b2-150">説明</span><span class="sxs-lookup"><span data-stu-id="f96b2-150">Description</span></span>
|:------------------|:----------------------------|:---------------------------
| <span data-ttu-id="f96b2-151">アクティビティ</span><span class="sxs-lookup"><span data-stu-id="f96b2-151">activities</span></span>        | <span data-ttu-id="f96b2-152">[itemActivity][] コレクション</span><span class="sxs-lookup"><span data-stu-id="f96b2-152">[itemActivity][] collection</span></span> | <span data-ttu-id="f96b2-153">この**Itemactivitの**リソースで表された**itemactivities**を公開します。</span><span class="sxs-lookup"><span data-stu-id="f96b2-153">Exposes the **itemActivities** represented in this **itemActivityStat** resource.</span></span>

[itemActivity]: itemactivity.md

## <a name="json-representation"></a><span data-ttu-id="f96b2-155">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="f96b2-155">JSON representation</span></span>

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
