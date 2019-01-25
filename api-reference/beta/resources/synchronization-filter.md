---
title: フィルター リソースの種類
description: アプリケーション オブジェクトを準備する必要がありますを決定します。 たとえば、米国内にあるユーザーのみを提供する可能性があります。 スコープ フィルターが存在する場合、フィルターを満たしていないオブジェクトは同期中にスキップされます。
localization_priority: Normal
ms.openlocfilehash: acc9f2efcfeef68ee3beda7dc720b5da5dea2b1d
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/24/2019
ms.locfileid: "29516680"
---
# <a name="filter-resource-type"></a><span data-ttu-id="99d58-105">フィルター リソースの種類</span><span class="sxs-lookup"><span data-stu-id="99d58-105">filter resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="99d58-106">アプリケーション オブジェクトを準備する必要がありますを決定します。</span><span class="sxs-lookup"><span data-stu-id="99d58-106">Determines which objects should be provisioned to the application.</span></span> <span data-ttu-id="99d58-107">たとえば、米国内にあるユーザーのみを提供する可能性があります。</span><span class="sxs-lookup"><span data-stu-id="99d58-107">For example, you might want to only provision users that are located in the US.</span></span> <span data-ttu-id="99d58-108">スコープ フィルターが存在する場合、フィルターを満たしていないオブジェクトは同期中にスキップされます。</span><span class="sxs-lookup"><span data-stu-id="99d58-108">When a scoping filter is present, objects that do not satisfy the filter will be skipped during synchronization.</span></span>

<span data-ttu-id="99d58-109">フィルターは、[オブジェクトのマッピング](synchronization-objectmapping.md)の一部です。</span><span class="sxs-lookup"><span data-stu-id="99d58-109">Filter is part of [object mapping](synchronization-objectmapping.md).</span></span> <span data-ttu-id="99d58-110">フィルターのグループのいくつかのセットで構成されていて、各フィルター グループが 1 つまたは複数の句を保持します。</span><span class="sxs-lookup"><span data-stu-id="99d58-110">It consists of several sets of filter groups, and each filter group holds one or more clauses.</span></span> <span data-ttu-id="99d58-111">オブジェクトは、グループのスコープ内と見なされます (グループが評価され、 `true`) にグループのすべての句が評価される場合にのみ`true`。</span><span class="sxs-lookup"><span data-stu-id="99d58-111">An object is considered in scope for the group (the group is evaluated to `true`) only if all the clauses of the group are evaluated to `true`.</span></span>

<span data-ttu-id="99d58-112">オブジェクトは、グループのスコープ内と見なされます (グループのセットが評価され、 `true`) 場合は、セット内のグループのいずれかが評価され、 `true`。</span><span class="sxs-lookup"><span data-stu-id="99d58-112">An object is considered in scope for the group set (group set is evaluated to `true`) if any of the groups in the set is evaluated to `true`.</span></span>

<span data-ttu-id="99d58-113">詳細については、[属性ベースのアプリケーションのスコープ フィルターを使用してプロビジョニング](https://docs.microsoft.com/en-us/azure/active-directory/active-directory-saas-scoping-filters)を参照してください。</span><span class="sxs-lookup"><span data-stu-id="99d58-113">For more information, see [Attribute-based application provisioning with scoping filters](https://docs.microsoft.com/en-us/azure/active-directory/active-directory-saas-scoping-filters)</span></span>

## <a name="properties"></a><span data-ttu-id="99d58-114">プロパティ</span><span class="sxs-lookup"><span data-stu-id="99d58-114">Properties</span></span>
| <span data-ttu-id="99d58-115">プロパティ</span><span class="sxs-lookup"><span data-stu-id="99d58-115">Property</span></span>     | <span data-ttu-id="99d58-116">型</span><span class="sxs-lookup"><span data-stu-id="99d58-116">Type</span></span>   |<span data-ttu-id="99d58-117">説明</span><span class="sxs-lookup"><span data-stu-id="99d58-117">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="99d58-118">categoryFilterGroups</span><span class="sxs-lookup"><span data-stu-id="99d58-118">categoryFilterGroups</span></span>|<span data-ttu-id="99d58-119">[filterGroup](synchronization-filtergroup.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="99d58-119">[filterGroup](synchronization-filtergroup.md) collection</span></span>|<span data-ttu-id="99d58-120">`*Experimental*`かどうか特定のオブジェクトが所属するグループのセットをフィルター処理し、このオブジェクトのマッピングの一部として処理する必要があります。</span><span class="sxs-lookup"><span data-stu-id="99d58-120">`*Experimental*` Filter group set used to decide whether given object belongs and should be processed as part of this object mapping.</span></span> <span data-ttu-id="99d58-121">オブジェクトがスコープ内と見なされる\*場合は、コレクション内のグループのいずれかが評価され、 `true` \*。</span><span class="sxs-lookup"><span data-stu-id="99d58-121">An object is considered in scope *if ANY of the groups in the collection is evaluated to `true`*.</span></span>|
|<span data-ttu-id="99d58-122">グループ</span><span class="sxs-lookup"><span data-stu-id="99d58-122">groups</span></span>|<span data-ttu-id="99d58-123">[filterGroup](synchronization-filtergroup.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="99d58-123">[filterGroup](synchronization-filtergroup.md) collection</span></span>|<span data-ttu-id="99d58-124">プロビジョニング用のスコープ、オブジェクトが指定されているかどうかを決定するために使用するグループ セットをフィルター処理します。</span><span class="sxs-lookup"><span data-stu-id="99d58-124">Filter group set used to decide whether given object is in scope for provisioning.</span></span> <span data-ttu-id="99d58-125">**これは、ほとんどの場合に使用するフィルター**です。</span><span class="sxs-lookup"><span data-stu-id="99d58-125">**This is the filter which should be used in most cases**.</span></span> <span data-ttu-id="99d58-126">そのフィルターではありませんので、特定の時点でこのフィルターを満たすために使用されるオブジェクトと、オブジェクトまたはフィルターが変更された場合はそのようなオブジェクトで満足できなくなった場合、\* はプロビジョニング解除」します。</span><span class="sxs-lookup"><span data-stu-id="99d58-126">If an object used to satisfy this filter at a given moment, and then the object or the filter was changed so that filter is not satisfied any longer, such object \*will get de-provisioned".</span></span> <span data-ttu-id="99d58-127">オブジェクトがスコープ内と見なされる\*場合は、コレクション内のグループのいずれかが評価され、 `true` \*。</span><span class="sxs-lookup"><span data-stu-id="99d58-127">An object is considered in scope *if ANY of the groups in the collection is evaluated to `true`*.</span></span>|
|<span data-ttu-id="99d58-128">inputFilterGroups</span><span class="sxs-lookup"><span data-stu-id="99d58-128">inputFilterGroups</span></span>|<span data-ttu-id="99d58-129">[filterGroup](synchronization-filtergroup.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="99d58-129">[filterGroup](synchronization-filtergroup.md) collection</span></span>|<span data-ttu-id="99d58-130">`*Experimental*`グループ セットのオブジェクトをディレクトリから読み取ることの初期の段階でフィルターをかけるためにフィルターを適用します。</span><span class="sxs-lookup"><span data-stu-id="99d58-130">`*Experimental*` Filter group set used to filter out objects at the early stage of reading them from the directory.</span></span> <span data-ttu-id="99d58-131">オブジェクトは、このフィルターを満たしていない場合にする処理は行われません。</span><span class="sxs-lookup"><span data-stu-id="99d58-131">If an object doesn't satisfy this filter it will not be processed further.</span></span> <span data-ttu-id="99d58-132">重要満たされる場合、オブジェクトは、特定の時点でこのフィルターを満たすために使用し、オブジェクト、またはフィルターが変更されていてそのフィルターはないことを理解するのなどのオブジェクト*が取得するが準備されていません*。</span><span class="sxs-lookup"><span data-stu-id="99d58-132">Important to understand is that if an object used to satisfy this filter at a given moment, and then the object or the filter was changed so that filter is no longer satisfied, such object *will NOT get de-provisioned*.</span></span> <span data-ttu-id="99d58-133">オブジェクトがスコープ内と見なされる\*場合は、コレクション内のグループのいずれかが評価され、 `true` \*。</span><span class="sxs-lookup"><span data-stu-id="99d58-133">An object is considered in scope *if ANY of the groups in the collection is evaluated to `true`*.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="99d58-134">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="99d58-134">JSON representation</span></span>

<span data-ttu-id="99d58-135">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="99d58-135">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.filter"
}-->

```json
{
  "categoryFilterGroups": [{"@odata.type": "microsoft.graph.filterGroup"}],
  "groups": [{"@odata.type": "microsoft.graph.filterGroup"}],
  "inputFilterGroups": [{"@odata.type": "microsoft.graph.filterGroup"}]
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "filter resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/synchronization-filter.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
