---
title: filtergroup リソースの種類
description: オブジェクトがスコープ内で考慮される必要がある一連の句を定義します。 グループのすべての句が評価される場合にのみ、グループの`true`スコープ内でオブジェクトが考慮され`true`ます (グループは評価されます)。
localization_priority: Normal
ms.openlocfilehash: b71bdf16d6639b5ecc8512565ccf56d592a0da58
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32582032"
---
# <a name="filtergroup-resource-type"></a><span data-ttu-id="b2715-104">filtergroup リソースの種類</span><span class="sxs-lookup"><span data-stu-id="b2715-104">filterGroup resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="b2715-105">オブジェクトがスコープ内で考慮される必要がある一連の句を定義します。</span><span class="sxs-lookup"><span data-stu-id="b2715-105">Defines a set of clauses that an object must satisfy to be considered in scope.</span></span> <span data-ttu-id="b2715-106">グループのすべての句が評価される場合にのみ、グループの`true`スコープ内でオブジェクトが考慮され`true`ます (グループは評価されます)。</span><span class="sxs-lookup"><span data-stu-id="b2715-106">An object is considered in scope for the group (the group is evaluated to `true`) only if all the clauses of the group are evaluated to `true`.</span></span>

## <a name="properties"></a><span data-ttu-id="b2715-107">プロパティ</span><span class="sxs-lookup"><span data-stu-id="b2715-107">Properties</span></span>
| <span data-ttu-id="b2715-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="b2715-108">Property</span></span>     | <span data-ttu-id="b2715-109">型</span><span class="sxs-lookup"><span data-stu-id="b2715-109">Type</span></span>   |<span data-ttu-id="b2715-110">説明</span><span class="sxs-lookup"><span data-stu-id="b2715-110">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="b2715-111">条項</span><span class="sxs-lookup"><span data-stu-id="b2715-111">clauses</span></span>|<span data-ttu-id="b2715-112">[filterclause](synchronization-filterclause.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="b2715-112">[filterClause](synchronization-filterclause.md) collection</span></span>|<span data-ttu-id="b2715-113">このグループのフィルター句 (条件)。</span><span class="sxs-lookup"><span data-stu-id="b2715-113">Filter clauses (conditions) of this group.</span></span> <span data-ttu-id="b2715-114">フィルターグループがに`true`評価されるように、グループ内のすべての句が満たされている必要があります。</span><span class="sxs-lookup"><span data-stu-id="b2715-114">All clauses in a group must be satisfied in order for the filter group to evaluate to `true`.</span></span>|
|<span data-ttu-id="b2715-115">name</span><span class="sxs-lookup"><span data-stu-id="b2715-115">name</span></span>|<span data-ttu-id="b2715-116">String</span><span class="sxs-lookup"><span data-stu-id="b2715-116">String</span></span>|<span data-ttu-id="b2715-117">ユーザーが読み取ることができるフィルターグループの名前。</span><span class="sxs-lookup"><span data-stu-id="b2715-117">Human-readable name of the filter group.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="b2715-118">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="b2715-118">JSON representation</span></span>

<span data-ttu-id="b2715-119">リソースの JSON 表記を次に示します。</span><span class="sxs-lookup"><span data-stu-id="b2715-119">The following is a JSON representation of the resource.</span></span>

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
  "suppressions": [
    "Error: /api-reference/beta/resources/synchronization-filtergroup.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
