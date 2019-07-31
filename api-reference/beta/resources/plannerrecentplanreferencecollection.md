---
title: plannerRecentPlanReferenceCollection リソースの種類
description: '**PlannerRecentPlanReferenceCollection**リソースは、ユーザーが最近参照したプランへの参照のコレクションを表します。 このリソースはオープンタイプで、プランのユーザーオブジェクトの一部です。 プロパティ名は、対応するプランの ID です。 プロパティと値のペアの値は、plannerRecentPlanReference オブジェクトです。'
localization_priority: Normal
author: TarkanSevilmis
ms.prod: planner
doc_type: resourcePageType
ms.openlocfilehash: 474cd321357e698d65b768b94fb867285978984b
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "35965860"
---
# <a name="plannerrecentplanreferencecollection-resource-type"></a><span data-ttu-id="ad1dd-106">plannerRecentPlanReferenceCollection リソースの種類</span><span class="sxs-lookup"><span data-stu-id="ad1dd-106">plannerRecentPlanReferenceCollection resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="ad1dd-107">**PlannerRecentPlanReferenceCollection**リソースは、ユーザーが最近参照したプランへの参照のコレクションを表します。</span><span class="sxs-lookup"><span data-stu-id="ad1dd-107">The **plannerRecentPlanReferenceCollection** resource represents the collection of references to plans that were recently viewed by a user.</span></span> <span data-ttu-id="ad1dd-108">このリソースはオープンタイプで、[プランのユーザー](planneruser.md)オブジェクトの一部です。</span><span class="sxs-lookup"><span data-stu-id="ad1dd-108">This resource is an open type and is part of the [plannerUser](planneruser.md) object.</span></span> <span data-ttu-id="ad1dd-109">プロパティ名は、対応するプランの ID です。</span><span class="sxs-lookup"><span data-stu-id="ad1dd-109">The property name is the ID of the corresponding plan.</span></span> <span data-ttu-id="ad1dd-110">プロパティと値のペアの値は、 [plannerRecentPlanReference](plannerrecentplanreference.md)オブジェクトです。</span><span class="sxs-lookup"><span data-stu-id="ad1dd-110">The value in the property-value pair is the [plannerRecentPlanReference](plannerrecentplanreference.md) object.</span></span>
<span data-ttu-id="ad1dd-111">このコレクションに新しい参照を追加すると、コレクションのサイズが事前に定義された最大値を超えると、最も古いエントリが自動的に削除されます。</span><span class="sxs-lookup"><span data-stu-id="ad1dd-111">Adding new references to this collection will automatically remove the oldest entries when the size of the collection exceeds a predetermined maximum value.</span></span>


## <a name="properties"></a><span data-ttu-id="ad1dd-112">プロパティ</span><span class="sxs-lookup"><span data-stu-id="ad1dd-112">Properties</span></span>
<span data-ttu-id="ad1dd-113">このオープン型のプロパティを定義できます。</span><span class="sxs-lookup"><span data-stu-id="ad1dd-113">You can define the properties of this open type.</span></span> <span data-ttu-id="ad1dd-114">プロパティ名は、 `id` plan リソース[](plannerplan.md)およびその値が[plannerRecentPlanReference](plannerrecentplanreference.md)オブジェクトである必要があることを示す値です。</span><span class="sxs-lookup"><span data-stu-id="ad1dd-114">The property names are `id` values of [plannerPlan](plannerplan.md) resources and their values must be [plannerRecentPlanReference](plannerrecentplanreference.md) objects.</span></span> <span data-ttu-id="ad1dd-115">[お気に入り] の一覧から項目を削除するには、プロパティの値`null`をに設定します。</span><span class="sxs-lookup"><span data-stu-id="ad1dd-115">To remove an item in the favorites list, set the value of the property to `null`.</span></span>


## <a name="json-representation"></a><span data-ttu-id="ad1dd-116">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="ad1dd-116">JSON representation</span></span>

<span data-ttu-id="ad1dd-117">リソースの JSON 表記を次に示します。</span><span class="sxs-lookup"><span data-stu-id="ad1dd-117">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.plannerRecentPlanReferenceCollection"
}-->

```json
{
  "7oTB5aMIAE2rVo-1N-L7RmQAGX2q": {
    "@odata.type": "microsoft.graph.plannerRecentPlanReference",
    "lastAccessedDateTime": "2017-12-02T22:49:46.155Z",
    "planTitle": "Purchase Workflow"
  },
  "iKNMHkk3vEWpSF7F7iZWIGQAAMMw": {
    "@odata.type": "microsoft.graph.plannerRecentPlanReference",
    "lastAccessedDateTime": "2017-12-03T21:59:28.975Z",
    "planTitle": "New Year's Office Party"
  }
}
```



<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "plannerRecentPlanReferenceCollection resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
