---
author: daspek
ms.author: dspektor
ms.date: 09/14/2017
title: ItemActivityStat
localization_priority: Normal
ms.openlocfilehash: d0917d0100d33abee1095e2a7d06a4732d382937
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/11/2019
ms.locfileid: "27854251"
---
# <a name="itemactivitystat-resource-type"></a><span data-ttu-id="1dd5a-102">itemActivityStat リソースの種類</span><span class="sxs-lookup"><span data-stu-id="1dd5a-102">itemActivityStat resource type</span></span>

> <span data-ttu-id="1dd5a-103">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="1dd5a-103">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="1dd5a-104">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="1dd5a-104">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="1dd5a-105">**ItemActivityStat**リソースでは、時間間隔内で行われた活動についての情報を提供します。</span><span class="sxs-lookup"><span data-stu-id="1dd5a-105">The **itemActivityStat** resource provides information about activities that took place within an interval of time.</span></span>

## <a name="json-representation"></a><span data-ttu-id="1dd5a-106">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="1dd5a-106">JSON representation</span></span>

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

## <a name="properties"></a><span data-ttu-id="1dd5a-107">プロパティ</span><span class="sxs-lookup"><span data-stu-id="1dd5a-107">Properties</span></span>

| <span data-ttu-id="1dd5a-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="1dd5a-108">Property</span></span>         | <span data-ttu-id="1dd5a-109">種類</span><span class="sxs-lookup"><span data-stu-id="1dd5a-109">Type</span></span>                    | <span data-ttu-id="1dd5a-110">説明</span><span class="sxs-lookup"><span data-stu-id="1dd5a-110">Description</span></span>
|:-----------------|:------------------------|:----------------------------------------
| <span data-ttu-id="1dd5a-111">incompleteData</span><span class="sxs-lookup"><span data-stu-id="1dd5a-111">incompleteData</span></span>   | <span data-ttu-id="1dd5a-112">[incompleteData][]</span><span class="sxs-lookup"><span data-stu-id="1dd5a-112">[incompleteData][]</span></span>      | <span data-ttu-id="1dd5a-113">この間隔で統計情報が不完全なデータに基づいていることを示します。</span><span class="sxs-lookup"><span data-stu-id="1dd5a-113">Indicates that the statistics in this interval are based on incomplete data.</span></span> <span data-ttu-id="1dd5a-114">読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="1dd5a-114">Read-only.</span></span>
| <span data-ttu-id="1dd5a-115">isTrending</span><span class="sxs-lookup"><span data-stu-id="1dd5a-115">isTrending</span></span>       | <span data-ttu-id="1dd5a-116">ブール型</span><span class="sxs-lookup"><span data-stu-id="1dd5a-116">Boolean</span></span>                 | <span data-ttu-id="1dd5a-117">かどうか、アイテムは「トレンド。」ことを示します。</span><span class="sxs-lookup"><span data-stu-id="1dd5a-117">Indicates whether the item is "trending."</span></span> <span data-ttu-id="1dd5a-118">読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="1dd5a-118">Read-only.</span></span>
| <span data-ttu-id="1dd5a-119">startDateTime</span><span class="sxs-lookup"><span data-stu-id="1dd5a-119">startDateTime</span></span>    | <span data-ttu-id="1dd5a-120">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="1dd5a-120">DateTimeOffset</span></span>          | <span data-ttu-id="1dd5a-121">間隔の開始時。</span><span class="sxs-lookup"><span data-stu-id="1dd5a-121">When the interval starts.</span></span> <span data-ttu-id="1dd5a-122">読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="1dd5a-122">Read-only.</span></span>
| <span data-ttu-id="1dd5a-123">endDateTime</span><span class="sxs-lookup"><span data-stu-id="1dd5a-123">endDateTime</span></span>      | <span data-ttu-id="1dd5a-124">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="1dd5a-124">DateTimeOffset</span></span>          | <span data-ttu-id="1dd5a-125">間隔が終了します。</span><span class="sxs-lookup"><span data-stu-id="1dd5a-125">When the interval ends.</span></span> <span data-ttu-id="1dd5a-126">読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="1dd5a-126">Read-only.</span></span>
| <span data-ttu-id="1dd5a-127">create</span><span class="sxs-lookup"><span data-stu-id="1dd5a-127">create</span></span>           | <span data-ttu-id="1dd5a-128">[itemActionStat][]</span><span class="sxs-lookup"><span data-stu-id="1dd5a-128">[itemActionStat][]</span></span>      | <span data-ttu-id="1dd5a-129">この間隔内のアクションの**作成**についての統計情報です。</span><span class="sxs-lookup"><span data-stu-id="1dd5a-129">Statistics about the **create** actions in this interval.</span></span> <span data-ttu-id="1dd5a-130">読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="1dd5a-130">Read-only.</span></span>
| <span data-ttu-id="1dd5a-131">edit</span><span class="sxs-lookup"><span data-stu-id="1dd5a-131">edit</span></span>             | <span data-ttu-id="1dd5a-132">[itemActionStat][]</span><span class="sxs-lookup"><span data-stu-id="1dd5a-132">[itemActionStat][]</span></span>      | <span data-ttu-id="1dd5a-133">この範囲の**編集**処理に関する統計情報です。</span><span class="sxs-lookup"><span data-stu-id="1dd5a-133">Statistics about the **edit** actions in this interval.</span></span> <span data-ttu-id="1dd5a-134">読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="1dd5a-134">Read-only.</span></span>
| <span data-ttu-id="1dd5a-135">delete</span><span class="sxs-lookup"><span data-stu-id="1dd5a-135">delete</span></span>           | <span data-ttu-id="1dd5a-136">[itemActionStat][]</span><span class="sxs-lookup"><span data-stu-id="1dd5a-136">[itemActionStat][]</span></span>      | <span data-ttu-id="1dd5a-137">この間隔で**削除**の操作に関する統計情報です。</span><span class="sxs-lookup"><span data-stu-id="1dd5a-137">Statistics about the **delete** actions in this interval.</span></span> <span data-ttu-id="1dd5a-138">読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="1dd5a-138">Read-only.</span></span>
| <span data-ttu-id="1dd5a-139">move</span><span class="sxs-lookup"><span data-stu-id="1dd5a-139">move</span></span>             | <span data-ttu-id="1dd5a-140">[itemActionStat][]</span><span class="sxs-lookup"><span data-stu-id="1dd5a-140">[itemActionStat][]</span></span>      | <span data-ttu-id="1dd5a-141">この間隔内の**移動**操作に関する統計情報です。</span><span class="sxs-lookup"><span data-stu-id="1dd5a-141">Statistics about the **move** actions in this interval.</span></span> <span data-ttu-id="1dd5a-142">読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="1dd5a-142">Read-only.</span></span>
| <span data-ttu-id="1dd5a-143">アクセス</span><span class="sxs-lookup"><span data-stu-id="1dd5a-143">access</span></span>           | <span data-ttu-id="1dd5a-144">[itemActionStat][]</span><span class="sxs-lookup"><span data-stu-id="1dd5a-144">[itemActionStat][]</span></span>      | <span data-ttu-id="1dd5a-145">この間隔で**のアクセス**の操作に関する統計情報です。</span><span class="sxs-lookup"><span data-stu-id="1dd5a-145">Statistics about the **access** actions in this interval.</span></span> <span data-ttu-id="1dd5a-146">読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="1dd5a-146">Read-only.</span></span>

[itemActionStat]: itemactionstat.md
[incompleteData]: incompletedata.md

## <a name="relationships"></a><span data-ttu-id="1dd5a-149">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="1dd5a-149">Relationships</span></span>

| <span data-ttu-id="1dd5a-150">リレーションシップ名</span><span class="sxs-lookup"><span data-stu-id="1dd5a-150">Relationship name</span></span> | <span data-ttu-id="1dd5a-151">種類</span><span class="sxs-lookup"><span data-stu-id="1dd5a-151">Type</span></span>                        | <span data-ttu-id="1dd5a-152">説明</span><span class="sxs-lookup"><span data-stu-id="1dd5a-152">Description</span></span>
|:------------------|:----------------------------|:---------------------------
| <span data-ttu-id="1dd5a-153">アクティビティ</span><span class="sxs-lookup"><span data-stu-id="1dd5a-153">activities</span></span>        | <span data-ttu-id="1dd5a-154">[itemActivity][] コレクション</span><span class="sxs-lookup"><span data-stu-id="1dd5a-154">[itemActivity][] collection</span></span> | <span data-ttu-id="1dd5a-155">この**itemActivityStat**リソースで表される**itemActivities**を公開します。</span><span class="sxs-lookup"><span data-stu-id="1dd5a-155">Exposes the **itemActivities** represented in this **itemActivityStat** resource.</span></span>

[itemActivity]: itemactivity.md

## <a name="remarks"></a><span data-ttu-id="1dd5a-157">解説</span><span class="sxs-lookup"><span data-stu-id="1dd5a-157">Remarks</span></span>

<!-- {
  "type": "#page.annotation",
  "description": "The ItemActivityStat object provides information about activities that took place on an item.",
  "keywords": "activities,activity,action,analytics",
  "section": "documentation",
  "tocPath": "Resources/ItemActivityStat"
} -->
