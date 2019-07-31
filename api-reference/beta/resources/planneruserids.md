---
title: plannerUserIds リソースの種類
description: '**PlannerUserIds**リソースは、プランを共有しているユーザー id のリストを表します。 これはオープン型です。 Office 365 グループを使用している場合は、グループのメンバーシップを管理するグループの API を使用して、グループの計画を共有します。 このコレクションにグループの既存のメンバーを追加することもできます。ただし、グループが所有しているプランにアクセスするためには必要ありません。'
localization_priority: Normal
author: TarkanSevilmis
ms.prod: planner
doc_type: resourcePageType
ms.openlocfilehash: 3382da3131040f6ae3dc78102ac6e5d64a23695c
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "35965846"
---
# <a name="planneruserids-resource-type"></a><span data-ttu-id="45fdf-106">plannerUserIds リソースの種類</span><span class="sxs-lookup"><span data-stu-id="45fdf-106">plannerUserIds resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="45fdf-107">**PlannerUserIds**リソースは、[プラン](plannerplan.md)を共有しているユーザー id のリストを表します。</span><span class="sxs-lookup"><span data-stu-id="45fdf-107">The **plannerUserIds** resource represents the list of users ids that a [plan](plannerplan.md) is shared with.</span></span> <span data-ttu-id="45fdf-108">これはオープン型です。</span><span class="sxs-lookup"><span data-stu-id="45fdf-108">This is an Open Type.</span></span> <span data-ttu-id="45fdf-109">Office 365 グループを使用している場合は、グループのメンバーシップを管理するグループの API を使用して、グループ[の](group.md)計画を共有します。</span><span class="sxs-lookup"><span data-stu-id="45fdf-109">If you are leveraging Office 365 Groups, use the Groups API to manage group membership to share the [group's](group.md) plan.</span></span> <span data-ttu-id="45fdf-110">このコレクションにグループの既存のメンバーを追加することもできます。ただし、グループが所有しているプランにアクセスするためには必要ありません。</span><span class="sxs-lookup"><span data-stu-id="45fdf-110">You can also add existing members of the group to this collection though it is not required for them to access the plan owned by the group.</span></span>


## <a name="properties"></a><span data-ttu-id="45fdf-111">プロパティ</span><span class="sxs-lookup"><span data-stu-id="45fdf-111">Properties</span></span>
<span data-ttu-id="45fdf-112">オープン型のプロパティは、クライアントで定義できます。</span><span class="sxs-lookup"><span data-stu-id="45fdf-112">Properties of an Open Type can be defined by the client.</span></span> <span data-ttu-id="45fdf-113">この場合、クライアントは、値が`true`ブール値のプロパティとしてユーザー id を提供する必要があります。</span><span class="sxs-lookup"><span data-stu-id="45fdf-113">In this case, the client should provide user ids as properties with their values being the `true` boolean.</span></span> <span data-ttu-id="45fdf-114">ユーザー id を共有しなくなった場合、プロパティの値を`false` boolean に設定することによってプロパティが自動的に削除されます。</span><span class="sxs-lookup"><span data-stu-id="45fdf-114">When user ids are no longer shared with, properties are automatically removed by setting their values to the `false` boolean.</span></span>


## <a name="json-representation"></a><span data-ttu-id="45fdf-115">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="45fdf-115">JSON representation</span></span>

<span data-ttu-id="45fdf-116">以下は、リソースの JSON 表記です</span><span class="sxs-lookup"><span data-stu-id="45fdf-116">Here is a JSON representation of the resource</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.plannerUserIds"
}-->

```json
{
  "String-value": true
}
```

<span data-ttu-id="45fdf-117">例</span><span class="sxs-lookup"><span data-stu-id="45fdf-117">// Example</span></span>
```json
{
  "400723e1-102b-43aa-aba9-f35524827084": true, // property name is user id
  "f117339e-c914-4a9c-9b66-1c062b027556": true,
  "e886d105-23b9-47e2-bde1-757e75ee4a28": true
}

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "plannerUserIds resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
