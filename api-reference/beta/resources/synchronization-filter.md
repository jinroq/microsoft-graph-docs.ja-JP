---
title: filter リソースの種類
description: アプリケーションにどのオブジェクトをプロビジョニングするかを指定します。 たとえば、US にあるユーザーのみをプロビジョニングする場合があります。 スコープフィルターが指定されている場合、フィルターを満たしていないオブジェクトは、同期中にスキップされます。
localization_priority: Normal
ms.openlocfilehash: acc9f2efcfeef68ee3beda7dc720b5da5dea2b1d
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32582117"
---
# <a name="filter-resource-type"></a><span data-ttu-id="631c1-105">filter リソースの種類</span><span class="sxs-lookup"><span data-stu-id="631c1-105">filter resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="631c1-106">アプリケーションにどのオブジェクトをプロビジョニングするかを指定します。</span><span class="sxs-lookup"><span data-stu-id="631c1-106">Determines which objects should be provisioned to the application.</span></span> <span data-ttu-id="631c1-107">たとえば、US にあるユーザーのみをプロビジョニングする場合があります。</span><span class="sxs-lookup"><span data-stu-id="631c1-107">For example, you might want to only provision users that are located in the US.</span></span> <span data-ttu-id="631c1-108">スコープフィルターが指定されている場合、フィルターを満たしていないオブジェクトは、同期中にスキップされます。</span><span class="sxs-lookup"><span data-stu-id="631c1-108">When a scoping filter is present, objects that do not satisfy the filter will be skipped during synchronization.</span></span>

<span data-ttu-id="631c1-109">フィルターは、[オブジェクトマッピング](synchronization-objectmapping.md)の一部です。</span><span class="sxs-lookup"><span data-stu-id="631c1-109">Filter is part of [object mapping](synchronization-objectmapping.md).</span></span> <span data-ttu-id="631c1-110">フィルターグループの複数のセットで構成され、各フィルターグループは1つまたは複数の句を保持します。</span><span class="sxs-lookup"><span data-stu-id="631c1-110">It consists of several sets of filter groups, and each filter group holds one or more clauses.</span></span> <span data-ttu-id="631c1-111">グループのすべての句が評価される場合にのみ、グループの`true`スコープ内でオブジェクトが考慮され`true`ます (グループは評価されます)。</span><span class="sxs-lookup"><span data-stu-id="631c1-111">An object is considered in scope for the group (the group is evaluated to `true`) only if all the clauses of the group are evaluated to `true`.</span></span>

<span data-ttu-id="631c1-112">セット内のいずれかのグループがに`true` `true`評価される場合、グループセットのスコープ内でオブジェクトが考慮されます (グループセットはに評価されます)。</span><span class="sxs-lookup"><span data-stu-id="631c1-112">An object is considered in scope for the group set (group set is evaluated to `true`) if any of the groups in the set is evaluated to `true`.</span></span>

<span data-ttu-id="631c1-113">詳細については、「[スコープフィルターを使用した属性ベースのアプリケーションのプロビジョニング](https://docs.microsoft.com/en-us/azure/active-directory/active-directory-saas-scoping-filters)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="631c1-113">For more information, see [Attribute-based application provisioning with scoping filters](https://docs.microsoft.com/en-us/azure/active-directory/active-directory-saas-scoping-filters)</span></span>

## <a name="properties"></a><span data-ttu-id="631c1-114">プロパティ</span><span class="sxs-lookup"><span data-stu-id="631c1-114">Properties</span></span>
| <span data-ttu-id="631c1-115">プロパティ</span><span class="sxs-lookup"><span data-stu-id="631c1-115">Property</span></span>     | <span data-ttu-id="631c1-116">型</span><span class="sxs-lookup"><span data-stu-id="631c1-116">Type</span></span>   |<span data-ttu-id="631c1-117">説明</span><span class="sxs-lookup"><span data-stu-id="631c1-117">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="631c1-118">カテゴリの filtergroups</span><span class="sxs-lookup"><span data-stu-id="631c1-118">categoryFilterGroups</span></span>|<span data-ttu-id="631c1-119">[filtergroup](synchronization-filtergroup.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="631c1-119">[filterGroup](synchronization-filtergroup.md) collection</span></span>|<span data-ttu-id="631c1-120">`*Experimental*`指定したオブジェクトが属しているかどうかを判断し、このオブジェクトマッピングの一部として処理する必要があることを決定するために使用されるフィルタグループセット。</span><span class="sxs-lookup"><span data-stu-id="631c1-120">`*Experimental*` Filter group set used to decide whether given object belongs and should be processed as part of this object mapping.</span></span> <span data-ttu-id="631c1-121">*コレクション内のいずれかのグループがに`true`評価される場合*、オブジェクトはスコープ内で考慮されます。</span><span class="sxs-lookup"><span data-stu-id="631c1-121">An object is considered in scope *if ANY of the groups in the collection is evaluated to `true`*.</span></span>|
|<span data-ttu-id="631c1-122">groups</span><span class="sxs-lookup"><span data-stu-id="631c1-122">groups</span></span>|<span data-ttu-id="631c1-123">[filtergroup](synchronization-filtergroup.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="631c1-123">[filterGroup](synchronization-filtergroup.md) collection</span></span>|<span data-ttu-id="631c1-124">フィルターグループセットは、指定されたオブジェクトがプロビジョニングの対象になっているかどうかを判断するために使用されます。</span><span class="sxs-lookup"><span data-stu-id="631c1-124">Filter group set used to decide whether given object is in scope for provisioning.</span></span> <span data-ttu-id="631c1-125">**このフィルターは、ほとんどの場合に使用する必要があり**ます。</span><span class="sxs-lookup"><span data-stu-id="631c1-125">**This is the filter which should be used in most cases**.</span></span> <span data-ttu-id="631c1-126">オブジェクトが指定された時点でこのフィルターに適合し、フィルターの条件が満たされなくなるようにオブジェクトまたはフィルターが変更された場合は、そのようなオブジェクト \* はプロビジョニング解除されます。</span><span class="sxs-lookup"><span data-stu-id="631c1-126">If an object used to satisfy this filter at a given moment, and then the object or the filter was changed so that filter is not satisfied any longer, such object \*will get de-provisioned".</span></span> <span data-ttu-id="631c1-127">*コレクション内のいずれかのグループがに`true`評価される場合*、オブジェクトはスコープ内で考慮されます。</span><span class="sxs-lookup"><span data-stu-id="631c1-127">An object is considered in scope *if ANY of the groups in the collection is evaluated to `true`*.</span></span>|
|<span data-ttu-id="631c1-128">inputfiltergroups</span><span class="sxs-lookup"><span data-stu-id="631c1-128">inputFilterGroups</span></span>|<span data-ttu-id="631c1-129">[filtergroup](synchronization-filtergroup.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="631c1-129">[filterGroup](synchronization-filtergroup.md) collection</span></span>|<span data-ttu-id="631c1-130">`*Experimental*`フィルタグループセットは、ディレクトリからの読み取りの初期段階でオブジェクトをフィルター処理するために使用されます。</span><span class="sxs-lookup"><span data-stu-id="631c1-130">`*Experimental*` Filter group set used to filter out objects at the early stage of reading them from the directory.</span></span> <span data-ttu-id="631c1-131">オブジェクトがこのフィルターを満たしていない場合は、それ以上処理されません。</span><span class="sxs-lookup"><span data-stu-id="631c1-131">If an object doesn't satisfy this filter it will not be processed further.</span></span> <span data-ttu-id="631c1-132">理解しておく必要がある重要な点は、オブジェクトが指定された時点でこのフィルターを満たしている場合に、フィルターが満たされなくなるようにオブジェクトまたはフィルターが変更された場合、そのようなオブジェクト*はプロビジョニング解除されません*。</span><span class="sxs-lookup"><span data-stu-id="631c1-132">Important to understand is that if an object used to satisfy this filter at a given moment, and then the object or the filter was changed so that filter is no longer satisfied, such object *will NOT get de-provisioned*.</span></span> <span data-ttu-id="631c1-133">*コレクション内のいずれかのグループがに`true`評価される場合*、オブジェクトはスコープ内で考慮されます。</span><span class="sxs-lookup"><span data-stu-id="631c1-133">An object is considered in scope *if ANY of the groups in the collection is evaluated to `true`*.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="631c1-134">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="631c1-134">JSON representation</span></span>

<span data-ttu-id="631c1-135">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="631c1-135">Here is a JSON representation of the resource.</span></span>

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
