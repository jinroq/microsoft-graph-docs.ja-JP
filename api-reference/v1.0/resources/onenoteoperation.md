---
title: onenoteOperation リソースの種類
description: OneNote の特定の長時間操作の状態。
author: jewan-microsoft
localization_priority: Normal
ms.prod: onenote
ms.openlocfilehash: eaab313e9399e6e8724d5096b7ac29ec315889ad
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/12/2019
ms.locfileid: "27977466"
---
# <a name="onenoteoperation-resource-type"></a><span data-ttu-id="e3465-103">onenoteOperation リソースの種類</span><span class="sxs-lookup"><span data-stu-id="e3465-103">onenoteOperation resource type</span></span>

<span data-ttu-id="e3465-104">OneNote の特定の長時間操作の状態。</span><span class="sxs-lookup"><span data-stu-id="e3465-104">The status of certain long-running OneNote operations.</span></span>

## <a name="json-representation"></a><span data-ttu-id="e3465-105">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="e3465-105">JSON representation</span></span>

<span data-ttu-id="e3465-106">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="e3465-106">Here is a JSON representation of the resource.</span></span>

<!--{
  "blockType": "resource",
  "optionalProperties": [],
  "baseType": "microsoft.graph.operation",
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
## <a name="properties"></a><span data-ttu-id="e3465-107">プロパティ</span><span class="sxs-lookup"><span data-stu-id="e3465-107">Properties</span></span>
| <span data-ttu-id="e3465-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="e3465-108">Property</span></span>     | <span data-ttu-id="e3465-109">種類</span><span class="sxs-lookup"><span data-stu-id="e3465-109">Type</span></span>   |<span data-ttu-id="e3465-110">説明</span><span class="sxs-lookup"><span data-stu-id="e3465-110">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="e3465-111">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="e3465-111">createdDateTime</span></span>| <span data-ttu-id="e3465-112">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="e3465-112">DateTimeOffset</span></span> |<span data-ttu-id="e3465-113">操作の開始時刻です。</span><span class="sxs-lookup"><span data-stu-id="e3465-113">The start time of the operation.</span></span>|
|<span data-ttu-id="e3465-114">error</span><span class="sxs-lookup"><span data-stu-id="e3465-114">error</span></span>|[<span data-ttu-id="e3465-115">onenoteOperationError</span><span class="sxs-lookup"><span data-stu-id="e3465-115">onenoteOperationError</span></span>](onenoteoperationerror.md)|<span data-ttu-id="e3465-116">操作によって返されるエラーです。</span><span class="sxs-lookup"><span data-stu-id="e3465-116">The error returned by the operation.</span></span>|
|<span data-ttu-id="e3465-117">ID</span><span class="sxs-lookup"><span data-stu-id="e3465-117">id</span></span>|<span data-ttu-id="e3465-118">文字列</span><span class="sxs-lookup"><span data-stu-id="e3465-118">string</span></span>|<span data-ttu-id="e3465-119">操作 ID です。読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="e3465-119">The operation id. Read-only.</span></span>|
|<span data-ttu-id="e3465-120">lastActionDateTime</span><span class="sxs-lookup"><span data-stu-id="e3465-120">lastActionDateTime</span></span>| <span data-ttu-id="e3465-121">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="e3465-121">DateTimeOffset</span></span> |<span data-ttu-id="e3465-122">操作の最後の操作の時間です。</span><span class="sxs-lookup"><span data-stu-id="e3465-122">The time of the last action of the operation.</span></span>|
|<span data-ttu-id="e3465-123">resourceId</span><span class="sxs-lookup"><span data-stu-id="e3465-123">resourceId</span></span>|<span data-ttu-id="e3465-124">文字列</span><span class="sxs-lookup"><span data-stu-id="e3465-124">string</span></span>|<span data-ttu-id="e3465-125">リソース ID。</span><span class="sxs-lookup"><span data-stu-id="e3465-125">The resource id.</span></span>|
|<span data-ttu-id="e3465-126">resourceLocation</span><span class="sxs-lookup"><span data-stu-id="e3465-126">resourceLocation</span></span>|<span data-ttu-id="e3465-127">文字列</span><span class="sxs-lookup"><span data-stu-id="e3465-127">string</span></span>|<span data-ttu-id="e3465-p101">オブジェクトのリソース URI。たとえば、コピーしたページまたはセクションのリソース URI。</span><span class="sxs-lookup"><span data-stu-id="e3465-p101">The resource URI for the object. For example, the resource URI for a copied page or section.</span></span> |
|<span data-ttu-id="e3465-130">status</span><span class="sxs-lookup"><span data-stu-id="e3465-130">status</span></span>|<span data-ttu-id="e3465-131">文字列</span><span class="sxs-lookup"><span data-stu-id="e3465-131">string</span></span>|<span data-ttu-id="e3465-132">操作の現在の状態: `notstarted`、`running`、`completed`、`failed`</span><span class="sxs-lookup"><span data-stu-id="e3465-132">The current status of the operation: `notstarted`, `running`, `completed`, `failed`</span></span> |
|<span data-ttu-id="e3465-133">percentComplete</span><span class="sxs-lookup"><span data-stu-id="e3465-133">percentComplete</span></span>|<span data-ttu-id="e3465-134">文字列</span><span class="sxs-lookup"><span data-stu-id="e3465-134">string</span></span>|<span data-ttu-id="e3465-135">操作がまだ `running` の状態の場合の操作達成率。</span><span class="sxs-lookup"><span data-stu-id="e3465-135">The operation percent complete if the operation is still in `running` status</span></span>

## <a name="relationships"></a><span data-ttu-id="e3465-136">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="e3465-136">Relationships</span></span>
<span data-ttu-id="e3465-137">なし</span><span class="sxs-lookup"><span data-stu-id="e3465-137">None</span></span>


## <a name="methods"></a><span data-ttu-id="e3465-138">メソッド</span><span class="sxs-lookup"><span data-stu-id="e3465-138">Methods</span></span>

| <span data-ttu-id="e3465-139">メソッド</span><span class="sxs-lookup"><span data-stu-id="e3465-139">Method</span></span>           | <span data-ttu-id="e3465-140">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="e3465-140">Return Type</span></span>    |<span data-ttu-id="e3465-141">説明</span><span class="sxs-lookup"><span data-stu-id="e3465-141">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="e3465-142">操作の取得</span><span class="sxs-lookup"><span data-stu-id="e3465-142">Get operation</span></span>](../api/onenoteoperation-get.md) | [<span data-ttu-id="e3465-143">onenoteOperation</span><span class="sxs-lookup"><span data-stu-id="e3465-143">onenoteOperation</span></span>](onenoteoperation.md) |<span data-ttu-id="e3465-144">操作の現在の状態を取得します。</span><span class="sxs-lookup"><span data-stu-id="e3465-144">Get the status of the operation.</span></span> |

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "onenoteOperation resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
