---
title: プラン/お気に入りプラン Referencecollection リソースの種類
description: " この値は、\"プラン参照\" オブジェクトを示します。"
author: TarkanSevilmis
localization_priority: Normal
ms.prod: planner
doc_type: resourcePageType
ms.openlocfilehash: 67149f0ccf8ec04fe702a0d77b1fb2f5f6020365
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "35965951"
---
# <a name="plannerfavoriteplanreferencecollection-resource-type"></a><span data-ttu-id="5cc9a-103">プラン/お気に入りプラン Referencecollection リソースの種類</span><span class="sxs-lookup"><span data-stu-id="5cc9a-103">plannerFavoritePlanReferenceCollection resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="5cc9a-104">**Plan**は、ユーザーによってお気に入りとしてマークされているプランへの参照のコレクションを表します。</span><span class="sxs-lookup"><span data-stu-id="5cc9a-104">The **plannerFavoritePlanReferenceCollection** resource represents the collection of references to plans that are marked as a favorite by a user.</span></span> <span data-ttu-id="5cc9a-105">このリソースはオープンタイプで、[プランのユーザー](planneruser.md)オブジェクトの一部です。</span><span class="sxs-lookup"><span data-stu-id="5cc9a-105">This resource is an open type and is part of the [plannerUser](planneruser.md) object.</span></span> <span data-ttu-id="5cc9a-106">プロパティと値のペアのプロパティ名は、対応するプランの ID です。この値は、"[プラン参照](plannerfavoriteplanreference.md)" オブジェクトを示します。</span><span class="sxs-lookup"><span data-stu-id="5cc9a-106">The property name in the property-value pair is the ID of the corresponding plan; the value is the [plannerFavoritePlanReference](plannerfavoriteplanreference.md) object.</span></span>


## <a name="properties"></a><span data-ttu-id="5cc9a-107">プロパティ</span><span class="sxs-lookup"><span data-stu-id="5cc9a-107">Properties</span></span>
<span data-ttu-id="5cc9a-108">このオープン型のプロパティを定義できます。</span><span class="sxs-lookup"><span data-stu-id="5cc9a-108">You can define the properties of this open type.</span></span> <span data-ttu-id="5cc9a-109">プロパティ名は`id` 、plan リソースとその値を[プラン](plannerplan.md)にする必要が[](plannerfavoriteplanreference.md)あります。</span><span class="sxs-lookup"><span data-stu-id="5cc9a-109">The property names are `id` values of [plannerPlan](plannerplan.md) resources and their values must be [plannerFavoritePlanReference](plannerfavoriteplanreference.md) objects.</span></span> <span data-ttu-id="5cc9a-110">[お気に入り] の一覧から項目を削除するには、プロパティの値`null`をに設定します。</span><span class="sxs-lookup"><span data-stu-id="5cc9a-110">To remove an item in the favorites list, set the value of the property to `null`.</span></span>


## <a name="json-representation"></a><span data-ttu-id="5cc9a-111">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="5cc9a-111">JSON representation</span></span>

<span data-ttu-id="5cc9a-112">リソースの JSON 表記を次に示します。</span><span class="sxs-lookup"><span data-stu-id="5cc9a-112">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.plannerFavoritePlanReferenceCollection"
}-->

```json
{
  "jd8S5gOaFk2S8aWCIAJz42QAAxtD": {
    "@odata.type": "microsoft.graph.plannerFavoritePlanReference",
    "orderHint": "8586866870001551087",
    "planTitle": "Customer reviews"
  },
  "uZWtCtli30CGoWLIWSat1mQAC0ai": {
    "@odata.type": "microsoft.graph.plannerFavoritePlanReference",
    "orderHint": "8586848705198093378",
    "planTitle": "Order Management (December 2017)"
  }
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "plannerFavoritePlanReferenceCollection resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
