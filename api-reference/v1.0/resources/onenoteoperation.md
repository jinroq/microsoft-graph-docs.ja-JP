---
title: onenoteOperation リソースの種類
description: OneNote の特定の長時間操作の状態。
author: Jewan-microsoft
localization_priority: Normal
ms.openlocfilehash: 89c1d1ac3404653ae3996a95bdf40c22fdd3b7c8
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/11/2019
ms.locfileid: "27845935"
---
# <a name="onenoteoperation-resource-type"></a><span data-ttu-id="55e0a-103">onenoteOperation リソースの種類</span><span class="sxs-lookup"><span data-stu-id="55e0a-103">onenoteOperation resource type</span></span>

<span data-ttu-id="55e0a-104">OneNote の特定の長時間操作の状態。</span><span class="sxs-lookup"><span data-stu-id="55e0a-104">The status of certain long-running OneNote operations.</span></span>

## <a name="json-representation"></a><span data-ttu-id="55e0a-105">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="55e0a-105">JSON representation</span></span>

<span data-ttu-id="55e0a-106">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="55e0a-106">Here is a JSON representation of the resource.</span></span>

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
## <a name="properties"></a><span data-ttu-id="55e0a-107">プロパティ</span><span class="sxs-lookup"><span data-stu-id="55e0a-107">Properties</span></span>
| <span data-ttu-id="55e0a-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="55e0a-108">Property</span></span>     | <span data-ttu-id="55e0a-109">種類</span><span class="sxs-lookup"><span data-stu-id="55e0a-109">Type</span></span>   |<span data-ttu-id="55e0a-110">説明</span><span class="sxs-lookup"><span data-stu-id="55e0a-110">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="55e0a-111">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="55e0a-111">createdDateTime</span></span>| <span data-ttu-id="55e0a-112">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="55e0a-112">DateTimeOffset</span></span> |<span data-ttu-id="55e0a-113">操作の開始時刻です。</span><span class="sxs-lookup"><span data-stu-id="55e0a-113">The start time of the operation.</span></span>|
|<span data-ttu-id="55e0a-114">error</span><span class="sxs-lookup"><span data-stu-id="55e0a-114">error</span></span>|[<span data-ttu-id="55e0a-115">onenoteOperationError</span><span class="sxs-lookup"><span data-stu-id="55e0a-115">onenoteOperationError</span></span>](onenoteoperationerror.md)|<span data-ttu-id="55e0a-116">操作によって返されるエラーです。</span><span class="sxs-lookup"><span data-stu-id="55e0a-116">The error returned by the operation.</span></span>|
|<span data-ttu-id="55e0a-117">ID</span><span class="sxs-lookup"><span data-stu-id="55e0a-117">id</span></span>|<span data-ttu-id="55e0a-118">文字列</span><span class="sxs-lookup"><span data-stu-id="55e0a-118">string</span></span>|<span data-ttu-id="55e0a-119">操作 ID です。読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="55e0a-119">The operation id. Read-only.</span></span>|
|<span data-ttu-id="55e0a-120">lastActionDateTime</span><span class="sxs-lookup"><span data-stu-id="55e0a-120">lastActionDateTime</span></span>| <span data-ttu-id="55e0a-121">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="55e0a-121">DateTimeOffset</span></span> |<span data-ttu-id="55e0a-122">操作の最後の操作の時間です。</span><span class="sxs-lookup"><span data-stu-id="55e0a-122">The time of the last action of the operation.</span></span>|
|<span data-ttu-id="55e0a-123">resourceId</span><span class="sxs-lookup"><span data-stu-id="55e0a-123">resourceId</span></span>|<span data-ttu-id="55e0a-124">文字列</span><span class="sxs-lookup"><span data-stu-id="55e0a-124">string</span></span>|<span data-ttu-id="55e0a-125">リソース ID。</span><span class="sxs-lookup"><span data-stu-id="55e0a-125">The resource id.</span></span>|
|<span data-ttu-id="55e0a-126">resourceLocation</span><span class="sxs-lookup"><span data-stu-id="55e0a-126">resourceLocation</span></span>|<span data-ttu-id="55e0a-127">文字列</span><span class="sxs-lookup"><span data-stu-id="55e0a-127">string</span></span>|<span data-ttu-id="55e0a-p101">オブジェクトのリソース URI。たとえば、コピーしたページまたはセクションのリソース URI。</span><span class="sxs-lookup"><span data-stu-id="55e0a-p101">The resource URI for the object. For example, the resource URI for a copied page or section.</span></span> |
|<span data-ttu-id="55e0a-130">status</span><span class="sxs-lookup"><span data-stu-id="55e0a-130">status</span></span>|<span data-ttu-id="55e0a-131">文字列</span><span class="sxs-lookup"><span data-stu-id="55e0a-131">string</span></span>|<span data-ttu-id="55e0a-132">操作の現在の状態: `notstarted`、`running`、`completed`、`failed`</span><span class="sxs-lookup"><span data-stu-id="55e0a-132">The current status of the operation: `notstarted`, `running`, `completed`, `failed`</span></span> |
|<span data-ttu-id="55e0a-133">percentComplete</span><span class="sxs-lookup"><span data-stu-id="55e0a-133">percentComplete</span></span>|<span data-ttu-id="55e0a-134">文字列</span><span class="sxs-lookup"><span data-stu-id="55e0a-134">string</span></span>|<span data-ttu-id="55e0a-135">操作がまだ `running` の状態の場合の操作達成率。</span><span class="sxs-lookup"><span data-stu-id="55e0a-135">The operation percent complete if the operation is still in `running` status</span></span>

## <a name="relationships"></a><span data-ttu-id="55e0a-136">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="55e0a-136">Relationships</span></span>
<span data-ttu-id="55e0a-137">なし</span><span class="sxs-lookup"><span data-stu-id="55e0a-137">None</span></span>


## <a name="methods"></a><span data-ttu-id="55e0a-138">メソッド</span><span class="sxs-lookup"><span data-stu-id="55e0a-138">Methods</span></span>

| <span data-ttu-id="55e0a-139">メソッド</span><span class="sxs-lookup"><span data-stu-id="55e0a-139">Method</span></span>           | <span data-ttu-id="55e0a-140">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="55e0a-140">Return Type</span></span>    |<span data-ttu-id="55e0a-141">説明</span><span class="sxs-lookup"><span data-stu-id="55e0a-141">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="55e0a-142">操作の取得</span><span class="sxs-lookup"><span data-stu-id="55e0a-142">Get operation</span></span>](../api/onenoteoperation-get.md) | [<span data-ttu-id="55e0a-143">onenoteOperation</span><span class="sxs-lookup"><span data-stu-id="55e0a-143">onenoteOperation</span></span>](onenoteoperation.md) |<span data-ttu-id="55e0a-144">操作の現在の状態を取得します。</span><span class="sxs-lookup"><span data-stu-id="55e0a-144">Get the status of the operation.</span></span> |

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "onenoteOperation resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
