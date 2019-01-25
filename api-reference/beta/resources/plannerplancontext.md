---
title: plannerPlanContext リソースの種類
description: '**PlannerPlanContext**リソースでは、プランナーの外部のユーザー エクスペリエンスの plannerPlan との関係を表します。 プランナーでプランは、その経験のコンテキストで作業を追跡するために、マイクロソフトのチームなど、他の経験で提示されることができます。'
localization_priority: Normal
author: TarkanSevilmis
ms.prod: planner
ms.openlocfilehash: 76260b51bc6f77acf6fac22e80bd676edd8b8e11
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/24/2019
ms.locfileid: "29509239"
---
# <a name="plannerplancontext-resource-type"></a><span data-ttu-id="9e6a0-104">plannerPlanContext リソースの種類</span><span class="sxs-lookup"><span data-stu-id="9e6a0-104">plannerPlanContext resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="9e6a0-105">**PlannerPlanContext**リソースでは、計画外のユーザー エクスペリエンスには、 [plannerPlan](plannerplan.md)との関係を表します。</span><span class="sxs-lookup"><span data-stu-id="9e6a0-105">The **plannerPlanContext** resource represents the relationship of a [plannerPlan](plannerplan.md) to a user experience outside of Planner.</span></span> <span data-ttu-id="9e6a0-106">プランナーでプランは、その経験のコンテキストで作業を追跡するために、マイクロソフトのチームなど、他の経験で提示されることができます。</span><span class="sxs-lookup"><span data-stu-id="9e6a0-106">Plans in Planner can be surfaced in other experiences, such as Microsoft Teams, to track work in the context of that experience.</span></span>
<span data-ttu-id="9e6a0-107">**PlannerPlanContext**エントリの reresents の経験は、 **ownerAppId**プロパティに基づいて識別できます。</span><span class="sxs-lookup"><span data-stu-id="9e6a0-107">The experience the **plannerPlanContext** entry reresents can be identified based on the **ownerAppId** property:</span></span>
 - <span data-ttu-id="9e6a0-108">5e3ce6c0-2b1f-4285-8d4b-75ee78787346: コンテキストのエントリは、マイクロソフトのチームに属しています。</span><span class="sxs-lookup"><span data-stu-id="9e6a0-108">5e3ce6c0-2b1f-4285-8d4b-75ee78787346 : The context entry belongs to Microsoft Teams.</span></span>
 - <span data-ttu-id="9e6a0-109">00000003-0000-0ff1-ce00-000000000000: コンテキスト項目が SharePoint に所属します。</span><span class="sxs-lookup"><span data-stu-id="9e6a0-109">00000003-0000-0ff1-ce00-000000000000 : The context entry belongs to SharePoint.</span></span>

## <a name="properties"></a><span data-ttu-id="9e6a0-110">プロパティ</span><span class="sxs-lookup"><span data-stu-id="9e6a0-110">Properties</span></span>
| <span data-ttu-id="9e6a0-111">プロパティ</span><span class="sxs-lookup"><span data-stu-id="9e6a0-111">Property</span></span>     | <span data-ttu-id="9e6a0-112">型</span><span class="sxs-lookup"><span data-stu-id="9e6a0-112">Type</span></span>   |<span data-ttu-id="9e6a0-113">説明</span><span class="sxs-lookup"><span data-stu-id="9e6a0-113">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="9e6a0-114">associationType</span><span class="sxs-lookup"><span data-stu-id="9e6a0-114">associationType</span></span>|<span data-ttu-id="9e6a0-115">String</span><span class="sxs-lookup"><span data-stu-id="9e6a0-115">String</span></span>|<span data-ttu-id="9e6a0-116">Null 許容型。</span><span class="sxs-lookup"><span data-stu-id="9e6a0-116">Nullable.</span></span> <span data-ttu-id="9e6a0-117">[PlannerPlan](plannerplan.md)とアプリケーション間の関連のアプリケーションで定義されている型。</span><span class="sxs-lookup"><span data-stu-id="9e6a0-117">An app-defined type of association between the [plannerPlan](plannerplan.md) and the app.</span></span> <span data-ttu-id="9e6a0-118">アプリケーションは、同じ[plannerPlan](plannerplan.md)を別の種類の関係を追跡するためにこの情報を使用できます。</span><span class="sxs-lookup"><span data-stu-id="9e6a0-118">The app can use this information to track different kinds of relationships to the same [plannerPlan](plannerplan.md).</span></span>|
|<span data-ttu-id="9e6a0-119">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="9e6a0-119">createdDateTime</span></span>|<span data-ttu-id="9e6a0-120">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="9e6a0-120">DateTimeOffset</span></span>|<span data-ttu-id="9e6a0-121">読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="9e6a0-121">Read-only.</span></span> <span data-ttu-id="9e6a0-122">日付と時刻**plannerPlanContext**が作成されました。</span><span class="sxs-lookup"><span data-stu-id="9e6a0-122">The date and time when the **plannerPlanContext** was created.</span></span> <span data-ttu-id="9e6a0-123">Timestamp 型は、ISO 8601 形式を使用して日付と時刻の情報を表し、常に UTC 時間です。</span><span class="sxs-lookup"><span data-stu-id="9e6a0-123">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="9e6a0-124">たとえば、2014 年 1 月 1 日午前 0 時 (UTC) は、`'2014-01-01T00:00:00Z'` のようになります。</span><span class="sxs-lookup"><span data-stu-id="9e6a0-124">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`.</span></span>|
|<span data-ttu-id="9e6a0-125">displayNameSegments</span><span class="sxs-lookup"><span data-stu-id="9e6a0-125">displayNameSegments</span></span>|<span data-ttu-id="9e6a0-126">String コレクション</span><span class="sxs-lookup"><span data-stu-id="9e6a0-126">String collection</span></span>|<span data-ttu-id="9e6a0-127">外部環境の名前のセグメントです。</span><span class="sxs-lookup"><span data-stu-id="9e6a0-127">The segments of the name of the external experience.</span></span> <span data-ttu-id="9e6a0-128">セグメントでは、リレーションシップを表示するには、他のアプリケーションを可能にする階層構造を表します。</span><span class="sxs-lookup"><span data-stu-id="9e6a0-128">Segments represent a hierarchical structure that allows other apps to display the relationship.</span></span>|
|<span data-ttu-id="9e6a0-129">ownerAppId</span><span class="sxs-lookup"><span data-stu-id="9e6a0-129">ownerAppId</span></span>|<span data-ttu-id="9e6a0-130">String</span><span class="sxs-lookup"><span data-stu-id="9e6a0-130">String</span></span>|<span data-ttu-id="9e6a0-131">読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="9e6a0-131">Read-only.</span></span> <span data-ttu-id="9e6a0-132">**PlannerPlanContext**を作成するアプリケーションの ID です。</span><span class="sxs-lookup"><span data-stu-id="9e6a0-132">ID of the app that created the **plannerPlanContext**.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="9e6a0-133">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="9e6a0-133">JSON representation</span></span>

<span data-ttu-id="9e6a0-134">リソースの JSON 表記を次に示します。</span><span class="sxs-lookup"><span data-stu-id="9e6a0-134">The following is a JSON representation of the resource.</span></span>

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
<!--
{
  "type": "#page.annotation",
  "description": "plannerPlanContext resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/plannerplancontext.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
