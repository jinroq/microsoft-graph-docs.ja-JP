---
title: プランリソースの種類
description: /**コレクション**リソースは、タスクに適用されているカテゴリ (またはラベル) のコレクションを表します。 このメソッドは、プランのタスクオブジェクトに含まれています。
localization_priority: Normal
author: TarkanSevilmis
ms.prod: planner
doc_type: resourcePageType
ms.openlocfilehash: 87b75da0489099edb5294df752278311b5bf2a86
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "35966056"
---
# <a name="plannerappliedcategories-resource-type"></a><span data-ttu-id="eb63e-104">プランリソースの種類</span><span class="sxs-lookup"><span data-stu-id="eb63e-104">plannerAppliedCategories resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="eb63e-105">/**コレクション**リソースは、タスクに適用されているカテゴリ (またはラベル) のコレクションを表します。</span><span class="sxs-lookup"><span data-stu-id="eb63e-105">The **AppliedCategoriesCollection** resource represents the collection of categories (or labels) that have been applied to a task.</span></span> <span data-ttu-id="eb63e-106">このメソッドは、[プランのタスク](plannertask.md)オブジェクトに含まれています。</span><span class="sxs-lookup"><span data-stu-id="eb63e-106">It is part of the [plannerTask](plannertask.md) object.</span></span>
<span data-ttu-id="eb63e-107">1つのタスクには最大6つのカテゴリを適用できます。</span><span class="sxs-lookup"><span data-stu-id="eb63e-107">There can be up to 6 categories applied to a task.</span></span> <span data-ttu-id="eb63e-108">カテゴリの説明 ( `category1` `category2`など) は、 [plan details](plannerplandetails.md)オブジェクトの一部です。</span><span class="sxs-lookup"><span data-stu-id="eb63e-108">Category descriptions, e.g. `category1`, `category2` etc., are part of the [plan details](plannerplandetails.md) object.</span></span> <span data-ttu-id="eb63e-109">これはオープン型です。</span><span class="sxs-lookup"><span data-stu-id="eb63e-109">This is an open type.</span></span>

## <a name="properties"></a><span data-ttu-id="eb63e-110">プロパティ</span><span class="sxs-lookup"><span data-stu-id="eb63e-110">Properties</span></span>
<span data-ttu-id="eb63e-111">オープン型のプロパティは、クライアントで定義できます。</span><span class="sxs-lookup"><span data-stu-id="eb63e-111">Properties of an Open Type can be defined by the client.</span></span> <span data-ttu-id="eb63e-112">この場合、クライアントは、対応するカテゴリ`category1`が`category2`タスク`category3`に`category4`適用`category5`されるとき`category6`に`true`ブール値で、、、、および/またはをプロパティとしてプロパティとして提供する必要があります。</span><span class="sxs-lookup"><span data-stu-id="eb63e-112">In this case though, the client must provide `category1`, `category2`, `category3`, `category4`, `category5` and/or `category6` as properties with their values being the `true` boolean when the corresponding categories are applied on the task.</span></span> <span data-ttu-id="eb63e-113">例を以下に示します。</span><span class="sxs-lookup"><span data-stu-id="eb63e-113">Example is shown below.</span></span> <span data-ttu-id="eb63e-114">このプロパティが適用されていない場合、プロパティの値を`false` boolean に設定すると、プロパティが自動的に削除されます。</span><span class="sxs-lookup"><span data-stu-id="eb63e-114">When they do not apply, properties are automatically removed by setting their values to the `false` boolean.</span></span> 

## <a name="json-representation"></a><span data-ttu-id="eb63e-115">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="eb63e-115">JSON representation</span></span>

<span data-ttu-id="eb63e-116">以下は、リソースの JSON 表記です</span><span class="sxs-lookup"><span data-stu-id="eb63e-116">Here is a JSON representation of the resource</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.plannerAppliedCategories"
}-->

```json
{
  "String-value": true
}
```

<span data-ttu-id="eb63e-117">例:</span><span class="sxs-lookup"><span data-stu-id="eb63e-117">Example:</span></span> 

```json
{
  "category1": true,
  "category3": true,
  "category5": true
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "plannerAppliedCategories resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
