---
title: plannerGroup リソースの種類
description: '**plannerGroup** リソースは、group の Planner リソースへのアクセスを提供します。使用可能なプロパティは含まれていません。'
localization_priority: Normal
author: TarkanSevilmis
ms.prod: planner
ms.openlocfilehash: 84bb20d0b13f9a99db2f8c59b20e0c9c7c87f93f
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/24/2019
ms.locfileid: "29513782"
---
# <a name="plannergroup-resource-type"></a><span data-ttu-id="72f79-104">plannerGroup リソースの種類</span><span class="sxs-lookup"><span data-stu-id="72f79-104">plannerGroup resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="72f79-p102">**plannerGroup** リソースは、[group](group.md) の Planner リソースへのアクセスを提供します。使用可能なプロパティは含まれていません。</span><span class="sxs-lookup"><span data-stu-id="72f79-p102">The **plannerGroup** resource provides access to Planner resources for a [group](group.md). It doesn't contain any usable properties.</span></span>

## <a name="methods"></a><span data-ttu-id="72f79-107">メソッド</span><span class="sxs-lookup"><span data-stu-id="72f79-107">Methods</span></span>

| <span data-ttu-id="72f79-108">メソッド</span><span class="sxs-lookup"><span data-stu-id="72f79-108">Method</span></span>           | <span data-ttu-id="72f79-109">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="72f79-109">Return Type</span></span>    |<span data-ttu-id="72f79-110">説明</span><span class="sxs-lookup"><span data-stu-id="72f79-110">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="72f79-111">plans を一覧表示する</span><span class="sxs-lookup"><span data-stu-id="72f79-111">List plans</span></span>](../api/plannergroup-list-plans.md) |<span data-ttu-id="72f79-112">[plannerPlan](plannerplan.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="72f79-112">[plannerPlan](plannerplan.md) collection</span></span>| <span data-ttu-id="72f79-113">**plannerPlan** オブジェクト コレクションを取得します。</span><span class="sxs-lookup"><span data-stu-id="72f79-113">Get a **plannerPlan** object collection.</span></span>|

## <a name="properties"></a><span data-ttu-id="72f79-114">プロパティ</span><span class="sxs-lookup"><span data-stu-id="72f79-114">Properties</span></span>
| <span data-ttu-id="72f79-115">プロパティ</span><span class="sxs-lookup"><span data-stu-id="72f79-115">Property</span></span>     | <span data-ttu-id="72f79-116">型</span><span class="sxs-lookup"><span data-stu-id="72f79-116">Type</span></span>   |<span data-ttu-id="72f79-117">説明</span><span class="sxs-lookup"><span data-stu-id="72f79-117">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="72f79-118">id</span><span class="sxs-lookup"><span data-stu-id="72f79-118">id</span></span>|<span data-ttu-id="72f79-119">String</span><span class="sxs-lookup"><span data-stu-id="72f79-119">String</span></span>| <span data-ttu-id="72f79-p103">読み取り専用です。**plannerGroup** の識別子</span><span class="sxs-lookup"><span data-stu-id="72f79-p103">Read-only. Identifier of the **plannerGroup**</span></span>|

## <a name="relationships"></a><span data-ttu-id="72f79-122">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="72f79-122">Relationships</span></span>
| <span data-ttu-id="72f79-123">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="72f79-123">Relationship</span></span> | <span data-ttu-id="72f79-124">型</span><span class="sxs-lookup"><span data-stu-id="72f79-124">Type</span></span>   |<span data-ttu-id="72f79-125">説明</span><span class="sxs-lookup"><span data-stu-id="72f79-125">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="72f79-126">plans</span><span class="sxs-lookup"><span data-stu-id="72f79-126">plans</span></span>|<span data-ttu-id="72f79-127">[plannerPlan](plannerplan.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="72f79-127">[plannerPlan](plannerplan.md) collection</span></span>| <span data-ttu-id="72f79-p104">読み取り専用です。Null 許容型。グループが所有する [plannerPlans](plannerplan.md) を返します。</span><span class="sxs-lookup"><span data-stu-id="72f79-p104">Read-only. Nullable. Returns the [plannerPlans](plannerplan.md) owned by the group.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="72f79-131">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="72f79-131">JSON representation</span></span>
<span data-ttu-id="72f79-132">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="72f79-132">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.plannerGroup"
}-->

```json
{
  "id": "String (identifier)"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "plannerGroup resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/plannergroup.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
