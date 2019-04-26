---
title: onenoteOperation リソースの種類
description: 長時間実行されている特定の OneNote 操作の状態。
author: jewan-microsoft
localization_priority: Normal
ms.prod: onenote
ms.openlocfilehash: f336021221cd86a45f8c5683a9736cc6f838a913
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/26/2019
ms.locfileid: "33341437"
---
# <a name="onenoteoperation-resource-type"></a><span data-ttu-id="658de-103">onenoteOperation リソースの種類</span><span class="sxs-lookup"><span data-stu-id="658de-103">onenoteOperation resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="658de-104">長時間実行されている特定の OneNote 操作の状態。</span><span class="sxs-lookup"><span data-stu-id="658de-104">The status of certain long-running OneNote operations.</span></span>

## <a name="json-representation"></a><span data-ttu-id="658de-105">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="658de-105">JSON representation</span></span>

<span data-ttu-id="658de-106">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="658de-106">Here is a JSON representation of the resource.</span></span>

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
## <a name="properties"></a><span data-ttu-id="658de-107">プロパティ</span><span class="sxs-lookup"><span data-stu-id="658de-107">Properties</span></span>
| <span data-ttu-id="658de-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="658de-108">Property</span></span>     | <span data-ttu-id="658de-109">型</span><span class="sxs-lookup"><span data-stu-id="658de-109">Type</span></span>   |<span data-ttu-id="658de-110">説明</span><span class="sxs-lookup"><span data-stu-id="658de-110">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="658de-111">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="658de-111">createdDateTime</span></span>| <span data-ttu-id="658de-112">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="658de-112">DateTimeOffset</span></span> |<span data-ttu-id="658de-113">操作の開始時刻。</span><span class="sxs-lookup"><span data-stu-id="658de-113">The start time of the operation.</span></span>|
|<span data-ttu-id="658de-114">error</span><span class="sxs-lookup"><span data-stu-id="658de-114">error</span></span>|[<span data-ttu-id="658de-115">onenoteOperationError</span><span class="sxs-lookup"><span data-stu-id="658de-115">onenoteOperationError</span></span>](onenoteoperationerror.md)|<span data-ttu-id="658de-116">操作によって返されたエラー。</span><span class="sxs-lookup"><span data-stu-id="658de-116">The error returned by the operation.</span></span>|
|<span data-ttu-id="658de-117">id</span><span class="sxs-lookup"><span data-stu-id="658de-117">id</span></span>|<span data-ttu-id="658de-118">string</span><span class="sxs-lookup"><span data-stu-id="658de-118">string</span></span>|<span data-ttu-id="658de-119">操作 id。読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="658de-119">The operation id. Read-only.</span></span>|
|<span data-ttu-id="658de-120">lastactiondatetime</span><span class="sxs-lookup"><span data-stu-id="658de-120">lastActionDateTime</span></span>| <span data-ttu-id="658de-121">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="658de-121">DateTimeOffset</span></span> |<span data-ttu-id="658de-122">操作の最後の操作の時刻。</span><span class="sxs-lookup"><span data-stu-id="658de-122">The time of the last action of the operation.</span></span>|
|<span data-ttu-id="658de-123">resourceId</span><span class="sxs-lookup"><span data-stu-id="658de-123">resourceId</span></span>|<span data-ttu-id="658de-124">string</span><span class="sxs-lookup"><span data-stu-id="658de-124">string</span></span>|<span data-ttu-id="658de-125">リソース id。</span><span class="sxs-lookup"><span data-stu-id="658de-125">The resource id.</span></span>|
|<span data-ttu-id="658de-126">resourceLocation</span><span class="sxs-lookup"><span data-stu-id="658de-126">resourceLocation</span></span>|<span data-ttu-id="658de-127">string</span><span class="sxs-lookup"><span data-stu-id="658de-127">string</span></span>|<span data-ttu-id="658de-128">オブジェクトのリソース URI。</span><span class="sxs-lookup"><span data-stu-id="658de-128">The resource URI for the object.</span></span> <span data-ttu-id="658de-129">たとえば、コピーされたページまたはセクションのリソース URI。</span><span class="sxs-lookup"><span data-stu-id="658de-129">For example, the resource URI for a copied page or section.</span></span> |
|<span data-ttu-id="658de-130">status</span><span class="sxs-lookup"><span data-stu-id="658de-130">status</span></span>|<span data-ttu-id="658de-131">string</span><span class="sxs-lookup"><span data-stu-id="658de-131">string</span></span>|<span data-ttu-id="658de-132">操作の現在の状態: `notstarted`、 `running` `completed`、、`failed`</span><span class="sxs-lookup"><span data-stu-id="658de-132">The current status of the operation: `notstarted`, `running`, `completed`, `failed`</span></span> |
|<span data-ttu-id="658de-133">percentComplete</span><span class="sxs-lookup"><span data-stu-id="658de-133">percentComplete</span></span>|<span data-ttu-id="658de-134">string</span><span class="sxs-lookup"><span data-stu-id="658de-134">string</span></span>|<span data-ttu-id="658de-135">操作がまだ状態の`running`場合の操作達成率。</span><span class="sxs-lookup"><span data-stu-id="658de-135">The operation percent complete if the operation is still in `running` status</span></span>

## <a name="relationships"></a><span data-ttu-id="658de-136">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="658de-136">Relationships</span></span>
<span data-ttu-id="658de-137">なし</span><span class="sxs-lookup"><span data-stu-id="658de-137">None</span></span>


## <a name="methods"></a><span data-ttu-id="658de-138">メソッド</span><span class="sxs-lookup"><span data-stu-id="658de-138">Methods</span></span>

| <span data-ttu-id="658de-139">メソッド</span><span class="sxs-lookup"><span data-stu-id="658de-139">Method</span></span>           | <span data-ttu-id="658de-140">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="658de-140">Return Type</span></span>    |<span data-ttu-id="658de-141">説明</span><span class="sxs-lookup"><span data-stu-id="658de-141">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="658de-142">操作を取得する</span><span class="sxs-lookup"><span data-stu-id="658de-142">Get operation</span></span>](../api/onenoteoperation-get.md) | [<span data-ttu-id="658de-143">onenoteOperation</span><span class="sxs-lookup"><span data-stu-id="658de-143">onenoteOperation</span></span>](onenoteoperation.md) |<span data-ttu-id="658de-144">操作の状態を取得します。</span><span class="sxs-lookup"><span data-stu-id="658de-144">Get the status of the operation.</span></span> |

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "onenoteOperation resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
