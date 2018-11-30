---
title: plannerPlanContext リソースの種類
description: '**PlannerPlanContext**リソースでは、プランナーの外部のユーザー エクスペリエンスの plannerPlan との関係を表します。 プランナーでプランは、その経験のコンテキストで作業を追跡するために、マイクロソフトのチームなど、他の経験で提示されることができます。'
ms.openlocfilehash: 84512c03081a3e1fd2b15456c64cecf3f9c39435
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27070633"
---
# <a name="plannerplancontext-resource-type"></a><span data-ttu-id="a2f24-104">plannerPlanContext リソースの種類</span><span class="sxs-lookup"><span data-stu-id="a2f24-104">plannerPlanContext resource type</span></span>

> <span data-ttu-id="a2f24-105">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="a2f24-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="a2f24-106">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="a2f24-106">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="a2f24-107">**PlannerPlanContext**リソースでは、計画外のユーザー エクスペリエンスには、 [plannerPlan](plannerplan.md)との関係を表します。</span><span class="sxs-lookup"><span data-stu-id="a2f24-107">The **plannerPlanContext** resource represents the relationship of a [plannerPlan](plannerplan.md) to a user experience outside of Planner.</span></span> <span data-ttu-id="a2f24-108">プランナーでプランは、その経験のコンテキストで作業を追跡するために、マイクロソフトのチームなど、他の経験で提示されることができます。</span><span class="sxs-lookup"><span data-stu-id="a2f24-108">Plans in Planner can be surfaced in other experiences, such as Microsoft Teams, to track work in the context of that experience.</span></span>
<span data-ttu-id="a2f24-109">**PlannerPlanContext**エントリの reresents の経験は、 **ownerAppId**プロパティに基づいて識別できます。</span><span class="sxs-lookup"><span data-stu-id="a2f24-109">The experience the **plannerPlanContext** entry reresents can be identified based on the **ownerAppId** property:</span></span>
 - <span data-ttu-id="a2f24-110">5e3ce6c0-2b1f-4285-8d4b-75ee78787346: コンテキストのエントリは、マイクロソフトのチームに属しています。</span><span class="sxs-lookup"><span data-stu-id="a2f24-110">5e3ce6c0-2b1f-4285-8d4b-75ee78787346 : The context entry belongs to Microsoft Teams.</span></span>
 - <span data-ttu-id="a2f24-111">00000003-0000-0ff1-ce00-000000000000: コンテキスト項目が SharePoint に所属します。</span><span class="sxs-lookup"><span data-stu-id="a2f24-111">00000003-0000-0ff1-ce00-000000000000 : The context entry belongs to SharePoint.</span></span>

## <a name="properties"></a><span data-ttu-id="a2f24-112">プロパティ</span><span class="sxs-lookup"><span data-stu-id="a2f24-112">Properties</span></span>
| <span data-ttu-id="a2f24-113">プロパティ</span><span class="sxs-lookup"><span data-stu-id="a2f24-113">Property</span></span>     | <span data-ttu-id="a2f24-114">型</span><span class="sxs-lookup"><span data-stu-id="a2f24-114">Type</span></span>   |<span data-ttu-id="a2f24-115">説明</span><span class="sxs-lookup"><span data-stu-id="a2f24-115">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="a2f24-116">associationType</span><span class="sxs-lookup"><span data-stu-id="a2f24-116">associationType</span></span>|<span data-ttu-id="a2f24-117">String</span><span class="sxs-lookup"><span data-stu-id="a2f24-117">String</span></span>|<span data-ttu-id="a2f24-118">Null 許容型。</span><span class="sxs-lookup"><span data-stu-id="a2f24-118">Nullable.</span></span> <span data-ttu-id="a2f24-119">[PlannerPlan](plannerplan.md)とアプリケーション間の関連のアプリケーションで定義されている型。</span><span class="sxs-lookup"><span data-stu-id="a2f24-119">An app-defined type of association between the [plannerPlan](plannerplan.md) and the app.</span></span> <span data-ttu-id="a2f24-120">アプリケーションは、同じ[plannerPlan](plannerplan.md)を別の種類の関係を追跡するためにこの情報を使用できます。</span><span class="sxs-lookup"><span data-stu-id="a2f24-120">The app can use this information to track different kinds of relationships to the same [plannerPlan](plannerplan.md).</span></span>|
|<span data-ttu-id="a2f24-121">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="a2f24-121">createdDateTime</span></span>|<span data-ttu-id="a2f24-122">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="a2f24-122">DateTimeOffset</span></span>|<span data-ttu-id="a2f24-123">読み取り専用。</span><span class="sxs-lookup"><span data-stu-id="a2f24-123">Read-only.</span></span> <span data-ttu-id="a2f24-124">日付と時刻**plannerPlanContext**が作成されました。</span><span class="sxs-lookup"><span data-stu-id="a2f24-124">The date and time when the **plannerPlanContext** was created.</span></span> <span data-ttu-id="a2f24-125">Timestamp 型は、ISO 8601 形式を使用して日付と時刻の情報を表し、常に UTC 時間です。</span><span class="sxs-lookup"><span data-stu-id="a2f24-125">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="a2f24-126">たとえば、2014 年 1 月 1 日午前 0 時 (UTC) は、次のようになります。`'2014-01-01T00:00:00Z'`</span><span class="sxs-lookup"><span data-stu-id="a2f24-126">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`.</span></span>|
|<span data-ttu-id="a2f24-127">displayNameSegments</span><span class="sxs-lookup"><span data-stu-id="a2f24-127">displayNameSegments</span></span>|<span data-ttu-id="a2f24-128">String コレクション</span><span class="sxs-lookup"><span data-stu-id="a2f24-128">String collection</span></span>|<span data-ttu-id="a2f24-129">外部環境の名前のセグメントです。</span><span class="sxs-lookup"><span data-stu-id="a2f24-129">The segments of the name of the external experience.</span></span> <span data-ttu-id="a2f24-130">セグメントでは、リレーションシップを表示するには、他のアプリケーションを可能にする階層構造を表します。</span><span class="sxs-lookup"><span data-stu-id="a2f24-130">Segments represent a hierarchical structure that allows other apps to display the relationship.</span></span>|
|<span data-ttu-id="a2f24-131">ownerAppId</span><span class="sxs-lookup"><span data-stu-id="a2f24-131">ownerAppId</span></span>|<span data-ttu-id="a2f24-132">String</span><span class="sxs-lookup"><span data-stu-id="a2f24-132">String</span></span>|<span data-ttu-id="a2f24-133">読み取り専用。</span><span class="sxs-lookup"><span data-stu-id="a2f24-133">Read-only.</span></span> <span data-ttu-id="a2f24-134">**PlannerPlanContext**を作成するアプリケーションの ID です。</span><span class="sxs-lookup"><span data-stu-id="a2f24-134">ID of the app that created the **plannerPlanContext**.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="a2f24-135">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="a2f24-135">JSON representation</span></span>

<span data-ttu-id="a2f24-136">リソースの JSON 表記を次に示します。</span><span class="sxs-lookup"><span data-stu-id="a2f24-136">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.plannerPlanContext"
}-->

```json
{
  "associationType": "Board",
  "createdDateTime": "2015-10-14T00:57:28.4698344Z",
  "displayNameSegments": [
    "Finance Team",
    "Budget Plans"
  ],
  "ownerAppId": "5e3ce6c0-2b1f-4285-8d4b-75ee78787346"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "plannerPlanContext resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
