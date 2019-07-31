---
title: plannerRecentPlanReference リソースの種類
description: '**PlannerRecentPlanReference**リソースの種類表す workbookconnection は、ユーザーが最近表示した plan プランへの参照を示します。 '
localization_priority: Normal
author: TarkanSevilmis
ms.prod: planner
doc_type: resourcePageType
ms.openlocfilehash: 8439502aa1214e1ef2bbedd9864ef4724abf8021
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "35965867"
---
# <a name="plannerrecentplanreference-resource-type"></a><span data-ttu-id="209c2-103">plannerRecentPlanReference リソースの種類</span><span class="sxs-lookup"><span data-stu-id="209c2-103">plannerRecentPlanReference resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="209c2-104">**PlannerRecentPlanReference**リソースの種類表す workbookconnection は、ユーザーが最近表示した[plan プラン](plannerplan.md)への参照を示します。</span><span class="sxs-lookup"><span data-stu-id="209c2-104">The **plannerRecentPlanReference** resource type repesents a reference to a [plannerPlan](plannerplan.md) that has recently been viewed by a user.</span></span> <span data-ttu-id="209c2-105">ユーザーの**plannerRecentPlanReferences**は、アプリによって明示的に管理されます。</span><span class="sxs-lookup"><span data-stu-id="209c2-105">The **plannerRecentPlanReferences** for a user are explicitly maintained by apps.</span></span> <span data-ttu-id="209c2-106">最近のプランを実装するすべてのアプリは、ユーザーが前回プランを表示したときに記録し、それに応じて**plannerRecentPlanReference**エントリを更新する必要があります。</span><span class="sxs-lookup"><span data-stu-id="209c2-106">Any app that implements the recent plans feature should record when the user last viewed a plan, and update **plannerRecentPlanReference** entries accordingly.</span></span>
<span data-ttu-id="209c2-107">**PlannerRecentPlanReference**エントリは、削除された**プラン**、ユーザーがアクセスできなくなったプラン、または別のタイトルで更新されたプランを参照できることに注意してください。</span><span class="sxs-lookup"><span data-stu-id="209c2-107">Apps should note that **plannerRecentPlanReference** entries can reference **plannerPlans** that are deleted, that the user can no longer access, or that have been updated with a different title.</span></span>
<span data-ttu-id="209c2-108">アプリでは、相違点がある場合にユーザーに通知し、エントリを最新の状態に保つことをお勧めします。</span><span class="sxs-lookup"><span data-stu-id="209c2-108">We recommend that apps notify users when there are discrepancies and keep the entries up to date.</span></span>

## <a name="properties"></a><span data-ttu-id="209c2-109">プロパティ</span><span class="sxs-lookup"><span data-stu-id="209c2-109">Properties</span></span>
| <span data-ttu-id="209c2-110">プロパティ</span><span class="sxs-lookup"><span data-stu-id="209c2-110">Property</span></span>     | <span data-ttu-id="209c2-111">型</span><span class="sxs-lookup"><span data-stu-id="209c2-111">Type</span></span>   |<span data-ttu-id="209c2-112">説明</span><span class="sxs-lookup"><span data-stu-id="209c2-112">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="209c2-113">lastAccessedDateTime</span><span class="sxs-lookup"><span data-stu-id="209c2-113">lastAccessedDateTime</span></span>|<span data-ttu-id="209c2-114">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="209c2-114">DateTimeOffset</span></span>|<span data-ttu-id="209c2-115">プランが最後にユーザーによって表示された日時。</span><span class="sxs-lookup"><span data-stu-id="209c2-115">The date and time the plan was last viewed by the user.</span></span> <span data-ttu-id="209c2-116">Timestamp 型は、ISO 8601 形式を使用して日付と時刻の情報を表します。これは常に UTC 時間です。</span><span class="sxs-lookup"><span data-stu-id="209c2-116">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="209c2-117">たとえば、2014 年 1 月 1 日午前 0 時 (UTC) は、次のようになります。`'2014-01-01T00:00:00Z'`</span><span class="sxs-lookup"><span data-stu-id="209c2-117">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`.</span></span>|
|<span data-ttu-id="209c2-118">プランのタイトル</span><span class="sxs-lookup"><span data-stu-id="209c2-118">planTitle</span></span>|<span data-ttu-id="209c2-119">String</span><span class="sxs-lookup"><span data-stu-id="209c2-119">String</span></span>|<span data-ttu-id="209c2-120">ユーザーが表示したときのプランのタイトル。</span><span class="sxs-lookup"><span data-stu-id="209c2-120">The title of the plan at the time the user viewed it.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="209c2-121">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="209c2-121">JSON representation</span></span>

<span data-ttu-id="209c2-122">リソースの JSON 表記を次に示します。</span><span class="sxs-lookup"><span data-stu-id="209c2-122">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.plannerRecentPlanReference"
}-->

```json
{
  "lastAccessedDateTime": "String (timestamp)",
  "planTitle": "String"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "plannerRecentPlanReference resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
