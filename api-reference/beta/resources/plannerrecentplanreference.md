---
title: plannerRecentPlanReference リソースの種類
description: '**PlannerRecentPlanReference**リソースは、repesents のユーザーが最近閲覧したされている plannerPlan への参照を入力します。 '
ms.openlocfilehash: ac774ffbf7ebdfe45211cf50c2ce065921de30f1
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27067198"
---
# <a name="plannerrecentplanreference-resource-type"></a><span data-ttu-id="4f28b-103">plannerRecentPlanReference リソースの種類</span><span class="sxs-lookup"><span data-stu-id="4f28b-103">plannerRecentPlanReference resource type</span></span>

> <span data-ttu-id="4f28b-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="4f28b-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="4f28b-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="4f28b-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="4f28b-106">**PlannerRecentPlanReference**リソースは、repesents のユーザーが最近閲覧したされている[plannerPlan](plannerplan.md)への参照を入力します。</span><span class="sxs-lookup"><span data-stu-id="4f28b-106">The **plannerRecentPlanReference** resource type repesents a reference to a [plannerPlan](plannerplan.md) that has recently been viewed by a user.</span></span> <span data-ttu-id="4f28b-107">ユーザーの**plannerRecentPlanReferences**は、アプリケーションによって明示的に維持されます。</span><span class="sxs-lookup"><span data-stu-id="4f28b-107">The **plannerRecentPlanReferences** for a user are explicitly maintained by apps.</span></span> <span data-ttu-id="4f28b-108">ユーザー最後を表示した場合の計画、および更新プログラム**plannerRecentPlanReference**のエントリに応じて、計画の最新の機能を実装する任意のアプリケーションを記録します。</span><span class="sxs-lookup"><span data-stu-id="4f28b-108">Any app that implements the recent plans feature should record when the user last viewed a plan, and update **plannerRecentPlanReference** entries accordingly.</span></span>
<span data-ttu-id="4f28b-109">アプリケーションでは、 **plannerRecentPlanReference**のエントリが削除する、ユーザーがアクセスできる不要になった、または別のタイトルで更新された**plannerPlans**を参照できるように注意してください。</span><span class="sxs-lookup"><span data-stu-id="4f28b-109">Apps should note that **plannerRecentPlanReference** entries can reference **plannerPlans** that are deleted, that the user can no longer access, or that have been updated with a different title.</span></span>
<span data-ttu-id="4f28b-110">アプリは不一致がある場合にユーザーに通知し、エントリを常に最新の状態に保つことをお勧めします。</span><span class="sxs-lookup"><span data-stu-id="4f28b-110">We recommend that apps notify users when there are discrepancies and keep the entries up to date.</span></span>

## <a name="properties"></a><span data-ttu-id="4f28b-111">プロパティ</span><span class="sxs-lookup"><span data-stu-id="4f28b-111">Properties</span></span>
| <span data-ttu-id="4f28b-112">プロパティ</span><span class="sxs-lookup"><span data-stu-id="4f28b-112">Property</span></span>     | <span data-ttu-id="4f28b-113">型</span><span class="sxs-lookup"><span data-stu-id="4f28b-113">Type</span></span>   |<span data-ttu-id="4f28b-114">説明</span><span class="sxs-lookup"><span data-stu-id="4f28b-114">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="4f28b-115">lastAccessedDateTime</span><span class="sxs-lookup"><span data-stu-id="4f28b-115">lastAccessedDateTime</span></span>|<span data-ttu-id="4f28b-116">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="4f28b-116">DateTimeOffset</span></span>|<span data-ttu-id="4f28b-117">日付と時刻計画が、ユーザーが最後に表示します。</span><span class="sxs-lookup"><span data-stu-id="4f28b-117">The date and time the plan was last viewed by the user.</span></span> <span data-ttu-id="4f28b-118">Timestamp 型は、ISO 8601 形式を使用して日付と時刻の情報を表し、常に UTC 時間です。</span><span class="sxs-lookup"><span data-stu-id="4f28b-118">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="4f28b-119">たとえば、2014 年 1 月 1 日午前 0 時 (UTC) は、次のようになります。`'2014-01-01T00:00:00Z'`</span><span class="sxs-lookup"><span data-stu-id="4f28b-119">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`.</span></span>|
|<span data-ttu-id="4f28b-120">planTitle</span><span class="sxs-lookup"><span data-stu-id="4f28b-120">planTitle</span></span>|<span data-ttu-id="4f28b-121">String</span><span class="sxs-lookup"><span data-stu-id="4f28b-121">String</span></span>|<span data-ttu-id="4f28b-122">時にプランのタイトル ユーザーに表示します。</span><span class="sxs-lookup"><span data-stu-id="4f28b-122">The title of the plan at the time the user viewed it.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="4f28b-123">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="4f28b-123">JSON representation</span></span>

<span data-ttu-id="4f28b-124">リソースの JSON 表記を次に示します。</span><span class="sxs-lookup"><span data-stu-id="4f28b-124">The following is a JSON representation of the resource.</span></span>

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
