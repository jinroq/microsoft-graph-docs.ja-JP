---
title: plannerFavoritePlanReferenceCollection リソースの種類
description: " 値は、plannerFavoritePlanReference オブジェクトです。"
author: TarkanSevilmis
ms.openlocfilehash: 056cb7b9ba728aa9dfe44ae4b90e550876461d6b
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 12/18/2018
ms.locfileid: "27344227"
---
# <a name="plannerfavoriteplanreferencecollection-resource-type"></a><span data-ttu-id="cc9fc-103">plannerFavoritePlanReferenceCollection リソースの種類</span><span class="sxs-lookup"><span data-stu-id="cc9fc-103">plannerFavoritePlanReferenceCollection resource type</span></span>

> <span data-ttu-id="cc9fc-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="cc9fc-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="cc9fc-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="cc9fc-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="cc9fc-106">**PlannerFavoritePlanReferenceCollection**リソースでは、ユーザーがお気に入りとしてマークされている計画への参照のコレクションを表します。</span><span class="sxs-lookup"><span data-stu-id="cc9fc-106">The **plannerFavoritePlanReferenceCollection** resource represents the collection of references to plans that are marked as a favorite by a user.</span></span> <span data-ttu-id="cc9fc-107">このリソースは、オープン型であり、 [plannerUser](planneruser.md)オブジェクトの一部であります。</span><span class="sxs-lookup"><span data-stu-id="cc9fc-107">This resource is an open type and is part of the [plannerUser](planneruser.md) object.</span></span> <span data-ttu-id="cc9fc-108">プロパティ名、プロパティ値のペアでは、対応する計画の ID をします。値は、 [plannerFavoritePlanReference](plannerfavoriteplanreference.md)オブジェクトです。</span><span class="sxs-lookup"><span data-stu-id="cc9fc-108">The property name in the property-value pair is the ID of the corresponding plan; the value is the [plannerFavoritePlanReference](plannerfavoriteplanreference.md) object.</span></span>


## <a name="properties"></a><span data-ttu-id="cc9fc-109">Properties</span><span class="sxs-lookup"><span data-stu-id="cc9fc-109">Properties</span></span>
<span data-ttu-id="cc9fc-110">このオープン型のプロパティを定義することができます。</span><span class="sxs-lookup"><span data-stu-id="cc9fc-110">You can define the properties of this open type.</span></span> <span data-ttu-id="cc9fc-111">プロパティ名は、 `id` [plannerPlan](plannerplan.md)リソースの値とその値は、 [plannerFavoritePlanReference](plannerfavoriteplanreference.md)オブジェクトをする必要があります。</span><span class="sxs-lookup"><span data-stu-id="cc9fc-111">The property names are `id` values of [plannerPlan](plannerplan.md) resources and their values must be [plannerFavoritePlanReference](plannerfavoriteplanreference.md) objects.</span></span> <span data-ttu-id="cc9fc-112">お気に入りの一覧で項目を削除するのにはプロパティの値を設定します`null`。</span><span class="sxs-lookup"><span data-stu-id="cc9fc-112">To remove an item in the favorites list, set the value of the property to `null`.</span></span>


## <a name="json-representation"></a><span data-ttu-id="cc9fc-113">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="cc9fc-113">JSON representation</span></span>

<span data-ttu-id="cc9fc-114">リソースの JSON 表記を次に示します。</span><span class="sxs-lookup"><span data-stu-id="cc9fc-114">The following is a JSON representation of the resource.</span></span>

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
<!-- {
  "type": "#page.annotation",
  "description": "plannerFavoritePlanReferenceCollection resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
