---
author: daspek
ms.author: dspektor
ms.date: 09/14/2017
title: ItemActivityStat
localization_priority: Normal
ms.openlocfilehash: 1362116c0dbe997eda941cb790e00e9ddb078ae4
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/24/2019
ms.locfileid: "29517632"
---
# <a name="itemactivitystat-resource-type"></a><span data-ttu-id="d4e10-102">itemActivityStat リソースの種類</span><span class="sxs-lookup"><span data-stu-id="d4e10-102">itemActivityStat resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="d4e10-103">**ItemActivityStat**リソースでは、時間間隔内で行われた活動についての情報を提供します。</span><span class="sxs-lookup"><span data-stu-id="d4e10-103">The **itemActivityStat** resource provides information about activities that took place within an interval of time.</span></span>

## <a name="json-representation"></a><span data-ttu-id="d4e10-104">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="d4e10-104">JSON representation</span></span>

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

## <a name="properties"></a><span data-ttu-id="d4e10-105">プロパティ</span><span class="sxs-lookup"><span data-stu-id="d4e10-105">Properties</span></span>

| <span data-ttu-id="d4e10-106">プロパティ</span><span class="sxs-lookup"><span data-stu-id="d4e10-106">Property</span></span>         | <span data-ttu-id="d4e10-107">型</span><span class="sxs-lookup"><span data-stu-id="d4e10-107">Type</span></span>                    | <span data-ttu-id="d4e10-108">説明</span><span class="sxs-lookup"><span data-stu-id="d4e10-108">Description</span></span>
|:-----------------|:------------------------|:----------------------------------------
| <span data-ttu-id="d4e10-109">incompleteData</span><span class="sxs-lookup"><span data-stu-id="d4e10-109">incompleteData</span></span>   | <span data-ttu-id="d4e10-110">[incompleteData][]</span><span class="sxs-lookup"><span data-stu-id="d4e10-110">[incompleteData][]</span></span>      | <span data-ttu-id="d4e10-111">この間隔で統計情報が不完全なデータに基づいていることを示します。</span><span class="sxs-lookup"><span data-stu-id="d4e10-111">Indicates that the statistics in this interval are based on incomplete data.</span></span> <span data-ttu-id="d4e10-112">読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="d4e10-112">Read-only.</span></span>
| <span data-ttu-id="d4e10-113">isTrending</span><span class="sxs-lookup"><span data-stu-id="d4e10-113">isTrending</span></span>       | <span data-ttu-id="d4e10-114">ブール値</span><span class="sxs-lookup"><span data-stu-id="d4e10-114">Boolean</span></span>                 | <span data-ttu-id="d4e10-115">かどうか、アイテムは「トレンド。」ことを示します。</span><span class="sxs-lookup"><span data-stu-id="d4e10-115">Indicates whether the item is "trending."</span></span> <span data-ttu-id="d4e10-116">読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="d4e10-116">Read-only.</span></span>
| <span data-ttu-id="d4e10-117">startDateTime</span><span class="sxs-lookup"><span data-stu-id="d4e10-117">startDateTime</span></span>    | <span data-ttu-id="d4e10-118">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="d4e10-118">DateTimeOffset</span></span>          | <span data-ttu-id="d4e10-119">間隔の開始時。</span><span class="sxs-lookup"><span data-stu-id="d4e10-119">When the interval starts.</span></span> <span data-ttu-id="d4e10-120">読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="d4e10-120">Read-only.</span></span>
| <span data-ttu-id="d4e10-121">endDateTime</span><span class="sxs-lookup"><span data-stu-id="d4e10-121">endDateTime</span></span>      | <span data-ttu-id="d4e10-122">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="d4e10-122">DateTimeOffset</span></span>          | <span data-ttu-id="d4e10-123">間隔が終了します。</span><span class="sxs-lookup"><span data-stu-id="d4e10-123">When the interval ends.</span></span> <span data-ttu-id="d4e10-124">読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="d4e10-124">Read-only.</span></span>
| <span data-ttu-id="d4e10-125">create</span><span class="sxs-lookup"><span data-stu-id="d4e10-125">create</span></span>           | <span data-ttu-id="d4e10-126">[itemActionStat][]</span><span class="sxs-lookup"><span data-stu-id="d4e10-126">[itemActionStat][]</span></span>      | <span data-ttu-id="d4e10-127">この間隔内のアクションの**作成**についての統計情報です。</span><span class="sxs-lookup"><span data-stu-id="d4e10-127">Statistics about the **create** actions in this interval.</span></span> <span data-ttu-id="d4e10-128">読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="d4e10-128">Read-only.</span></span>
| <span data-ttu-id="d4e10-129">edit</span><span class="sxs-lookup"><span data-stu-id="d4e10-129">edit</span></span>             | <span data-ttu-id="d4e10-130">[itemActionStat][]</span><span class="sxs-lookup"><span data-stu-id="d4e10-130">[itemActionStat][]</span></span>      | <span data-ttu-id="d4e10-131">この範囲の**編集**処理に関する統計情報です。</span><span class="sxs-lookup"><span data-stu-id="d4e10-131">Statistics about the **edit** actions in this interval.</span></span> <span data-ttu-id="d4e10-132">読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="d4e10-132">Read-only.</span></span>
| <span data-ttu-id="d4e10-133">delete</span><span class="sxs-lookup"><span data-stu-id="d4e10-133">delete</span></span>           | <span data-ttu-id="d4e10-134">[itemActionStat][]</span><span class="sxs-lookup"><span data-stu-id="d4e10-134">[itemActionStat][]</span></span>      | <span data-ttu-id="d4e10-135">この間隔で**削除**の操作に関する統計情報です。</span><span class="sxs-lookup"><span data-stu-id="d4e10-135">Statistics about the **delete** actions in this interval.</span></span> <span data-ttu-id="d4e10-136">読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="d4e10-136">Read-only.</span></span>
| <span data-ttu-id="d4e10-137">move</span><span class="sxs-lookup"><span data-stu-id="d4e10-137">move</span></span>             | <span data-ttu-id="d4e10-138">[itemActionStat][]</span><span class="sxs-lookup"><span data-stu-id="d4e10-138">[itemActionStat][]</span></span>      | <span data-ttu-id="d4e10-139">この間隔内の**移動**操作に関する統計情報です。</span><span class="sxs-lookup"><span data-stu-id="d4e10-139">Statistics about the **move** actions in this interval.</span></span> <span data-ttu-id="d4e10-140">読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="d4e10-140">Read-only.</span></span>
| <span data-ttu-id="d4e10-141">Access</span><span class="sxs-lookup"><span data-stu-id="d4e10-141">access</span></span>           | <span data-ttu-id="d4e10-142">[itemActionStat][]</span><span class="sxs-lookup"><span data-stu-id="d4e10-142">[itemActionStat][]</span></span>      | <span data-ttu-id="d4e10-143">この間隔で**のアクセス**の操作に関する統計情報です。</span><span class="sxs-lookup"><span data-stu-id="d4e10-143">Statistics about the **access** actions in this interval.</span></span> <span data-ttu-id="d4e10-144">読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="d4e10-144">Read-only.</span></span>

[itemActionStat]: itemactionstat.md
[incompleteData]: incompletedata.md

## <a name="relationships"></a><span data-ttu-id="d4e10-147">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="d4e10-147">Relationships</span></span>

| <span data-ttu-id="d4e10-148">リレーションシップ名</span><span class="sxs-lookup"><span data-stu-id="d4e10-148">Relationship name</span></span> | <span data-ttu-id="d4e10-149">種類</span><span class="sxs-lookup"><span data-stu-id="d4e10-149">Type</span></span>                        | <span data-ttu-id="d4e10-150">説明</span><span class="sxs-lookup"><span data-stu-id="d4e10-150">Description</span></span>
|:------------------|:----------------------------|:---------------------------
| <span data-ttu-id="d4e10-151">アクティビティ</span><span class="sxs-lookup"><span data-stu-id="d4e10-151">activities</span></span>        | <span data-ttu-id="d4e10-152">[itemActivity][] コレクション</span><span class="sxs-lookup"><span data-stu-id="d4e10-152">[itemActivity][] collection</span></span> | <span data-ttu-id="d4e10-153">この**itemActivityStat**リソースで表される**itemActivities**を公開します。</span><span class="sxs-lookup"><span data-stu-id="d4e10-153">Exposes the **itemActivities** represented in this **itemActivityStat** resource.</span></span>

[itemActivity]: itemactivity.md

## <a name="remarks"></a><span data-ttu-id="d4e10-155">解説</span><span class="sxs-lookup"><span data-stu-id="d4e10-155">Remarks</span></span>

<!--
{
  "type": "#page.annotation",
  "description": "The ItemActivityStat object provides information about activities that took place on an item.",
  "keywords": "activities,activity,action,analytics",
  "section": "documentation",
  "tocPath": "Resources/ItemActivityStat",
  "suppressions": [
    "Error: /api-reference/beta/resources/itemactivitystat.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
