---
title: plannerRecentPlanReference リソースの種類
description: '**PlannerRecentPlanReference**リソースは、repesents のユーザーが最近閲覧したされている plannerPlan への参照を入力します。 '
localization_priority: Normal
ms.openlocfilehash: 6ac17cd0a99d384cbc1f42e2e0d243c582204101
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/11/2019
ms.locfileid: "27805678"
---
# <a name="plannerrecentplanreference-resource-type"></a><span data-ttu-id="2f7d6-103">plannerRecentPlanReference リソースの種類</span><span class="sxs-lookup"><span data-stu-id="2f7d6-103">plannerRecentPlanReference resource type</span></span>

> <span data-ttu-id="2f7d6-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="2f7d6-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="2f7d6-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="2f7d6-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="2f7d6-106">**PlannerRecentPlanReference**リソースは、repesents のユーザーが最近閲覧したされている[plannerPlan](plannerplan.md)への参照を入力します。</span><span class="sxs-lookup"><span data-stu-id="2f7d6-106">The **plannerRecentPlanReference** resource type repesents a reference to a [plannerPlan](plannerplan.md) that has recently been viewed by a user.</span></span> <span data-ttu-id="2f7d6-107">ユーザーの**plannerRecentPlanReferences**は、アプリケーションによって明示的に維持されます。</span><span class="sxs-lookup"><span data-stu-id="2f7d6-107">The **plannerRecentPlanReferences** for a user are explicitly maintained by apps.</span></span> <span data-ttu-id="2f7d6-108">ユーザー最後を表示した場合の計画、および更新プログラム**plannerRecentPlanReference**のエントリに応じて、計画の最新の機能を実装する任意のアプリケーションを記録します。</span><span class="sxs-lookup"><span data-stu-id="2f7d6-108">Any app that implements the recent plans feature should record when the user last viewed a plan, and update **plannerRecentPlanReference** entries accordingly.</span></span>
<span data-ttu-id="2f7d6-109">アプリケーションでは、 **plannerRecentPlanReference**のエントリが削除する、ユーザーがアクセスできる不要になった、または別のタイトルで更新された**plannerPlans**を参照できるように注意してください。</span><span class="sxs-lookup"><span data-stu-id="2f7d6-109">Apps should note that **plannerRecentPlanReference** entries can reference **plannerPlans** that are deleted, that the user can no longer access, or that have been updated with a different title.</span></span>
<span data-ttu-id="2f7d6-110">アプリは不一致がある場合にユーザーに通知し、エントリを常に最新の状態に保つことをお勧めします。</span><span class="sxs-lookup"><span data-stu-id="2f7d6-110">We recommend that apps notify users when there are discrepancies and keep the entries up to date.</span></span>

## <a name="properties"></a><span data-ttu-id="2f7d6-111">プロパティ</span><span class="sxs-lookup"><span data-stu-id="2f7d6-111">Properties</span></span>
| <span data-ttu-id="2f7d6-112">プロパティ</span><span class="sxs-lookup"><span data-stu-id="2f7d6-112">Property</span></span>     | <span data-ttu-id="2f7d6-113">種類</span><span class="sxs-lookup"><span data-stu-id="2f7d6-113">Type</span></span>   |<span data-ttu-id="2f7d6-114">説明</span><span class="sxs-lookup"><span data-stu-id="2f7d6-114">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="2f7d6-115">lastAccessedDateTime</span><span class="sxs-lookup"><span data-stu-id="2f7d6-115">lastAccessedDateTime</span></span>|<span data-ttu-id="2f7d6-116">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="2f7d6-116">DateTimeOffset</span></span>|<span data-ttu-id="2f7d6-117">日付と時刻計画が、ユーザーが最後に表示します。</span><span class="sxs-lookup"><span data-stu-id="2f7d6-117">The date and time the plan was last viewed by the user.</span></span> <span data-ttu-id="2f7d6-118">Timestamp 型は、ISO 8601 形式を使用して日付と時刻の情報を表し、常に UTC 時間です。</span><span class="sxs-lookup"><span data-stu-id="2f7d6-118">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="2f7d6-119">たとえば、2014 年 1 月 1 日午前 0 時 (UTC) は、次のようになります。`'2014-01-01T00:00:00Z'`</span><span class="sxs-lookup"><span data-stu-id="2f7d6-119">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`.</span></span>|
|<span data-ttu-id="2f7d6-120">planTitle</span><span class="sxs-lookup"><span data-stu-id="2f7d6-120">planTitle</span></span>|<span data-ttu-id="2f7d6-121">String</span><span class="sxs-lookup"><span data-stu-id="2f7d6-121">String</span></span>|<span data-ttu-id="2f7d6-122">時にプランのタイトル ユーザーに表示します。</span><span class="sxs-lookup"><span data-stu-id="2f7d6-122">The title of the plan at the time the user viewed it.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="2f7d6-123">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="2f7d6-123">JSON representation</span></span>

<span data-ttu-id="2f7d6-124">リソースの JSON 表記を次に示します。</span><span class="sxs-lookup"><span data-stu-id="2f7d6-124">The following is a JSON representation of the resource.</span></span>

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
<!-- {
  "type": "#page.annotation",
  "description": "plannerRecentPlanReference resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
