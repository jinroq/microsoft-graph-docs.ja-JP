---
title: onenoteOperation リソースの種類
description: OneNote の特定の長時間操作の状態。
author: Jewan-microsoft
ms.openlocfilehash: 7835c150cbc06915aa8d4e8f8bf1e1257f341ee4
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 12/18/2018
ms.locfileid: "27338676"
---
# <a name="onenoteoperation-resource-type"></a><span data-ttu-id="5a3ad-103">onenoteOperation リソースの種類</span><span class="sxs-lookup"><span data-stu-id="5a3ad-103">onenoteOperation resource type</span></span>

> <span data-ttu-id="5a3ad-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="5a3ad-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="5a3ad-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="5a3ad-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="5a3ad-106">OneNote の特定の長時間操作の状態。</span><span class="sxs-lookup"><span data-stu-id="5a3ad-106">The status of certain long-running OneNote operations.</span></span>

## <a name="json-representation"></a><span data-ttu-id="5a3ad-107">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="5a3ad-107">JSON representation</span></span>

<span data-ttu-id="5a3ad-108">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="5a3ad-108">Here is a JSON representation of the resource.</span></span>

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
## <a name="properties"></a><span data-ttu-id="5a3ad-109">プロパティ</span><span class="sxs-lookup"><span data-stu-id="5a3ad-109">Properties</span></span>
| <span data-ttu-id="5a3ad-110">プロパティ</span><span class="sxs-lookup"><span data-stu-id="5a3ad-110">Property</span></span>     | <span data-ttu-id="5a3ad-111">種類</span><span class="sxs-lookup"><span data-stu-id="5a3ad-111">Type</span></span>   |<span data-ttu-id="5a3ad-112">説明</span><span class="sxs-lookup"><span data-stu-id="5a3ad-112">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="5a3ad-113">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="5a3ad-113">createdDateTime</span></span>| <span data-ttu-id="5a3ad-114">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="5a3ad-114">DateTimeOffset</span></span> |<span data-ttu-id="5a3ad-115">操作の開始時刻です。</span><span class="sxs-lookup"><span data-stu-id="5a3ad-115">The start time of the operation.</span></span>|
|<span data-ttu-id="5a3ad-116">error</span><span class="sxs-lookup"><span data-stu-id="5a3ad-116">error</span></span>|[<span data-ttu-id="5a3ad-117">onenoteOperationError</span><span class="sxs-lookup"><span data-stu-id="5a3ad-117">onenoteOperationError</span></span>](onenoteoperationerror.md)|<span data-ttu-id="5a3ad-118">操作によって返されるエラーです。</span><span class="sxs-lookup"><span data-stu-id="5a3ad-118">The error returned by the operation.</span></span>|
|<span data-ttu-id="5a3ad-119">ID</span><span class="sxs-lookup"><span data-stu-id="5a3ad-119">id</span></span>|<span data-ttu-id="5a3ad-120">string</span><span class="sxs-lookup"><span data-stu-id="5a3ad-120">string</span></span>|<span data-ttu-id="5a3ad-121">操作 ID です。読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="5a3ad-121">The operation id. Read-only.</span></span>|
|<span data-ttu-id="5a3ad-122">lastActionDateTime</span><span class="sxs-lookup"><span data-stu-id="5a3ad-122">lastActionDateTime</span></span>| <span data-ttu-id="5a3ad-123">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="5a3ad-123">DateTimeOffset</span></span> |<span data-ttu-id="5a3ad-124">操作の最後の操作の時間です。</span><span class="sxs-lookup"><span data-stu-id="5a3ad-124">The time of the last action of the operation.</span></span>|
|<span data-ttu-id="5a3ad-125">resourceId</span><span class="sxs-lookup"><span data-stu-id="5a3ad-125">resourceId</span></span>|<span data-ttu-id="5a3ad-126">string</span><span class="sxs-lookup"><span data-stu-id="5a3ad-126">string</span></span>|<span data-ttu-id="5a3ad-127">リソース ID。</span><span class="sxs-lookup"><span data-stu-id="5a3ad-127">The resource id.</span></span>|
|<span data-ttu-id="5a3ad-128">resourceLocation</span><span class="sxs-lookup"><span data-stu-id="5a3ad-128">resourceLocation</span></span>|<span data-ttu-id="5a3ad-129">string</span><span class="sxs-lookup"><span data-stu-id="5a3ad-129">string</span></span>|<span data-ttu-id="5a3ad-p102">オブジェクトのリソース URI。たとえば、コピーしたページまたはセクションのリソース URI。</span><span class="sxs-lookup"><span data-stu-id="5a3ad-p102">The resource URI for the object. For example, the resource URI for a copied page or section.</span></span> |
|<span data-ttu-id="5a3ad-132">status</span><span class="sxs-lookup"><span data-stu-id="5a3ad-132">status</span></span>|<span data-ttu-id="5a3ad-133">string</span><span class="sxs-lookup"><span data-stu-id="5a3ad-133">string</span></span>|<span data-ttu-id="5a3ad-134">操作の現在の状態: `notstarted`、`running`、`completed`、`failed`</span><span class="sxs-lookup"><span data-stu-id="5a3ad-134">The current status of the operation: `notstarted`, `running`, `completed`, `failed`</span></span> |
|<span data-ttu-id="5a3ad-135">percentComplete</span><span class="sxs-lookup"><span data-stu-id="5a3ad-135">percentComplete</span></span>|<span data-ttu-id="5a3ad-136">string</span><span class="sxs-lookup"><span data-stu-id="5a3ad-136">string</span></span>|<span data-ttu-id="5a3ad-137">操作がまだ `running` の状態の場合の操作達成率。</span><span class="sxs-lookup"><span data-stu-id="5a3ad-137">The operation percent complete if the operation is still in `running` status</span></span>

## <a name="relationships"></a><span data-ttu-id="5a3ad-138">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="5a3ad-138">Relationships</span></span>
<span data-ttu-id="5a3ad-139">なし</span><span class="sxs-lookup"><span data-stu-id="5a3ad-139">None</span></span>


## <a name="methods"></a><span data-ttu-id="5a3ad-140">メソッド</span><span class="sxs-lookup"><span data-stu-id="5a3ad-140">Methods</span></span>

| <span data-ttu-id="5a3ad-141">メソッド</span><span class="sxs-lookup"><span data-stu-id="5a3ad-141">Method</span></span>           | <span data-ttu-id="5a3ad-142">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="5a3ad-142">Return Type</span></span>    |<span data-ttu-id="5a3ad-143">説明</span><span class="sxs-lookup"><span data-stu-id="5a3ad-143">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="5a3ad-144">操作の取得</span><span class="sxs-lookup"><span data-stu-id="5a3ad-144">Get operation</span></span>](../api/onenoteoperation-get.md) | [<span data-ttu-id="5a3ad-145">onenoteOperation</span><span class="sxs-lookup"><span data-stu-id="5a3ad-145">onenoteOperation</span></span>](onenoteoperation.md) |<span data-ttu-id="5a3ad-146">操作の現在の状態を取得します。</span><span class="sxs-lookup"><span data-stu-id="5a3ad-146">Get the status of the operation.</span></span> |

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "onenoteOperation resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
