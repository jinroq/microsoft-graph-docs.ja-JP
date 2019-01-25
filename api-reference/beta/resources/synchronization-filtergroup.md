---
title: filterGroup リソースの種類
description: スコープでオブジェクトが満たす必要がある句のセットを定義します。 オブジェクトは、グループのスコープ内と見なされます (グループが評価され、 `true`) にグループのすべての句が評価される場合にのみ`true`。
localization_priority: Normal
ms.openlocfilehash: b71bdf16d6639b5ecc8512565ccf56d592a0da58
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/24/2019
ms.locfileid: "29514188"
---
# <a name="filtergroup-resource-type"></a><span data-ttu-id="252a8-104">filterGroup リソースの種類</span><span class="sxs-lookup"><span data-stu-id="252a8-104">filterGroup resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="252a8-105">スコープでオブジェクトが満たす必要がある句のセットを定義します。</span><span class="sxs-lookup"><span data-stu-id="252a8-105">Defines a set of clauses that an object must satisfy to be considered in scope.</span></span> <span data-ttu-id="252a8-106">オブジェクトは、グループのスコープ内と見なされます (グループが評価され、 `true`) にグループのすべての句が評価される場合にのみ`true`。</span><span class="sxs-lookup"><span data-stu-id="252a8-106">An object is considered in scope for the group (the group is evaluated to `true`) only if all the clauses of the group are evaluated to `true`.</span></span>

## <a name="properties"></a><span data-ttu-id="252a8-107">プロパティ</span><span class="sxs-lookup"><span data-stu-id="252a8-107">Properties</span></span>
| <span data-ttu-id="252a8-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="252a8-108">Property</span></span>     | <span data-ttu-id="252a8-109">型</span><span class="sxs-lookup"><span data-stu-id="252a8-109">Type</span></span>   |<span data-ttu-id="252a8-110">説明</span><span class="sxs-lookup"><span data-stu-id="252a8-110">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="252a8-111">句</span><span class="sxs-lookup"><span data-stu-id="252a8-111">clauses</span></span>|<span data-ttu-id="252a8-112">[filterClause](synchronization-filterclause.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="252a8-112">[filterClause](synchronization-filterclause.md) collection</span></span>|<span data-ttu-id="252a8-113">句 (条件) をこのグループのフィルターを適用します。</span><span class="sxs-lookup"><span data-stu-id="252a8-113">Filter clauses (conditions) of this group.</span></span> <span data-ttu-id="252a8-114">グループ内のすべての句は、フィルターのグループを評価するために満たす必要があります`true`。</span><span class="sxs-lookup"><span data-stu-id="252a8-114">All clauses in a group must be satisfied in order for the filter group to evaluate to `true`.</span></span>|
|<span data-ttu-id="252a8-115">name</span><span class="sxs-lookup"><span data-stu-id="252a8-115">name</span></span>|<span data-ttu-id="252a8-116">String</span><span class="sxs-lookup"><span data-stu-id="252a8-116">String</span></span>|<span data-ttu-id="252a8-117">フィルター グループの名前を人間が判読できます。</span><span class="sxs-lookup"><span data-stu-id="252a8-117">Human-readable name of the filter group.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="252a8-118">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="252a8-118">JSON representation</span></span>

<span data-ttu-id="252a8-119">リソースの JSON 表記を次に示します。</span><span class="sxs-lookup"><span data-stu-id="252a8-119">The following is a JSON representation of the resource.</span></span>

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
