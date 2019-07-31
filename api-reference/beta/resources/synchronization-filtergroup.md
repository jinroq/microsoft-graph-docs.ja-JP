---
title: filterGroup リソースの種類
description: オブジェクトがスコープ内で考慮される必要がある一連の句を定義します。 グループのすべての句が評価される場合にのみ、グループの`true`スコープ内でオブジェクトが考慮され`true`ます (グループは評価されます)。
localization_priority: Normal
doc_type: resourcePageType
author: davidmu1
ms.prod: microsoft-identity-platform
ms.openlocfilehash: dd2b30c8ffa07eab87949bf53eaa98e6d88851c1
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "36007943"
---
# <a name="filtergroup-resource-type"></a><span data-ttu-id="83906-104">filterGroup リソースの種類</span><span class="sxs-lookup"><span data-stu-id="83906-104">filterGroup resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="83906-105">オブジェクトがスコープ内で考慮される必要がある一連の句を定義します。</span><span class="sxs-lookup"><span data-stu-id="83906-105">Defines a set of clauses that an object must satisfy to be considered in scope.</span></span> <span data-ttu-id="83906-106">グループのすべての句が評価される場合にのみ、グループの`true`スコープ内でオブジェクトが考慮され`true`ます (グループは評価されます)。</span><span class="sxs-lookup"><span data-stu-id="83906-106">An object is considered in scope for the group (the group is evaluated to `true`) only if all the clauses of the group are evaluated to `true`.</span></span>

## <a name="properties"></a><span data-ttu-id="83906-107">プロパティ</span><span class="sxs-lookup"><span data-stu-id="83906-107">Properties</span></span>
| <span data-ttu-id="83906-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="83906-108">Property</span></span>     | <span data-ttu-id="83906-109">型</span><span class="sxs-lookup"><span data-stu-id="83906-109">Type</span></span>   |<span data-ttu-id="83906-110">説明</span><span class="sxs-lookup"><span data-stu-id="83906-110">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="83906-111">条項</span><span class="sxs-lookup"><span data-stu-id="83906-111">clauses</span></span>|<span data-ttu-id="83906-112">[Filterclause](synchronization-filterclause.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="83906-112">[filterClause](synchronization-filterclause.md) collection</span></span>|<span data-ttu-id="83906-113">このグループのフィルター句 (条件)。</span><span class="sxs-lookup"><span data-stu-id="83906-113">Filter clauses (conditions) of this group.</span></span> <span data-ttu-id="83906-114">フィルターグループがに`true`評価されるように、グループ内のすべての句が満たされている必要があります。</span><span class="sxs-lookup"><span data-stu-id="83906-114">All clauses in a group must be satisfied in order for the filter group to evaluate to `true`.</span></span>|
|<span data-ttu-id="83906-115">name</span><span class="sxs-lookup"><span data-stu-id="83906-115">name</span></span>|<span data-ttu-id="83906-116">String</span><span class="sxs-lookup"><span data-stu-id="83906-116">String</span></span>|<span data-ttu-id="83906-117">ユーザーが読み取ることができるフィルターグループの名前。</span><span class="sxs-lookup"><span data-stu-id="83906-117">Human-readable name of the filter group.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="83906-118">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="83906-118">JSON representation</span></span>

<span data-ttu-id="83906-119">リソースの JSON 表記を次に示します。</span><span class="sxs-lookup"><span data-stu-id="83906-119">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.filterGroup"
}-->

```json
{
  "clauses": [{"@odata.type": "microsoft.graph.filterClause"}],
  "name": "String"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "filterGroup resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
