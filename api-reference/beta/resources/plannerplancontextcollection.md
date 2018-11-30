---
title: plannerPlanContextCollection リソースの種類
description: '**PlannerPlanContextCollection**リソースでは、プランがリンクされている外部のコンテキストのコレクションを表します。 このリソースは、オープン型であり、plannerPlan オブジェクトの一部であります。 プロパティと値のペアの値は、plannerPlanContext オブジェクトです。'
ms.openlocfilehash: ae17e604bf3d59b7b825fe36a8f93f05d5cc835f
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27070154"
---
# <a name="plannerplancontextcollection-resource-type"></a><span data-ttu-id="14574-105">plannerPlanContextCollection リソースの種類</span><span class="sxs-lookup"><span data-stu-id="14574-105">plannerPlanContextCollection resource type</span></span>

> <span data-ttu-id="14574-106">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="14574-106">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="14574-107">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="14574-107">Use of these APIs in production applications is not supported.</span></span>


<span data-ttu-id="14574-108">**PlannerPlanContextCollection**リソースでは、プランがリンクされている外部のコンテキストのコレクションを表します。</span><span class="sxs-lookup"><span data-stu-id="14574-108">The **plannerPlanContextCollection** resource represents the collection of external contexts to which a plan is linked.</span></span> <span data-ttu-id="14574-109">このリソースは、オープン型であり、 [plannerPlan](plannerplan.md)オブジェクトの一部であります。</span><span class="sxs-lookup"><span data-stu-id="14574-109">This resource is an open type and is part of the [plannerPlan](plannerplan.md) object.</span></span> <span data-ttu-id="14574-110">プロパティと値のペアの値は、 [plannerPlanContext](plannerplancontext.md)オブジェクトです。</span><span class="sxs-lookup"><span data-stu-id="14574-110">The value in the property-value pair is the [plannerPlanContext](plannerplancontext.md) object.</span></span>


## <a name="properties"></a><span data-ttu-id="14574-111">プロパティ</span><span class="sxs-lookup"><span data-stu-id="14574-111">Properties</span></span>
<span data-ttu-id="14574-112">このオープン型のプロパティを定義することができます。</span><span class="sxs-lookup"><span data-stu-id="14574-112">You can define the properties of this open type.</span></span> <span data-ttu-id="14574-113">プロパティの値はプロパティ名と外部のコンテキストを表す特徴的な識別子である必要があります。</span><span class="sxs-lookup"><span data-stu-id="14574-113">The property values should be distinctive identifier that represents the external context as the property name.</span></span> <span data-ttu-id="14574-114">プロパティの値は、 [plannerPlanContext](plannerplancontext.md)オブジェクトである必要があります。</span><span class="sxs-lookup"><span data-stu-id="14574-114">The property values must be [plannerPlanContext](plannerplancontext.md) objects.</span></span> <span data-ttu-id="14574-115">OData の要件に基づき、オープン型のプロパティ名は次の文字を含めることはできません: `.`、 `:`、 `%`、 `@`。</span><span class="sxs-lookup"><span data-stu-id="14574-115">Based on OData requirements, property names in open types cannot contain the following characters: `.`, `:`, `%`, `@`.</span></span> <span data-ttu-id="14574-116">これらの文字は、URL エンコーディングを使用してエンコードする必要があります。</span><span class="sxs-lookup"><span data-stu-id="14574-116">These characters need to be encoded using URL encoding.</span></span> <span data-ttu-id="14574-117">お気に入りの一覧で項目を削除するのにはプロパティの値を設定します`null`。</span><span class="sxs-lookup"><span data-stu-id="14574-117">To remove an item in the favorites list, set the value of the property to `null`.</span></span>

## <a name="json-representation"></a><span data-ttu-id="14574-118">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="14574-118">JSON representation</span></span>

<span data-ttu-id="14574-119">リソースの JSON 表記を次に示します。</span><span class="sxs-lookup"><span data-stu-id="14574-119">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.plannerPlanContextCollection"
}-->

```json
{
  "48#19%3Ad128c63941b24733951ea7defd81e550%40thread%2Eskype19%3Ad128c63941b24733951ea7defd81e550%40thread%2Eskype": {
    "@odata.type": "#microsoft.graph.plannerPlanContext",
    "associationType": "Board",
    "createdDateTime": "2015-10-14T00:57:28.4698344Z",
    "displayNameSegments": [
        "Finance Team",
        "Budget Plans"
    ],
    "ownerAppId": "5e3ce6c0-2b1f-4285-8d4b-75ee78787346"
  }
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "plannerPlanContextCollection resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
