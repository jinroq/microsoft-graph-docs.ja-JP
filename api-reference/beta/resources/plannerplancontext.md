---
title: プラン "Context/プラン" コンテキストリソースの種類
description: '**Plan By コンテキスト**リソースは、Planner の外部のユーザー環境に対するプランの関係を表します。 Planner のプランは、Microsoft Teams などの他のエクスペリエンスで提示して、そのエクスペリエンスのコンテキストで作業を追跡することができます。'
localization_priority: Normal
author: TarkanSevilmis
ms.prod: planner
doc_type: resourcePageType
ms.openlocfilehash: 6a1d638e26ae51bdca86bf397889d84a3a97dc11
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "36009028"
---
# <a name="plannerplancontext-resource-type"></a><span data-ttu-id="92b24-104">プラン "Context/プラン" コンテキストリソースの種類</span><span class="sxs-lookup"><span data-stu-id="92b24-104">plannerPlanContext resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="92b24-105">**Plan By コンテキスト**リソースは、Planner の外部のユーザー環境に対する[プラン](plannerplan.md)の関係を表します。</span><span class="sxs-lookup"><span data-stu-id="92b24-105">The **plannerPlanContext** resource represents the relationship of a [plannerPlan](plannerplan.md) to a user experience outside of Planner.</span></span> <span data-ttu-id="92b24-106">Planner のプランは、Microsoft Teams などの他のエクスペリエンスで提示して、そのエクスペリエンスのコンテキストで作業を追跡することができます。</span><span class="sxs-lookup"><span data-stu-id="92b24-106">Plans in Planner can be surfaced in other experiences, such as Microsoft Teams, to track work in the context of that experience.</span></span>
<span data-ttu-id="92b24-107">**プランのコンテキスト**エントリ再生機能は、 **ownerappid**プロパティに基づいて識別できます。</span><span class="sxs-lookup"><span data-stu-id="92b24-107">The experience the **plannerPlanContext** entry reresents can be identified based on the **ownerAppId** property:</span></span>
- <span data-ttu-id="92b24-108">5e3ce6c0-2b1f-4285-8d4b-75ee78787346: コンテキストエントリは Microsoft Teams に属しています。</span><span class="sxs-lookup"><span data-stu-id="92b24-108">5e3ce6c0-2b1f-4285-8d4b-75ee78787346 : The context entry belongs to Microsoft Teams.</span></span>
- <span data-ttu-id="92b24-109">00000003-0000-0ff1-ce00-000000000000: コンテキストエントリは SharePoint に属しています。</span><span class="sxs-lookup"><span data-stu-id="92b24-109">00000003-0000-0ff1-ce00-000000000000 : The context entry belongs to SharePoint.</span></span>

## <a name="properties"></a><span data-ttu-id="92b24-110">プロパティ</span><span class="sxs-lookup"><span data-stu-id="92b24-110">Properties</span></span>
| <span data-ttu-id="92b24-111">プロパティ</span><span class="sxs-lookup"><span data-stu-id="92b24-111">Property</span></span>     | <span data-ttu-id="92b24-112">型</span><span class="sxs-lookup"><span data-stu-id="92b24-112">Type</span></span>   |<span data-ttu-id="92b24-113">説明</span><span class="sxs-lookup"><span data-stu-id="92b24-113">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="92b24-114">associationType</span><span class="sxs-lookup"><span data-stu-id="92b24-114">associationType</span></span>|<span data-ttu-id="92b24-115">String</span><span class="sxs-lookup"><span data-stu-id="92b24-115">String</span></span>|<span data-ttu-id="92b24-116">Null 許容型。</span><span class="sxs-lookup"><span data-stu-id="92b24-116">Nullable.</span></span> <span data-ttu-id="92b24-117">アプリケーションで定義された、[プラン](plannerplan.md)とアプリの間の関連付けの種類。</span><span class="sxs-lookup"><span data-stu-id="92b24-117">An app-defined type of association between the [plannerPlan](plannerplan.md) and the app.</span></span> <span data-ttu-id="92b24-118">アプリはこの情報を使用して、同じ[プラン](plannerplan.md)の異なる種類のリレーションシップを追跡できます。</span><span class="sxs-lookup"><span data-stu-id="92b24-118">The app can use this information to track different kinds of relationships to the same [plannerPlan](plannerplan.md).</span></span>|
|<span data-ttu-id="92b24-119">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="92b24-119">createdDateTime</span></span>|<span data-ttu-id="92b24-120">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="92b24-120">DateTimeOffset</span></span>|<span data-ttu-id="92b24-121">読み取り専用。</span><span class="sxs-lookup"><span data-stu-id="92b24-121">Read-only.</span></span> <span data-ttu-id="92b24-122">**プラン**が作成された日付と時刻。</span><span class="sxs-lookup"><span data-stu-id="92b24-122">The date and time when the **plannerPlanContext** was created.</span></span> <span data-ttu-id="92b24-123">Timestamp 型は、ISO 8601 形式を使用して日付と時刻の情報を表します。これは常に UTC 時間です。</span><span class="sxs-lookup"><span data-stu-id="92b24-123">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="92b24-124">たとえば、2014 年 1 月 1 日午前 0 時 (UTC) は、次のようになります。`'2014-01-01T00:00:00Z'`</span><span class="sxs-lookup"><span data-stu-id="92b24-124">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`.</span></span>|
|<span data-ttu-id="92b24-125">displayNameSegments</span><span class="sxs-lookup"><span data-stu-id="92b24-125">displayNameSegments</span></span>|<span data-ttu-id="92b24-126">文字列コレクション</span><span class="sxs-lookup"><span data-stu-id="92b24-126">String collection</span></span>|<span data-ttu-id="92b24-127">外部環境の名前のセグメント。</span><span class="sxs-lookup"><span data-stu-id="92b24-127">The segments of the name of the external experience.</span></span> <span data-ttu-id="92b24-128">セグメントは、他のアプリがリレーションシップを表示できる階層構造を表します。</span><span class="sxs-lookup"><span data-stu-id="92b24-128">Segments represent a hierarchical structure that allows other apps to display the relationship.</span></span>|
|<span data-ttu-id="92b24-129">ownerAppId</span><span class="sxs-lookup"><span data-stu-id="92b24-129">ownerAppId</span></span>|<span data-ttu-id="92b24-130">String</span><span class="sxs-lookup"><span data-stu-id="92b24-130">String</span></span>|<span data-ttu-id="92b24-131">読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="92b24-131">Read-only.</span></span> <span data-ttu-id="92b24-132">**プランのコンテキスト**を作成したアプリの ID です。</span><span class="sxs-lookup"><span data-stu-id="92b24-132">ID of the app that created the **plannerPlanContext**.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="92b24-133">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="92b24-133">JSON representation</span></span>

<span data-ttu-id="92b24-134">リソースの JSON 表記を次に示します。</span><span class="sxs-lookup"><span data-stu-id="92b24-134">The following is a JSON representation of the resource.</span></span>

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
  "suppressions": []
}
-->
