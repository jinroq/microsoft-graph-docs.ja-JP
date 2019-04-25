---
author: daspek
ms.author: dspektor
ms.date: 09/14/2017
title: itemactiv
localization_priority: Normal
ms.openlocfilehash: 1362116c0dbe997eda941cb790e00e9ddb078ae4
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32561909"
---
# <a name="itemactivitystat-resource-type"></a><span data-ttu-id="f764d-102">リソースの種類での itemactiv</span><span class="sxs-lookup"><span data-stu-id="f764d-102">itemActivityStat resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="f764d-103">**itemactivit(** リソース) は、ある期間内に発生したアクティビティに関する情報を提供します。</span><span class="sxs-lookup"><span data-stu-id="f764d-103">The **itemActivityStat** resource provides information about activities that took place within an interval of time.</span></span>

## <a name="json-representation"></a><span data-ttu-id="f764d-104">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="f764d-104">JSON representation</span></span>

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

## <a name="properties"></a><span data-ttu-id="f764d-105">プロパティ</span><span class="sxs-lookup"><span data-stu-id="f764d-105">Properties</span></span>

| <span data-ttu-id="f764d-106">プロパティ</span><span class="sxs-lookup"><span data-stu-id="f764d-106">Property</span></span>         | <span data-ttu-id="f764d-107">型</span><span class="sxs-lookup"><span data-stu-id="f764d-107">Type</span></span>                    | <span data-ttu-id="f764d-108">説明</span><span class="sxs-lookup"><span data-stu-id="f764d-108">Description</span></span>
|:-----------------|:------------------------|:----------------------------------------
| <span data-ttu-id="f764d-109">incompletedata</span><span class="sxs-lookup"><span data-stu-id="f764d-109">incompleteData</span></span>   | <span data-ttu-id="f764d-110">[incompletedata][]</span><span class="sxs-lookup"><span data-stu-id="f764d-110">[incompleteData][]</span></span>      | <span data-ttu-id="f764d-111">この間隔の統計情報が不完全なデータに基づくことを示します。</span><span class="sxs-lookup"><span data-stu-id="f764d-111">Indicates that the statistics in this interval are based on incomplete data.</span></span> <span data-ttu-id="f764d-112">読み取り専用。</span><span class="sxs-lookup"><span data-stu-id="f764d-112">Read-only.</span></span>
| <span data-ttu-id="f764d-113">istrending</span><span class="sxs-lookup"><span data-stu-id="f764d-113">isTrending</span></span>       | <span data-ttu-id="f764d-114">Boolean</span><span class="sxs-lookup"><span data-stu-id="f764d-114">Boolean</span></span>                 | <span data-ttu-id="f764d-115">アイテムが "傾向" であるかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="f764d-115">Indicates whether the item is "trending."</span></span> <span data-ttu-id="f764d-116">読み取り専用。</span><span class="sxs-lookup"><span data-stu-id="f764d-116">Read-only.</span></span>
| <span data-ttu-id="f764d-117">startDateTime</span><span class="sxs-lookup"><span data-stu-id="f764d-117">startDateTime</span></span>    | <span data-ttu-id="f764d-118">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="f764d-118">DateTimeOffset</span></span>          | <span data-ttu-id="f764d-119">間隔が開始されたとき。</span><span class="sxs-lookup"><span data-stu-id="f764d-119">When the interval starts.</span></span> <span data-ttu-id="f764d-120">読み取り専用。</span><span class="sxs-lookup"><span data-stu-id="f764d-120">Read-only.</span></span>
| <span data-ttu-id="f764d-121">endDateTime</span><span class="sxs-lookup"><span data-stu-id="f764d-121">endDateTime</span></span>      | <span data-ttu-id="f764d-122">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="f764d-122">DateTimeOffset</span></span>          | <span data-ttu-id="f764d-123">間隔が終了したとき。</span><span class="sxs-lookup"><span data-stu-id="f764d-123">When the interval ends.</span></span> <span data-ttu-id="f764d-124">読み取り専用。</span><span class="sxs-lookup"><span data-stu-id="f764d-124">Read-only.</span></span>
| <span data-ttu-id="f764d-125">create</span><span class="sxs-lookup"><span data-stu-id="f764d-125">create</span></span>           | <span data-ttu-id="f764d-126">[itemactionstat][]</span><span class="sxs-lookup"><span data-stu-id="f764d-126">[itemActionStat][]</span></span>      | <span data-ttu-id="f764d-127">この間隔における**create**アクションに関する統計。</span><span class="sxs-lookup"><span data-stu-id="f764d-127">Statistics about the **create** actions in this interval.</span></span> <span data-ttu-id="f764d-128">読み取り専用。</span><span class="sxs-lookup"><span data-stu-id="f764d-128">Read-only.</span></span>
| <span data-ttu-id="f764d-129">edit</span><span class="sxs-lookup"><span data-stu-id="f764d-129">edit</span></span>             | <span data-ttu-id="f764d-130">[itemactionstat][]</span><span class="sxs-lookup"><span data-stu-id="f764d-130">[itemActionStat][]</span></span>      | <span data-ttu-id="f764d-131">この間隔の**編集**アクションに関する統計。</span><span class="sxs-lookup"><span data-stu-id="f764d-131">Statistics about the **edit** actions in this interval.</span></span> <span data-ttu-id="f764d-132">読み取り専用。</span><span class="sxs-lookup"><span data-stu-id="f764d-132">Read-only.</span></span>
| <span data-ttu-id="f764d-133">delete</span><span class="sxs-lookup"><span data-stu-id="f764d-133">delete</span></span>           | <span data-ttu-id="f764d-134">[itemactionstat][]</span><span class="sxs-lookup"><span data-stu-id="f764d-134">[itemActionStat][]</span></span>      | <span data-ttu-id="f764d-135">この間隔の**削除**アクションに関する統計情報。</span><span class="sxs-lookup"><span data-stu-id="f764d-135">Statistics about the **delete** actions in this interval.</span></span> <span data-ttu-id="f764d-136">読み取り専用。</span><span class="sxs-lookup"><span data-stu-id="f764d-136">Read-only.</span></span>
| <span data-ttu-id="f764d-137">move</span><span class="sxs-lookup"><span data-stu-id="f764d-137">move</span></span>             | <span data-ttu-id="f764d-138">[itemactionstat][]</span><span class="sxs-lookup"><span data-stu-id="f764d-138">[itemActionStat][]</span></span>      | <span data-ttu-id="f764d-139">この間隔における**移動**アクションに関する統計。</span><span class="sxs-lookup"><span data-stu-id="f764d-139">Statistics about the **move** actions in this interval.</span></span> <span data-ttu-id="f764d-140">読み取り専用。</span><span class="sxs-lookup"><span data-stu-id="f764d-140">Read-only.</span></span>
| <span data-ttu-id="f764d-141">接続</span><span class="sxs-lookup"><span data-stu-id="f764d-141">access</span></span>           | <span data-ttu-id="f764d-142">[itemactionstat][]</span><span class="sxs-lookup"><span data-stu-id="f764d-142">[itemActionStat][]</span></span>      | <span data-ttu-id="f764d-143">この間隔における**アクセス**アクションに関する統計情報。</span><span class="sxs-lookup"><span data-stu-id="f764d-143">Statistics about the **access** actions in this interval.</span></span> <span data-ttu-id="f764d-144">読み取り専用。</span><span class="sxs-lookup"><span data-stu-id="f764d-144">Read-only.</span></span>

[itemactionstat]: itemactionstat.md
[itemActionStat]: itemactionstat.md
[incompletedata]: incompletedata.md
[incompleteData]: incompletedata.md

## <a name="relationships"></a><span data-ttu-id="f764d-147">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="f764d-147">Relationships</span></span>

| <span data-ttu-id="f764d-148">リレーションシップ名</span><span class="sxs-lookup"><span data-stu-id="f764d-148">Relationship name</span></span> | <span data-ttu-id="f764d-149">種類</span><span class="sxs-lookup"><span data-stu-id="f764d-149">Type</span></span>                        | <span data-ttu-id="f764d-150">説明</span><span class="sxs-lookup"><span data-stu-id="f764d-150">Description</span></span>
|:------------------|:----------------------------|:---------------------------
| <span data-ttu-id="f764d-151">アクティビティ</span><span class="sxs-lookup"><span data-stu-id="f764d-151">activities</span></span>        | <span data-ttu-id="f764d-152">[itemActivity][] コレクション</span><span class="sxs-lookup"><span data-stu-id="f764d-152">[itemActivity][] collection</span></span> | <span data-ttu-id="f764d-153">この**itemactivitの**リソースで表された**itemactivities**を公開します。</span><span class="sxs-lookup"><span data-stu-id="f764d-153">Exposes the **itemActivities** represented in this **itemActivityStat** resource.</span></span>

[itemActivity]: itemactivity.md

## <a name="remarks"></a><span data-ttu-id="f764d-155">備考</span><span class="sxs-lookup"><span data-stu-id="f764d-155">Remarks</span></span>

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
