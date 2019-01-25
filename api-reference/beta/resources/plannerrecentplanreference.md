---
title: plannerRecentPlanReference リソースの種類
description: '**PlannerRecentPlanReference**リソースは、repesents のユーザーが最近閲覧したされている plannerPlan への参照を入力します。 '
localization_priority: Normal
author: TarkanSevilmis
ms.prod: planner
ms.openlocfilehash: 55ccf34055d7d181dbbeecd5b6c30a3843f211d5
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/24/2019
ms.locfileid: "29509162"
---
# <a name="plannerrecentplanreference-resource-type"></a><span data-ttu-id="caa71-103">plannerRecentPlanReference リソースの種類</span><span class="sxs-lookup"><span data-stu-id="caa71-103">plannerRecentPlanReference resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="caa71-104">**PlannerRecentPlanReference**リソースは、repesents のユーザーが最近閲覧したされている[plannerPlan](plannerplan.md)への参照を入力します。</span><span class="sxs-lookup"><span data-stu-id="caa71-104">The **plannerRecentPlanReference** resource type repesents a reference to a [plannerPlan](plannerplan.md) that has recently been viewed by a user.</span></span> <span data-ttu-id="caa71-105">ユーザーの**plannerRecentPlanReferences**は、アプリケーションによって明示的に維持されます。</span><span class="sxs-lookup"><span data-stu-id="caa71-105">The **plannerRecentPlanReferences** for a user are explicitly maintained by apps.</span></span> <span data-ttu-id="caa71-106">ユーザー最後を表示した場合の計画、および更新プログラム**plannerRecentPlanReference**のエントリに応じて、計画の最新の機能を実装する任意のアプリケーションを記録します。</span><span class="sxs-lookup"><span data-stu-id="caa71-106">Any app that implements the recent plans feature should record when the user last viewed a plan, and update **plannerRecentPlanReference** entries accordingly.</span></span>
<span data-ttu-id="caa71-107">アプリケーションでは、 **plannerRecentPlanReference**のエントリが削除する、ユーザーがアクセスできる不要になった、または別のタイトルで更新された**plannerPlans**を参照できるように注意してください。</span><span class="sxs-lookup"><span data-stu-id="caa71-107">Apps should note that **plannerRecentPlanReference** entries can reference **plannerPlans** that are deleted, that the user can no longer access, or that have been updated with a different title.</span></span>
<span data-ttu-id="caa71-108">アプリは不一致がある場合にユーザーに通知し、エントリを常に最新の状態に保つことをお勧めします。</span><span class="sxs-lookup"><span data-stu-id="caa71-108">We recommend that apps notify users when there are discrepancies and keep the entries up to date.</span></span>

## <a name="properties"></a><span data-ttu-id="caa71-109">プロパティ</span><span class="sxs-lookup"><span data-stu-id="caa71-109">Properties</span></span>
| <span data-ttu-id="caa71-110">プロパティ</span><span class="sxs-lookup"><span data-stu-id="caa71-110">Property</span></span>     | <span data-ttu-id="caa71-111">型</span><span class="sxs-lookup"><span data-stu-id="caa71-111">Type</span></span>   |<span data-ttu-id="caa71-112">説明</span><span class="sxs-lookup"><span data-stu-id="caa71-112">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="caa71-113">lastAccessedDateTime</span><span class="sxs-lookup"><span data-stu-id="caa71-113">lastAccessedDateTime</span></span>|<span data-ttu-id="caa71-114">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="caa71-114">DateTimeOffset</span></span>|<span data-ttu-id="caa71-115">日付と時刻計画が、ユーザーが最後に表示します。</span><span class="sxs-lookup"><span data-stu-id="caa71-115">The date and time the plan was last viewed by the user.</span></span> <span data-ttu-id="caa71-116">Timestamp 型は、ISO 8601 形式を使用して日付と時刻の情報を表し、常に UTC 時間です。</span><span class="sxs-lookup"><span data-stu-id="caa71-116">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="caa71-117">たとえば、2014 年 1 月 1 日午前 0 時 (UTC) は、`'2014-01-01T00:00:00Z'` のようになります。</span><span class="sxs-lookup"><span data-stu-id="caa71-117">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`.</span></span>|
|<span data-ttu-id="caa71-118">planTitle</span><span class="sxs-lookup"><span data-stu-id="caa71-118">planTitle</span></span>|<span data-ttu-id="caa71-119">String</span><span class="sxs-lookup"><span data-stu-id="caa71-119">String</span></span>|<span data-ttu-id="caa71-120">時にプランのタイトル ユーザーに表示します。</span><span class="sxs-lookup"><span data-stu-id="caa71-120">The title of the plan at the time the user viewed it.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="caa71-121">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="caa71-121">JSON representation</span></span>

<span data-ttu-id="caa71-122">リソースの JSON 表記を次に示します。</span><span class="sxs-lookup"><span data-stu-id="caa71-122">The following is a JSON representation of the resource.</span></span>

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
  "suppressions": [
    "Error: /api-reference/beta/resources/plannerrecentplanreference.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
