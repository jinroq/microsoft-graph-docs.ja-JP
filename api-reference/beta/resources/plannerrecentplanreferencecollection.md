---
title: plannerRecentPlanReferenceCollection リソースの種類
description: '**PlannerRecentPlanReferenceCollection**リソースでは、ユーザーが最近表示されたプランへの参照のコレクションを表します。 このリソースは、オープン型であり、plannerUser オブジェクトの一部であります。 プロパティ名は、対応する計画の ID です。 プロパティと値のペアの値は、plannerRecentPlanReference オブジェクトです。'
ms.openlocfilehash: b22f7367a1826c95889b63a6884885ce49497c33
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27074329"
---
# <a name="plannerrecentplanreferencecollection-resource-type"></a><span data-ttu-id="64822-106">plannerRecentPlanReferenceCollection リソースの種類</span><span class="sxs-lookup"><span data-stu-id="64822-106">plannerRecentPlanReferenceCollection resource type</span></span>

> <span data-ttu-id="64822-107">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="64822-107">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="64822-108">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="64822-108">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="64822-109">**PlannerRecentPlanReferenceCollection**リソースでは、ユーザーが最近表示されたプランへの参照のコレクションを表します。</span><span class="sxs-lookup"><span data-stu-id="64822-109">The **plannerRecentPlanReferenceCollection** resource represents the collection of references to plans that were recently viewed by a user.</span></span> <span data-ttu-id="64822-110">このリソースは、オープン型であり、 [plannerUser](planneruser.md)オブジェクトの一部であります。</span><span class="sxs-lookup"><span data-stu-id="64822-110">This resource is an open type and is part of the [plannerUser](planneruser.md) object.</span></span> <span data-ttu-id="64822-111">プロパティ名は、対応する計画の ID です。</span><span class="sxs-lookup"><span data-stu-id="64822-111">The property name is the ID of the corresponding plan.</span></span> <span data-ttu-id="64822-112">プロパティと値のペアの値は、 [plannerRecentPlanReference](plannerrecentplanreference.md)オブジェクトです。</span><span class="sxs-lookup"><span data-stu-id="64822-112">The value in the property-value pair is the [plannerRecentPlanReference](plannerrecentplanreference.md) object.</span></span>
<span data-ttu-id="64822-113">このコレクションに新しい参照を追加するがコレクションのサイズが事前に定義された最大値を超えたときに自動的に最も古いエントリを削除します。</span><span class="sxs-lookup"><span data-stu-id="64822-113">Adding new references to this collection will automatically remove the oldest entries when the size of the collection exceeds a predetermined maximum value.</span></span>


## <a name="properties"></a><span data-ttu-id="64822-114">プロパティ</span><span class="sxs-lookup"><span data-stu-id="64822-114">Properties</span></span>
<span data-ttu-id="64822-115">このオープン型のプロパティを定義することができます。</span><span class="sxs-lookup"><span data-stu-id="64822-115">You can define the properties of this open type.</span></span> <span data-ttu-id="64822-116">プロパティ名は、 `id` [plannerPlan](plannerplan.md)リソースの値とその値は、 [plannerRecentPlanReference](plannerrecentplanreference.md)オブジェクトをする必要があります。</span><span class="sxs-lookup"><span data-stu-id="64822-116">The property names are `id` values of [plannerPlan](plannerplan.md) resources and their values must be [plannerRecentPlanReference](plannerrecentplanreference.md) objects.</span></span> <span data-ttu-id="64822-117">お気に入りの一覧で項目を削除するのにはプロパティの値を設定します`null`。</span><span class="sxs-lookup"><span data-stu-id="64822-117">To remove an item in the favorites list, set the value of the property to `null`.</span></span>


## <a name="json-representation"></a><span data-ttu-id="64822-118">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="64822-118">JSON representation</span></span>

<span data-ttu-id="64822-119">リソースの JSON 表記を次に示します。</span><span class="sxs-lookup"><span data-stu-id="64822-119">The following is a JSON representation of the resource.</span></span>

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
<!-- {
  "type": "#page.annotation",
  "description": "plannerRecentPlanReferenceCollection resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->