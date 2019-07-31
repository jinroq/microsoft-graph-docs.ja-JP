---
title: filter リソースの種類
description: アプリケーションにどのオブジェクトをプロビジョニングするかを指定します。 たとえば、US にあるユーザーのみをプロビジョニングする場合があります。 スコープフィルターが指定されている場合、フィルターを満たしていないオブジェクトは、同期中にスキップされます。
localization_priority: Normal
doc_type: resourcePageType
author: davidmu1
ms.prod: microsoft-identity-platform
ms.openlocfilehash: afc100b7f75554506a7752036dc9bdeb856ca72f
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "35964829"
---
# <a name="filter-resource-type"></a><span data-ttu-id="9834e-105">filter リソースの種類</span><span class="sxs-lookup"><span data-stu-id="9834e-105">filter resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="9834e-106">アプリケーションにどのオブジェクトをプロビジョニングするかを指定します。</span><span class="sxs-lookup"><span data-stu-id="9834e-106">Determines which objects should be provisioned to the application.</span></span> <span data-ttu-id="9834e-107">たとえば、US にあるユーザーのみをプロビジョニングする場合があります。</span><span class="sxs-lookup"><span data-stu-id="9834e-107">For example, you might want to only provision users that are located in the US.</span></span> <span data-ttu-id="9834e-108">スコープフィルターが指定されている場合、フィルターを満たしていないオブジェクトは、同期中にスキップされます。</span><span class="sxs-lookup"><span data-stu-id="9834e-108">When a scoping filter is present, objects that do not satisfy the filter will be skipped during synchronization.</span></span>

<span data-ttu-id="9834e-109">フィルターは、[オブジェクトマッピング](synchronization-objectmapping.md)の一部です。</span><span class="sxs-lookup"><span data-stu-id="9834e-109">Filter is part of [object mapping](synchronization-objectmapping.md).</span></span> <span data-ttu-id="9834e-110">フィルターグループの複数のセットで構成され、各フィルターグループは1つまたは複数の句を保持します。</span><span class="sxs-lookup"><span data-stu-id="9834e-110">It consists of several sets of filter groups, and each filter group holds one or more clauses.</span></span> <span data-ttu-id="9834e-111">グループのすべての句が評価される場合にのみ、グループの`true`スコープ内でオブジェクトが考慮され`true`ます (グループは評価されます)。</span><span class="sxs-lookup"><span data-stu-id="9834e-111">An object is considered in scope for the group (the group is evaluated to `true`) only if all the clauses of the group are evaluated to `true`.</span></span>

<span data-ttu-id="9834e-112">セット内のいずれかのグループがに`true` `true`評価される場合、グループセットのスコープ内でオブジェクトが考慮されます (グループセットはに評価されます)。</span><span class="sxs-lookup"><span data-stu-id="9834e-112">An object is considered in scope for the group set (group set is evaluated to `true`) if any of the groups in the set is evaluated to `true`.</span></span>

<span data-ttu-id="9834e-113">詳細については、「[スコープフィルターを使用した属性ベースのアプリケーションのプロビジョニング](https://docs.microsoft.com/en-us/azure/active-directory/active-directory-saas-scoping-filters)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="9834e-113">For more information, see [Attribute-based application provisioning with scoping filters](https://docs.microsoft.com/en-us/azure/active-directory/active-directory-saas-scoping-filters)</span></span>

## <a name="properties"></a><span data-ttu-id="9834e-114">プロパティ</span><span class="sxs-lookup"><span data-stu-id="9834e-114">Properties</span></span>
| <span data-ttu-id="9834e-115">プロパティ</span><span class="sxs-lookup"><span data-stu-id="9834e-115">Property</span></span>     | <span data-ttu-id="9834e-116">型</span><span class="sxs-lookup"><span data-stu-id="9834e-116">Type</span></span>   |<span data-ttu-id="9834e-117">説明</span><span class="sxs-lookup"><span data-stu-id="9834e-117">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="9834e-118">カテゴリの Filtergroups</span><span class="sxs-lookup"><span data-stu-id="9834e-118">categoryFilterGroups</span></span>|<span data-ttu-id="9834e-119">[Filtergroup](synchronization-filtergroup.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="9834e-119">[filterGroup](synchronization-filtergroup.md) collection</span></span>|<span data-ttu-id="9834e-120">`*Experimental*`指定したオブジェクトが属しているかどうかを判断し、このオブジェクトマッピングの一部として処理する必要があることを決定するために使用されるフィルタグループセット。</span><span class="sxs-lookup"><span data-stu-id="9834e-120">`*Experimental*` Filter group set used to decide whether given object belongs and should be processed as part of this object mapping.</span></span> <span data-ttu-id="9834e-121">*コレクション内のいずれかのグループがに`true`評価される場合*、オブジェクトはスコープ内で考慮されます。</span><span class="sxs-lookup"><span data-stu-id="9834e-121">An object is considered in scope *if ANY of the groups in the collection is evaluated to `true`*.</span></span>|
|<span data-ttu-id="9834e-122">groups</span><span class="sxs-lookup"><span data-stu-id="9834e-122">groups</span></span>|<span data-ttu-id="9834e-123">[Filtergroup](synchronization-filtergroup.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="9834e-123">[filterGroup](synchronization-filtergroup.md) collection</span></span>|<span data-ttu-id="9834e-124">フィルターグループセットは、指定されたオブジェクトがプロビジョニングの対象になっているかどうかを判断するために使用されます。</span><span class="sxs-lookup"><span data-stu-id="9834e-124">Filter group set used to decide whether given object is in scope for provisioning.</span></span> <span data-ttu-id="9834e-125">**このフィルターは、ほとんどの場合に使用する必要があり**ます。</span><span class="sxs-lookup"><span data-stu-id="9834e-125">**This is the filter which should be used in most cases**.</span></span> <span data-ttu-id="9834e-126">オブジェクトが指定された時点でこのフィルターに適合し、フィルターの条件が満たされなくなるようにオブジェクトまたはフィルターが変更された場合は、そのようなオブジェクト \* はプロビジョニング解除されます。</span><span class="sxs-lookup"><span data-stu-id="9834e-126">If an object used to satisfy this filter at a given moment, and then the object or the filter was changed so that filter is not satisfied any longer, such object \*will get de-provisioned".</span></span> <span data-ttu-id="9834e-127">*コレクション内のいずれかのグループがに`true`評価される場合*、オブジェクトはスコープ内で考慮されます。</span><span class="sxs-lookup"><span data-stu-id="9834e-127">An object is considered in scope *if ANY of the groups in the collection is evaluated to `true`*.</span></span>|
|<span data-ttu-id="9834e-128">inputFilterGroups</span><span class="sxs-lookup"><span data-stu-id="9834e-128">inputFilterGroups</span></span>|<span data-ttu-id="9834e-129">[Filtergroup](synchronization-filtergroup.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="9834e-129">[filterGroup](synchronization-filtergroup.md) collection</span></span>|<span data-ttu-id="9834e-130">`*Experimental*`フィルタグループセットは、ディレクトリからの読み取りの初期段階でオブジェクトをフィルター処理するために使用されます。</span><span class="sxs-lookup"><span data-stu-id="9834e-130">`*Experimental*` Filter group set used to filter out objects at the early stage of reading them from the directory.</span></span> <span data-ttu-id="9834e-131">オブジェクトがこのフィルターを満たしていない場合は、それ以上処理されません。</span><span class="sxs-lookup"><span data-stu-id="9834e-131">If an object doesn't satisfy this filter it will not be processed further.</span></span> <span data-ttu-id="9834e-132">理解しておく必要がある重要な点は、オブジェクトが指定された時点でこのフィルターを満たしている場合に、フィルターが満たされなくなるようにオブジェクトまたはフィルターが変更された場合、そのようなオブジェクト*はプロビジョニング解除されません*。</span><span class="sxs-lookup"><span data-stu-id="9834e-132">Important to understand is that if an object used to satisfy this filter at a given moment, and then the object or the filter was changed so that filter is no longer satisfied, such object *will NOT get de-provisioned*.</span></span> <span data-ttu-id="9834e-133">*コレクション内のいずれかのグループがに`true`評価される場合*、オブジェクトはスコープ内で考慮されます。</span><span class="sxs-lookup"><span data-stu-id="9834e-133">An object is considered in scope *if ANY of the groups in the collection is evaluated to `true`*.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="9834e-134">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="9834e-134">JSON representation</span></span>

<span data-ttu-id="9834e-135">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="9834e-135">Here is a JSON representation of the resource.</span></span>

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
  "suppressions": []
}
-->
