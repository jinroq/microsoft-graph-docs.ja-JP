---
title: プラン/プランコンテキストコレクションリソースの種類
description: plan **** は、プランがリンクされている外部コンテキストのコレクションを表します。 このリソースはオープン型であり、plan オブジェクトの一部です。 プロパティと値のペアの値は、plan プロパティのコンテキストオブジェクトです。
localization_priority: Normal
author: TarkanSevilmis
ms.prod: planner
ms.openlocfilehash: 8d5394ff8a9503ab9ffba4810c9c2cad0d9a2fbf
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/26/2019
ms.locfileid: "33344459"
---
# <a name="plannerplancontextcollection-resource-type"></a><span data-ttu-id="8e671-105">プラン/プランコンテキストコレクションリソースの種類</span><span class="sxs-lookup"><span data-stu-id="8e671-105">plannerPlanContextCollection resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]


<span data-ttu-id="8e671-106">plan \*\*\*\* は、プランがリンクされている外部コンテキストのコレクションを表します。</span><span class="sxs-lookup"><span data-stu-id="8e671-106">The **plannerPlanContextCollection** resource represents the collection of external contexts to which a plan is linked.</span></span> <span data-ttu-id="8e671-107">このリソースはオープン型であり、 [plan](plannerplan.md)オブジェクトの一部です。</span><span class="sxs-lookup"><span data-stu-id="8e671-107">This resource is an open type and is part of the [plannerPlan](plannerplan.md) object.</span></span> <span data-ttu-id="8e671-108">プロパティと値のペアの値は、plan プロパティの[コンテキスト](plannerplancontext.md)オブジェクトです。</span><span class="sxs-lookup"><span data-stu-id="8e671-108">The value in the property-value pair is the [plannerPlanContext](plannerplancontext.md) object.</span></span>


## <a name="properties"></a><span data-ttu-id="8e671-109">プロパティ</span><span class="sxs-lookup"><span data-stu-id="8e671-109">Properties</span></span>
<span data-ttu-id="8e671-110">このオープン型のプロパティを定義できます。</span><span class="sxs-lookup"><span data-stu-id="8e671-110">You can define the properties of this open type.</span></span> <span data-ttu-id="8e671-111">プロパティの値は、プロパティ名として外部コンテキストを表す特徴的識別子にする必要があります。</span><span class="sxs-lookup"><span data-stu-id="8e671-111">The property values should be distinctive identifier that represents the external context as the property name.</span></span> <span data-ttu-id="8e671-112">プロパティの値は、 [context](plannerplancontext.md)オブジェクトをプランする必要があります。</span><span class="sxs-lookup"><span data-stu-id="8e671-112">The property values must be [plannerPlanContext](plannerplancontext.md) objects.</span></span> <span data-ttu-id="8e671-113">OData 要件に基づいて、オープン型のプロパティ名に次の文字を`.`含める`:`こと`%`は`@`できません:、、、。</span><span class="sxs-lookup"><span data-stu-id="8e671-113">Based on OData requirements, property names in open types cannot contain the following characters: `.`, `:`, `%`, `@`.</span></span> <span data-ttu-id="8e671-114">これらの文字は、URL エンコードを使用してエンコードする必要があります。</span><span class="sxs-lookup"><span data-stu-id="8e671-114">These characters need to be encoded using URL encoding.</span></span> <span data-ttu-id="8e671-115">[お気に入り] の一覧から項目を削除するには、プロパティの値`null`をに設定します。</span><span class="sxs-lookup"><span data-stu-id="8e671-115">To remove an item in the favorites list, set the value of the property to `null`.</span></span>

## <a name="json-representation"></a><span data-ttu-id="8e671-116">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="8e671-116">JSON representation</span></span>

<span data-ttu-id="8e671-117">リソースの JSON 表記を次に示します。</span><span class="sxs-lookup"><span data-stu-id="8e671-117">The following is a JSON representation of the resource.</span></span>

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
<!--
{
  "type": "#page.annotation",
  "description": "plannerPlanContextCollection resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
