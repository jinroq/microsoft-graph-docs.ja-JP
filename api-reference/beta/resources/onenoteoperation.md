---
title: onenoteOperation リソースの種類
description: OneNote の特定の長時間操作の状態。
author: jewan-microsoft
localization_priority: Normal
ms.prod: onenote
ms.openlocfilehash: 146a1b1d9a51cc541e06fd789f987a2d39dff48a
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/24/2019
ms.locfileid: "29512851"
---
# <a name="onenoteoperation-resource-type"></a><span data-ttu-id="a180f-103">onenoteOperation リソースの種類</span><span class="sxs-lookup"><span data-stu-id="a180f-103">onenoteOperation resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="a180f-104">OneNote の特定の長時間操作の状態。</span><span class="sxs-lookup"><span data-stu-id="a180f-104">The status of certain long-running OneNote operations.</span></span>

## <a name="json-representation"></a><span data-ttu-id="a180f-105">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="a180f-105">JSON representation</span></span>

<span data-ttu-id="a180f-106">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="a180f-106">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.onenoteOperation"
}-->

```json
{
  "createdDateTime": "String (timestamp)",
  "error": {"@odata.type": "microsoft.graph.onenoteOperationError"},
  "id": "string (identifier)",
  "lastActionDateTime": "String (timestamp)",
  "resourceId": "string",
  "resourceLocation": "string",
  "status": "string",
  "percentComplete": "string"
}

```
## <a name="properties"></a><span data-ttu-id="a180f-107">プロパティ</span><span class="sxs-lookup"><span data-stu-id="a180f-107">Properties</span></span>
| <span data-ttu-id="a180f-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="a180f-108">Property</span></span>     | <span data-ttu-id="a180f-109">型</span><span class="sxs-lookup"><span data-stu-id="a180f-109">Type</span></span>   |<span data-ttu-id="a180f-110">説明</span><span class="sxs-lookup"><span data-stu-id="a180f-110">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="a180f-111">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="a180f-111">createdDateTime</span></span>| <span data-ttu-id="a180f-112">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="a180f-112">DateTimeOffset</span></span> |<span data-ttu-id="a180f-113">操作の開始時刻です。</span><span class="sxs-lookup"><span data-stu-id="a180f-113">The start time of the operation.</span></span>|
|<span data-ttu-id="a180f-114">error</span><span class="sxs-lookup"><span data-stu-id="a180f-114">error</span></span>|[<span data-ttu-id="a180f-115">onenoteOperationError</span><span class="sxs-lookup"><span data-stu-id="a180f-115">onenoteOperationError</span></span>](onenoteoperationerror.md)|<span data-ttu-id="a180f-116">操作によって返されるエラーです。</span><span class="sxs-lookup"><span data-stu-id="a180f-116">The error returned by the operation.</span></span>|
|<span data-ttu-id="a180f-117">id</span><span class="sxs-lookup"><span data-stu-id="a180f-117">id</span></span>|<span data-ttu-id="a180f-118">string</span><span class="sxs-lookup"><span data-stu-id="a180f-118">string</span></span>|<span data-ttu-id="a180f-119">操作 ID です。読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="a180f-119">The operation id. Read-only.</span></span>|
|<span data-ttu-id="a180f-120">lastActionDateTime</span><span class="sxs-lookup"><span data-stu-id="a180f-120">lastActionDateTime</span></span>| <span data-ttu-id="a180f-121">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="a180f-121">DateTimeOffset</span></span> |<span data-ttu-id="a180f-122">操作の最後の操作の時間です。</span><span class="sxs-lookup"><span data-stu-id="a180f-122">The time of the last action of the operation.</span></span>|
|<span data-ttu-id="a180f-123">resourceId</span><span class="sxs-lookup"><span data-stu-id="a180f-123">resourceId</span></span>|<span data-ttu-id="a180f-124">string</span><span class="sxs-lookup"><span data-stu-id="a180f-124">string</span></span>|<span data-ttu-id="a180f-125">リソース ID。</span><span class="sxs-lookup"><span data-stu-id="a180f-125">The resource id.</span></span>|
|<span data-ttu-id="a180f-126">resourceLocation</span><span class="sxs-lookup"><span data-stu-id="a180f-126">resourceLocation</span></span>|<span data-ttu-id="a180f-127">string</span><span class="sxs-lookup"><span data-stu-id="a180f-127">string</span></span>|<span data-ttu-id="a180f-p101">オブジェクトのリソース URI。たとえば、コピーしたページまたはセクションのリソース URI。</span><span class="sxs-lookup"><span data-stu-id="a180f-p101">The resource URI for the object. For example, the resource URI for a copied page or section.</span></span> |
|<span data-ttu-id="a180f-130">status</span><span class="sxs-lookup"><span data-stu-id="a180f-130">status</span></span>|<span data-ttu-id="a180f-131">string</span><span class="sxs-lookup"><span data-stu-id="a180f-131">string</span></span>|<span data-ttu-id="a180f-132">操作の現在の状態: `notstarted`、`running`、`completed`、`failed`</span><span class="sxs-lookup"><span data-stu-id="a180f-132">The current status of the operation: `notstarted`, `running`, `completed`, `failed`</span></span> |
|<span data-ttu-id="a180f-133">percentComplete</span><span class="sxs-lookup"><span data-stu-id="a180f-133">percentComplete</span></span>|<span data-ttu-id="a180f-134">string</span><span class="sxs-lookup"><span data-stu-id="a180f-134">string</span></span>|<span data-ttu-id="a180f-135">操作がまだ `running` の状態の場合の操作達成率。</span><span class="sxs-lookup"><span data-stu-id="a180f-135">The operation percent complete if the operation is still in `running` status</span></span>

## <a name="relationships"></a><span data-ttu-id="a180f-136">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="a180f-136">Relationships</span></span>
<span data-ttu-id="a180f-137">なし</span><span class="sxs-lookup"><span data-stu-id="a180f-137">None</span></span>


## <a name="methods"></a><span data-ttu-id="a180f-138">メソッド</span><span class="sxs-lookup"><span data-stu-id="a180f-138">Methods</span></span>

| <span data-ttu-id="a180f-139">メソッド</span><span class="sxs-lookup"><span data-stu-id="a180f-139">Method</span></span>           | <span data-ttu-id="a180f-140">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="a180f-140">Return Type</span></span>    |<span data-ttu-id="a180f-141">説明</span><span class="sxs-lookup"><span data-stu-id="a180f-141">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="a180f-142">操作の取得</span><span class="sxs-lookup"><span data-stu-id="a180f-142">Get operation</span></span>](../api/onenoteoperation-get.md) | [<span data-ttu-id="a180f-143">onenoteOperation</span><span class="sxs-lookup"><span data-stu-id="a180f-143">onenoteOperation</span></span>](onenoteoperation.md) |<span data-ttu-id="a180f-144">操作の現在の状態を取得します。</span><span class="sxs-lookup"><span data-stu-id="a180f-144">Get the status of the operation.</span></span> |

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "onenoteOperation resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/onenoteoperation.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
