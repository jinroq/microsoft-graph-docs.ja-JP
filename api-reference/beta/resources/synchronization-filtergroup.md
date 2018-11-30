---
title: filterGroup リソースの種類
description: スコープでオブジェクトが満たす必要がある句のセットを定義します。 オブジェクトは、グループのスコープ内と見なされます (グループが評価され、 `true`) にグループのすべての句が評価される場合にのみ`true`。
ms.openlocfilehash: d49f7a4364f1d8ce3e1c4daba3bb331cf9a9c001
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27072613"
---
# <a name="filtergroup-resource-type"></a><span data-ttu-id="2254e-104">filterGroup リソースの種類</span><span class="sxs-lookup"><span data-stu-id="2254e-104">filterGroup resource type</span></span>

> <span data-ttu-id="2254e-105">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="2254e-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="2254e-106">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="2254e-106">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="2254e-107">スコープでオブジェクトが満たす必要がある句のセットを定義します。</span><span class="sxs-lookup"><span data-stu-id="2254e-107">Defines a set of clauses that an object must satisfy to be considered in scope.</span></span> <span data-ttu-id="2254e-108">オブジェクトは、グループのスコープ内と見なされます (グループが評価され、 `true`) にグループのすべての句が評価される場合にのみ`true`。</span><span class="sxs-lookup"><span data-stu-id="2254e-108">An object is considered in scope for the group (the group is evaluated to `true`) only if all the clauses of the group are evaluated to `true`.</span></span>

## <a name="properties"></a><span data-ttu-id="2254e-109">プロパティ</span><span class="sxs-lookup"><span data-stu-id="2254e-109">Properties</span></span>
| <span data-ttu-id="2254e-110">プロパティ</span><span class="sxs-lookup"><span data-stu-id="2254e-110">Property</span></span>     | <span data-ttu-id="2254e-111">型</span><span class="sxs-lookup"><span data-stu-id="2254e-111">Type</span></span>   |<span data-ttu-id="2254e-112">説明</span><span class="sxs-lookup"><span data-stu-id="2254e-112">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="2254e-113">句</span><span class="sxs-lookup"><span data-stu-id="2254e-113">clauses</span></span>|<span data-ttu-id="2254e-114">[filterClause](synchronization-filterclause.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="2254e-114">[filterClause](synchronization-filterclause.md) collection</span></span>|<span data-ttu-id="2254e-115">句 (条件) をこのグループのフィルターを適用します。</span><span class="sxs-lookup"><span data-stu-id="2254e-115">Filter clauses (conditions) of this group.</span></span> <span data-ttu-id="2254e-116">グループ内のすべての句は、フィルターのグループを評価するために満たす必要があります`true`。</span><span class="sxs-lookup"><span data-stu-id="2254e-116">All clauses in a group must be satisfied in order for the filter group to evaluate to `true`.</span></span>|
|<span data-ttu-id="2254e-117">名前</span><span class="sxs-lookup"><span data-stu-id="2254e-117">name</span></span>|<span data-ttu-id="2254e-118">String</span><span class="sxs-lookup"><span data-stu-id="2254e-118">String</span></span>|<span data-ttu-id="2254e-119">フィルター グループの名前を人間が判読できます。</span><span class="sxs-lookup"><span data-stu-id="2254e-119">Human-readable name of the filter group.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="2254e-120">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="2254e-120">JSON representation</span></span>

<span data-ttu-id="2254e-121">リソースの JSON 表記を次に示します。</span><span class="sxs-lookup"><span data-stu-id="2254e-121">The following is a JSON representation of the resource.</span></span>

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
<!-- {
  "type": "#page.annotation",
  "description": "filterGroup resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->