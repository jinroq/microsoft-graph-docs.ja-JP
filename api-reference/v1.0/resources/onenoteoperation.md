---
title: onenoteOperation リソースの種類
description: 長時間実行されている特定の OneNote 操作の状態。
author: jewan-microsoft
localization_priority: Normal
ms.prod: onenote
ms.openlocfilehash: eaab313e9399e6e8724d5096b7ac29ec315889ad
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32462663"
---
# <a name="onenoteoperation-resource-type"></a><span data-ttu-id="f313b-103">onenoteOperation リソースの種類</span><span class="sxs-lookup"><span data-stu-id="f313b-103">onenoteOperation resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="f313b-104">長時間実行されている特定の OneNote 操作の状態。</span><span class="sxs-lookup"><span data-stu-id="f313b-104">The status of certain long-running OneNote operations.</span></span>

## <a name="json-representation"></a><span data-ttu-id="f313b-105">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="f313b-105">JSON representation</span></span>

<span data-ttu-id="f313b-106">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="f313b-106">Here is a JSON representation of the resource.</span></span>

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
## <a name="properties"></a><span data-ttu-id="f313b-107">プロパティ</span><span class="sxs-lookup"><span data-stu-id="f313b-107">Properties</span></span>
| <span data-ttu-id="f313b-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="f313b-108">Property</span></span>     | <span data-ttu-id="f313b-109">型</span><span class="sxs-lookup"><span data-stu-id="f313b-109">Type</span></span>   |<span data-ttu-id="f313b-110">説明</span><span class="sxs-lookup"><span data-stu-id="f313b-110">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="f313b-111">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="f313b-111">createdDateTime</span></span>| <span data-ttu-id="f313b-112">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="f313b-112">DateTimeOffset</span></span> |<span data-ttu-id="f313b-113">操作の開始時刻。</span><span class="sxs-lookup"><span data-stu-id="f313b-113">The start time of the operation.</span></span>|
|<span data-ttu-id="f313b-114">error</span><span class="sxs-lookup"><span data-stu-id="f313b-114">error</span></span>|[<span data-ttu-id="f313b-115">onenoteOperationError</span><span class="sxs-lookup"><span data-stu-id="f313b-115">onenoteOperationError</span></span>](onenoteoperationerror.md)|<span data-ttu-id="f313b-116">操作によって返されたエラー。</span><span class="sxs-lookup"><span data-stu-id="f313b-116">The error returned by the operation.</span></span>|
|<span data-ttu-id="f313b-117">ID</span><span class="sxs-lookup"><span data-stu-id="f313b-117">id</span></span>|<span data-ttu-id="f313b-118">string</span><span class="sxs-lookup"><span data-stu-id="f313b-118">string</span></span>|<span data-ttu-id="f313b-119">操作 id。読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="f313b-119">The operation id. Read-only.</span></span>|
|<span data-ttu-id="f313b-120">lastactiondatetime</span><span class="sxs-lookup"><span data-stu-id="f313b-120">lastActionDateTime</span></span>| <span data-ttu-id="f313b-121">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="f313b-121">DateTimeOffset</span></span> |<span data-ttu-id="f313b-122">操作の最後の操作の時刻。</span><span class="sxs-lookup"><span data-stu-id="f313b-122">The time of the last action of the operation.</span></span>|
|<span data-ttu-id="f313b-123">resourceId</span><span class="sxs-lookup"><span data-stu-id="f313b-123">resourceId</span></span>|<span data-ttu-id="f313b-124">string</span><span class="sxs-lookup"><span data-stu-id="f313b-124">string</span></span>|<span data-ttu-id="f313b-125">リソース id。</span><span class="sxs-lookup"><span data-stu-id="f313b-125">The resource id.</span></span>|
|<span data-ttu-id="f313b-126">resourceLocation</span><span class="sxs-lookup"><span data-stu-id="f313b-126">resourceLocation</span></span>|<span data-ttu-id="f313b-127">string</span><span class="sxs-lookup"><span data-stu-id="f313b-127">string</span></span>|<span data-ttu-id="f313b-128">オブジェクトのリソース URI。</span><span class="sxs-lookup"><span data-stu-id="f313b-128">The resource URI for the object.</span></span> <span data-ttu-id="f313b-129">たとえば、コピーされたページまたはセクションのリソース URI。</span><span class="sxs-lookup"><span data-stu-id="f313b-129">For example, the resource URI for a copied page or section.</span></span> |
|<span data-ttu-id="f313b-130">status</span><span class="sxs-lookup"><span data-stu-id="f313b-130">status</span></span>|<span data-ttu-id="f313b-131">string</span><span class="sxs-lookup"><span data-stu-id="f313b-131">string</span></span>|<span data-ttu-id="f313b-132">操作の現在の状態: `notstarted`、 `running` `completed`、、`failed`</span><span class="sxs-lookup"><span data-stu-id="f313b-132">The current status of the operation: `notstarted`, `running`, `completed`, `failed`</span></span> |
|<span data-ttu-id="f313b-133">percentComplete</span><span class="sxs-lookup"><span data-stu-id="f313b-133">percentComplete</span></span>|<span data-ttu-id="f313b-134">string</span><span class="sxs-lookup"><span data-stu-id="f313b-134">string</span></span>|<span data-ttu-id="f313b-135">操作がまだ状態の`running`場合の操作達成率。</span><span class="sxs-lookup"><span data-stu-id="f313b-135">The operation percent complete if the operation is still in `running` status</span></span>

## <a name="relationships"></a><span data-ttu-id="f313b-136">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="f313b-136">Relationships</span></span>
<span data-ttu-id="f313b-137">なし</span><span class="sxs-lookup"><span data-stu-id="f313b-137">None</span></span>


## <a name="methods"></a><span data-ttu-id="f313b-138">メソッド</span><span class="sxs-lookup"><span data-stu-id="f313b-138">Methods</span></span>

| <span data-ttu-id="f313b-139">メソッド</span><span class="sxs-lookup"><span data-stu-id="f313b-139">Method</span></span>           | <span data-ttu-id="f313b-140">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="f313b-140">Return Type</span></span>    |<span data-ttu-id="f313b-141">説明</span><span class="sxs-lookup"><span data-stu-id="f313b-141">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="f313b-142">操作を取得する</span><span class="sxs-lookup"><span data-stu-id="f313b-142">Get operation</span></span>](../api/onenoteoperation-get.md) | [<span data-ttu-id="f313b-143">onenoteOperation</span><span class="sxs-lookup"><span data-stu-id="f313b-143">onenoteOperation</span></span>](onenoteoperation.md) |<span data-ttu-id="f313b-144">操作の状態を取得します。</span><span class="sxs-lookup"><span data-stu-id="f313b-144">Get the status of the operation.</span></span> |

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
