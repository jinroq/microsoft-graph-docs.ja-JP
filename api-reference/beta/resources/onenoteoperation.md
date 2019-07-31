---
title: onenoteOperation リソースの種類
description: 長時間実行されている特定の OneNote 操作の状態。
author: jewan-microsoft
localization_priority: Normal
ms.prod: onenote
doc_type: resourcePageType
ms.openlocfilehash: 3f6a8bdfc6cee8b71fb77fb7778171677acb5df9
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "35966434"
---
# <a name="onenoteoperation-resource-type"></a><span data-ttu-id="31d0b-103">onenoteOperation リソースの種類</span><span class="sxs-lookup"><span data-stu-id="31d0b-103">onenoteOperation resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="31d0b-104">長時間実行されている特定の OneNote 操作の状態。</span><span class="sxs-lookup"><span data-stu-id="31d0b-104">The status of certain long-running OneNote operations.</span></span>

## <a name="json-representation"></a><span data-ttu-id="31d0b-105">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="31d0b-105">JSON representation</span></span>

<span data-ttu-id="31d0b-106">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="31d0b-106">Here is a JSON representation of the resource.</span></span>

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
## <a name="properties"></a><span data-ttu-id="31d0b-107">プロパティ</span><span class="sxs-lookup"><span data-stu-id="31d0b-107">Properties</span></span>
| <span data-ttu-id="31d0b-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="31d0b-108">Property</span></span>     | <span data-ttu-id="31d0b-109">型</span><span class="sxs-lookup"><span data-stu-id="31d0b-109">Type</span></span>   |<span data-ttu-id="31d0b-110">説明</span><span class="sxs-lookup"><span data-stu-id="31d0b-110">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="31d0b-111">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="31d0b-111">createdDateTime</span></span>| <span data-ttu-id="31d0b-112">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="31d0b-112">DateTimeOffset</span></span> |<span data-ttu-id="31d0b-113">操作の開始時刻。</span><span class="sxs-lookup"><span data-stu-id="31d0b-113">The start time of the operation.</span></span>|
|<span data-ttu-id="31d0b-114">error</span><span class="sxs-lookup"><span data-stu-id="31d0b-114">error</span></span>|[<span data-ttu-id="31d0b-115">onenoteOperationError</span><span class="sxs-lookup"><span data-stu-id="31d0b-115">onenoteOperationError</span></span>](onenoteoperationerror.md)|<span data-ttu-id="31d0b-116">操作によって返されたエラー。</span><span class="sxs-lookup"><span data-stu-id="31d0b-116">The error returned by the operation.</span></span>|
|<span data-ttu-id="31d0b-117">id</span><span class="sxs-lookup"><span data-stu-id="31d0b-117">id</span></span>|<span data-ttu-id="31d0b-118">string</span><span class="sxs-lookup"><span data-stu-id="31d0b-118">string</span></span>|<span data-ttu-id="31d0b-119">操作 id。読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="31d0b-119">The operation id. Read-only.</span></span>|
|<span data-ttu-id="31d0b-120">lastActionDateTime</span><span class="sxs-lookup"><span data-stu-id="31d0b-120">lastActionDateTime</span></span>| <span data-ttu-id="31d0b-121">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="31d0b-121">DateTimeOffset</span></span> |<span data-ttu-id="31d0b-122">操作の最後の操作の時刻。</span><span class="sxs-lookup"><span data-stu-id="31d0b-122">The time of the last action of the operation.</span></span>|
|<span data-ttu-id="31d0b-123">resourceId</span><span class="sxs-lookup"><span data-stu-id="31d0b-123">resourceId</span></span>|<span data-ttu-id="31d0b-124">string</span><span class="sxs-lookup"><span data-stu-id="31d0b-124">string</span></span>|<span data-ttu-id="31d0b-125">リソース id。</span><span class="sxs-lookup"><span data-stu-id="31d0b-125">The resource id.</span></span>|
|<span data-ttu-id="31d0b-126">resourceLocation</span><span class="sxs-lookup"><span data-stu-id="31d0b-126">resourceLocation</span></span>|<span data-ttu-id="31d0b-127">string</span><span class="sxs-lookup"><span data-stu-id="31d0b-127">string</span></span>|<span data-ttu-id="31d0b-128">オブジェクトのリソース URI。</span><span class="sxs-lookup"><span data-stu-id="31d0b-128">The resource URI for the object.</span></span> <span data-ttu-id="31d0b-129">たとえば、コピーされたページまたはセクションのリソース URI。</span><span class="sxs-lookup"><span data-stu-id="31d0b-129">For example, the resource URI for a copied page or section.</span></span> |
|<span data-ttu-id="31d0b-130">status</span><span class="sxs-lookup"><span data-stu-id="31d0b-130">status</span></span>|<span data-ttu-id="31d0b-131">string</span><span class="sxs-lookup"><span data-stu-id="31d0b-131">string</span></span>|<span data-ttu-id="31d0b-132">操作の現在の状態: `notstarted`、 `running` `completed`、、`failed`</span><span class="sxs-lookup"><span data-stu-id="31d0b-132">The current status of the operation: `notstarted`, `running`, `completed`, `failed`</span></span> |
|<span data-ttu-id="31d0b-133">percentComplete</span><span class="sxs-lookup"><span data-stu-id="31d0b-133">percentComplete</span></span>|<span data-ttu-id="31d0b-134">string</span><span class="sxs-lookup"><span data-stu-id="31d0b-134">string</span></span>|<span data-ttu-id="31d0b-135">操作がまだ状態の`running`場合の操作達成率。</span><span class="sxs-lookup"><span data-stu-id="31d0b-135">The operation percent complete if the operation is still in `running` status</span></span>

## <a name="relationships"></a><span data-ttu-id="31d0b-136">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="31d0b-136">Relationships</span></span>
<span data-ttu-id="31d0b-137">なし</span><span class="sxs-lookup"><span data-stu-id="31d0b-137">None</span></span>


## <a name="methods"></a><span data-ttu-id="31d0b-138">メソッド</span><span class="sxs-lookup"><span data-stu-id="31d0b-138">Methods</span></span>

| <span data-ttu-id="31d0b-139">メソッド</span><span class="sxs-lookup"><span data-stu-id="31d0b-139">Method</span></span>           | <span data-ttu-id="31d0b-140">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="31d0b-140">Return Type</span></span>    |<span data-ttu-id="31d0b-141">説明</span><span class="sxs-lookup"><span data-stu-id="31d0b-141">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="31d0b-142">操作を取得する</span><span class="sxs-lookup"><span data-stu-id="31d0b-142">Get operation</span></span>](../api/onenoteoperation-get.md) | [<span data-ttu-id="31d0b-143">onenoteOperation</span><span class="sxs-lookup"><span data-stu-id="31d0b-143">onenoteOperation</span></span>](onenoteoperation.md) |<span data-ttu-id="31d0b-144">操作の状態を取得します。</span><span class="sxs-lookup"><span data-stu-id="31d0b-144">Get the status of the operation.</span></span> |

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
