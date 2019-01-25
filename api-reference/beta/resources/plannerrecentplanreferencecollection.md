---
title: plannerRecentPlanReferenceCollection リソースの種類
description: '**PlannerRecentPlanReferenceCollection**リソースでは、ユーザーが最近表示されたプランへの参照のコレクションを表します。 このリソースは、オープン型であり、plannerUser オブジェクトの一部であります。 プロパティ名は、対応する計画の ID です。 プロパティと値のペアの値は、plannerRecentPlanReference オブジェクトです。'
localization_priority: Normal
author: TarkanSevilmis
ms.prod: planner
ms.openlocfilehash: e27375e3f2395b3528873d8b83f0b5aa6f48d52e
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/24/2019
ms.locfileid: "29514993"
---
# <a name="plannerrecentplanreferencecollection-resource-type"></a><span data-ttu-id="c8653-106">plannerRecentPlanReferenceCollection リソースの種類</span><span class="sxs-lookup"><span data-stu-id="c8653-106">plannerRecentPlanReferenceCollection resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="c8653-107">**PlannerRecentPlanReferenceCollection**リソースでは、ユーザーが最近表示されたプランへの参照のコレクションを表します。</span><span class="sxs-lookup"><span data-stu-id="c8653-107">The **plannerRecentPlanReferenceCollection** resource represents the collection of references to plans that were recently viewed by a user.</span></span> <span data-ttu-id="c8653-108">このリソースは、オープン型であり、 [plannerUser](planneruser.md)オブジェクトの一部であります。</span><span class="sxs-lookup"><span data-stu-id="c8653-108">This resource is an open type and is part of the [plannerUser](planneruser.md) object.</span></span> <span data-ttu-id="c8653-109">プロパティ名は、対応する計画の ID です。</span><span class="sxs-lookup"><span data-stu-id="c8653-109">The property name is the ID of the corresponding plan.</span></span> <span data-ttu-id="c8653-110">プロパティと値のペアの値は、 [plannerRecentPlanReference](plannerrecentplanreference.md)オブジェクトです。</span><span class="sxs-lookup"><span data-stu-id="c8653-110">The value in the property-value pair is the [plannerRecentPlanReference](plannerrecentplanreference.md) object.</span></span>
<span data-ttu-id="c8653-111">このコレクションに新しい参照を追加するがコレクションのサイズが事前に定義された最大値を超えたときに自動的に最も古いエントリを削除します。</span><span class="sxs-lookup"><span data-stu-id="c8653-111">Adding new references to this collection will automatically remove the oldest entries when the size of the collection exceeds a predetermined maximum value.</span></span>


## <a name="properties"></a><span data-ttu-id="c8653-112">プロパティ</span><span class="sxs-lookup"><span data-stu-id="c8653-112">Properties</span></span>
<span data-ttu-id="c8653-113">このオープン型のプロパティを定義することができます。</span><span class="sxs-lookup"><span data-stu-id="c8653-113">You can define the properties of this open type.</span></span> <span data-ttu-id="c8653-114">プロパティ名は、 `id` [plannerPlan](plannerplan.md)リソースの値とその値は、 [plannerRecentPlanReference](plannerrecentplanreference.md)オブジェクトをする必要があります。</span><span class="sxs-lookup"><span data-stu-id="c8653-114">The property names are `id` values of [plannerPlan](plannerplan.md) resources and their values must be [plannerRecentPlanReference](plannerrecentplanreference.md) objects.</span></span> <span data-ttu-id="c8653-115">お気に入りの一覧で項目を削除するのにはプロパティの値を設定します`null`。</span><span class="sxs-lookup"><span data-stu-id="c8653-115">To remove an item in the favorites list, set the value of the property to `null`.</span></span>


## <a name="json-representation"></a><span data-ttu-id="c8653-116">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="c8653-116">JSON representation</span></span>

<span data-ttu-id="c8653-117">リソースの JSON 表記を次に示します。</span><span class="sxs-lookup"><span data-stu-id="c8653-117">The following is a JSON representation of the resource.</span></span>

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
  "suppressions": [
    "Error: /api-reference/beta/resources/plannerrecentplanreferencecollection.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
