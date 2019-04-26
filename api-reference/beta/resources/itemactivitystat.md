---
author: daspek
ms.author: dspektor
ms.date: 09/14/2017
title: itemactiv
localization_priority: Normal
ms.openlocfilehash: 08bbfd414a32e8eb8a0144d879ede55c71c19b89
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/26/2019
ms.locfileid: "33339882"
---
# <a name="itemactivitystat-resource-type"></a><span data-ttu-id="976a5-102">リソースの種類での itemactiv</span><span class="sxs-lookup"><span data-stu-id="976a5-102">itemActivityStat resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="976a5-103">**itemactivit(** リソース) は、ある期間内に発生したアクティビティに関する情報を提供します。</span><span class="sxs-lookup"><span data-stu-id="976a5-103">The **itemActivityStat** resource provides information about activities that took place within an interval of time.</span></span>

## <a name="json-representation"></a><span data-ttu-id="976a5-104">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="976a5-104">JSON representation</span></span>

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

## <a name="properties"></a><span data-ttu-id="976a5-105">プロパティ</span><span class="sxs-lookup"><span data-stu-id="976a5-105">Properties</span></span>

| <span data-ttu-id="976a5-106">プロパティ</span><span class="sxs-lookup"><span data-stu-id="976a5-106">Property</span></span>         | <span data-ttu-id="976a5-107">型</span><span class="sxs-lookup"><span data-stu-id="976a5-107">Type</span></span>                    | <span data-ttu-id="976a5-108">説明</span><span class="sxs-lookup"><span data-stu-id="976a5-108">Description</span></span>
|:-----------------|:------------------------|:----------------------------------------
| <span data-ttu-id="976a5-109">incompletedata</span><span class="sxs-lookup"><span data-stu-id="976a5-109">incompleteData</span></span>   | <span data-ttu-id="976a5-110">[incompletedata][]</span><span class="sxs-lookup"><span data-stu-id="976a5-110">[incompleteData][]</span></span>      | <span data-ttu-id="976a5-111">この間隔の統計情報が不完全なデータに基づくことを示します。</span><span class="sxs-lookup"><span data-stu-id="976a5-111">Indicates that the statistics in this interval are based on incomplete data.</span></span> <span data-ttu-id="976a5-112">読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="976a5-112">Read-only.</span></span>
| <span data-ttu-id="976a5-113">istrending</span><span class="sxs-lookup"><span data-stu-id="976a5-113">isTrending</span></span>       | <span data-ttu-id="976a5-114">Boolean</span><span class="sxs-lookup"><span data-stu-id="976a5-114">Boolean</span></span>                 | <span data-ttu-id="976a5-115">アイテムが "傾向" であるかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="976a5-115">Indicates whether the item is "trending."</span></span> <span data-ttu-id="976a5-116">読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="976a5-116">Read-only.</span></span>
| <span data-ttu-id="976a5-117">startDateTime</span><span class="sxs-lookup"><span data-stu-id="976a5-117">startDateTime</span></span>    | <span data-ttu-id="976a5-118">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="976a5-118">DateTimeOffset</span></span>          | <span data-ttu-id="976a5-119">間隔が開始されたとき。</span><span class="sxs-lookup"><span data-stu-id="976a5-119">When the interval starts.</span></span> <span data-ttu-id="976a5-120">読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="976a5-120">Read-only.</span></span>
| <span data-ttu-id="976a5-121">endDateTime</span><span class="sxs-lookup"><span data-stu-id="976a5-121">endDateTime</span></span>      | <span data-ttu-id="976a5-122">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="976a5-122">DateTimeOffset</span></span>          | <span data-ttu-id="976a5-123">間隔が終了したとき。</span><span class="sxs-lookup"><span data-stu-id="976a5-123">When the interval ends.</span></span> <span data-ttu-id="976a5-124">読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="976a5-124">Read-only.</span></span>
| <span data-ttu-id="976a5-125">create</span><span class="sxs-lookup"><span data-stu-id="976a5-125">create</span></span>           | <span data-ttu-id="976a5-126">[itemactionstat][]</span><span class="sxs-lookup"><span data-stu-id="976a5-126">[itemActionStat][]</span></span>      | <span data-ttu-id="976a5-127">この間隔における**create**アクションに関する統計。</span><span class="sxs-lookup"><span data-stu-id="976a5-127">Statistics about the **create** actions in this interval.</span></span> <span data-ttu-id="976a5-128">読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="976a5-128">Read-only.</span></span>
| <span data-ttu-id="976a5-129">edit</span><span class="sxs-lookup"><span data-stu-id="976a5-129">edit</span></span>             | <span data-ttu-id="976a5-130">[itemactionstat][]</span><span class="sxs-lookup"><span data-stu-id="976a5-130">[itemActionStat][]</span></span>      | <span data-ttu-id="976a5-131">この間隔の**編集**アクションに関する統計。</span><span class="sxs-lookup"><span data-stu-id="976a5-131">Statistics about the **edit** actions in this interval.</span></span> <span data-ttu-id="976a5-132">読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="976a5-132">Read-only.</span></span>
| <span data-ttu-id="976a5-133">delete</span><span class="sxs-lookup"><span data-stu-id="976a5-133">delete</span></span>           | <span data-ttu-id="976a5-134">[itemactionstat][]</span><span class="sxs-lookup"><span data-stu-id="976a5-134">[itemActionStat][]</span></span>      | <span data-ttu-id="976a5-135">この間隔の**削除**アクションに関する統計情報。</span><span class="sxs-lookup"><span data-stu-id="976a5-135">Statistics about the **delete** actions in this interval.</span></span> <span data-ttu-id="976a5-136">読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="976a5-136">Read-only.</span></span>
| <span data-ttu-id="976a5-137">move</span><span class="sxs-lookup"><span data-stu-id="976a5-137">move</span></span>             | <span data-ttu-id="976a5-138">[itemactionstat][]</span><span class="sxs-lookup"><span data-stu-id="976a5-138">[itemActionStat][]</span></span>      | <span data-ttu-id="976a5-139">この間隔における**移動**アクションに関する統計。</span><span class="sxs-lookup"><span data-stu-id="976a5-139">Statistics about the **move** actions in this interval.</span></span> <span data-ttu-id="976a5-140">読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="976a5-140">Read-only.</span></span>
| <span data-ttu-id="976a5-141">接続</span><span class="sxs-lookup"><span data-stu-id="976a5-141">access</span></span>           | <span data-ttu-id="976a5-142">[itemactionstat][]</span><span class="sxs-lookup"><span data-stu-id="976a5-142">[itemActionStat][]</span></span>      | <span data-ttu-id="976a5-143">この間隔における**アクセス**アクションに関する統計情報。</span><span class="sxs-lookup"><span data-stu-id="976a5-143">Statistics about the **access** actions in this interval.</span></span> <span data-ttu-id="976a5-144">読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="976a5-144">Read-only.</span></span>

[itemactionstat]: itemactionstat.md
[itemActionStat]: itemactionstat.md
[incompletedata]: incompletedata.md
[incompleteData]: incompletedata.md

## <a name="relationships"></a><span data-ttu-id="976a5-147">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="976a5-147">Relationships</span></span>

| <span data-ttu-id="976a5-148">リレーションシップ名</span><span class="sxs-lookup"><span data-stu-id="976a5-148">Relationship name</span></span> | <span data-ttu-id="976a5-149">種類</span><span class="sxs-lookup"><span data-stu-id="976a5-149">Type</span></span>                        | <span data-ttu-id="976a5-150">説明</span><span class="sxs-lookup"><span data-stu-id="976a5-150">Description</span></span>
|:------------------|:----------------------------|:---------------------------
| <span data-ttu-id="976a5-151">アクティビティ</span><span class="sxs-lookup"><span data-stu-id="976a5-151">activities</span></span>        | <span data-ttu-id="976a5-152">[itemActivity][] コレクション</span><span class="sxs-lookup"><span data-stu-id="976a5-152">[itemActivity][] collection</span></span> | <span data-ttu-id="976a5-153">この**itemactivitの**リソースで表された**itemactivities**を公開します。</span><span class="sxs-lookup"><span data-stu-id="976a5-153">Exposes the **itemActivities** represented in this **itemActivityStat** resource.</span></span>

[itemActivity]: itemactivity.md

## <a name="remarks"></a><span data-ttu-id="976a5-155">備考</span><span class="sxs-lookup"><span data-stu-id="976a5-155">Remarks</span></span>

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
