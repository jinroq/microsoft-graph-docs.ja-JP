---
title: dataPolicyOperation リソースの種類
description: 送信されたデータ ポリシー操作を表します。 操作のステータスを追跡するために必要な情報が含まれています。 など、企業の管理者は、従業員の会社のデータをエクスポートするのにはデータのポリシーの操作要求を送信し、その要求を後で追跡できます。
ms.openlocfilehash: e6763f4050157658ea0a7f4d1e6f52668ed6e4b6
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27071957"
---
# <a name="datapolicyoperation-resource-type"></a><span data-ttu-id="af334-105">dataPolicyOperation リソースの種類</span><span class="sxs-lookup"><span data-stu-id="af334-105">dataPolicyOperation resource type</span></span>

<span data-ttu-id="af334-106">送信されたデータ ポリシー操作を表します。</span><span class="sxs-lookup"><span data-stu-id="af334-106">Represents a submitted data policy operation.</span></span> <span data-ttu-id="af334-107">操作のステータスを追跡するために必要な情報が含まれています。</span><span class="sxs-lookup"><span data-stu-id="af334-107">It contains necessary information for tracking the status of an operation.</span></span> <span data-ttu-id="af334-108">など、企業の管理者は、従業員の会社のデータをエクスポートするのにはデータのポリシーの操作要求を送信し、その要求を後で追跡できます。</span><span class="sxs-lookup"><span data-stu-id="af334-108">For example, a company administrator can submit a data policy operation request to export an employee's company data, and then later track that request.</span></span>

## <a name="methods"></a><span data-ttu-id="af334-109">メソッド</span><span class="sxs-lookup"><span data-stu-id="af334-109">Methods</span></span>

| <span data-ttu-id="af334-110">メソッド</span><span class="sxs-lookup"><span data-stu-id="af334-110">Method</span></span>           | <span data-ttu-id="af334-111">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="af334-111">Return Type</span></span>    |<span data-ttu-id="af334-112">説明</span><span class="sxs-lookup"><span data-stu-id="af334-112">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="af334-113">DataPolicyOperation を取得します。</span><span class="sxs-lookup"><span data-stu-id="af334-113">Get dataPolicyOperation</span></span>](../api/datapolicyoperation-get.md) | [<span data-ttu-id="af334-114">dataPolicyOperation</span><span class="sxs-lookup"><span data-stu-id="af334-114">dataPolicyOperation</span></span>](datapolicyoperation.md) |<span data-ttu-id="af334-115">DataPolicyOperation オブジェクトのプロパティを参照します。</span><span class="sxs-lookup"><span data-stu-id="af334-115">Read properties of the dataPolicyOperation object.</span></span>|

## <a name="properties"></a><span data-ttu-id="af334-116">プロパティ</span><span class="sxs-lookup"><span data-stu-id="af334-116">Properties</span></span>

> <span data-ttu-id="af334-117">**注:** このリソースのすべてのプロパティは、読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="af334-117">**Note:** All properties of this resource are read-only.</span></span>

| <span data-ttu-id="af334-118">プロパティ</span><span class="sxs-lookup"><span data-stu-id="af334-118">Property</span></span>     | <span data-ttu-id="af334-119">型</span><span class="sxs-lookup"><span data-stu-id="af334-119">Type</span></span>   |<span data-ttu-id="af334-120">説明</span><span class="sxs-lookup"><span data-stu-id="af334-120">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="af334-121">CompletedDateTime</span><span class="sxs-lookup"><span data-stu-id="af334-121">completedDateTime</span></span>|<span data-ttu-id="af334-122">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="af334-122">DateTimeOffset</span></span>|<span data-ttu-id="af334-123">このデータ ポリシーの操作の要求が完了すると、UTC 時刻での ISO 8601 形式を使用して表します。</span><span class="sxs-lookup"><span data-stu-id="af334-123">Represents when the request for this data policy operation was completed, in UTC time, using the ISO 8601 format.</span></span> <span data-ttu-id="af334-124">たとえば、2014 年 1 月 1 日午前 0 時 (UTC) は、次のようになります。`'2014-01-01T00:00:00Z'`</span><span class="sxs-lookup"><span data-stu-id="af334-124">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`.</span></span> <span data-ttu-id="af334-125">操作が完了するまで null になります。</span><span class="sxs-lookup"><span data-stu-id="af334-125">Null until the operation completes.</span></span>|
|<span data-ttu-id="af334-126">id</span><span class="sxs-lookup"><span data-stu-id="af334-126">id</span></span>|<span data-ttu-id="af334-127">String</span><span class="sxs-lookup"><span data-stu-id="af334-127">String</span></span>| <span data-ttu-id="af334-128">この操作に固有のキーです。</span><span class="sxs-lookup"><span data-stu-id="af334-128">Unique key for this operation.</span></span> |
|<span data-ttu-id="af334-129">status</span><span class="sxs-lookup"><span data-stu-id="af334-129">status</span></span>|<span data-ttu-id="af334-130">文字列</span><span class="sxs-lookup"><span data-stu-id="af334-130">string</span></span>| <span data-ttu-id="af334-131">可能な値は、`notStarted`、`running`、`complete`、`failed`、`unknownFutureValue` です。</span><span class="sxs-lookup"><span data-stu-id="af334-131">Possible values are: `notStarted`, `running`, `complete`, `failed`, `unknownFutureValue`.</span></span>|
|<span data-ttu-id="af334-132">storageLocation</span><span class="sxs-lookup"><span data-stu-id="af334-132">storageLocation</span></span>|<span data-ttu-id="af334-133">String</span><span class="sxs-lookup"><span data-stu-id="af334-133">String</span></span>|<span data-ttu-id="af334-134">URL の場所のデータをエクスポートするのには、要求をエクスポートします。</span><span class="sxs-lookup"><span data-stu-id="af334-134">The URL location to where data is being exported for export requests.</span></span>|
|<span data-ttu-id="af334-135">userId</span><span class="sxs-lookup"><span data-stu-id="af334-135">userId</span></span>|<span data-ttu-id="af334-136">String</span><span class="sxs-lookup"><span data-stu-id="af334-136">String</span></span>|<span data-ttu-id="af334-137">操作を実行するユーザーのユーザーの id。</span><span class="sxs-lookup"><span data-stu-id="af334-137">The id for the user on whom the operation is performed.</span></span>|
|<span data-ttu-id="af334-138">submittedDateTime</span><span class="sxs-lookup"><span data-stu-id="af334-138">submittedDateTime</span></span>|<span data-ttu-id="af334-139">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="af334-139">DateTimeOffset</span></span>|<span data-ttu-id="af334-140">このデータの操作の要求が送信された UTC 時刻での ISO 8601 形式を使用する場合を表します。</span><span class="sxs-lookup"><span data-stu-id="af334-140">Represents when the request for this data operation was submitted, in UTC time, using the ISO 8601 format.</span></span> <span data-ttu-id="af334-141">たとえば、2014 年 1 月 1 日午前 0 時 (UTC) は、次のようになります。`'2014-01-01T00:00:00Z'`</span><span class="sxs-lookup"><span data-stu-id="af334-141">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|

## <a name="relationships"></a><span data-ttu-id="af334-142">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="af334-142">Relationships</span></span>
<span data-ttu-id="af334-143">なし</span><span class="sxs-lookup"><span data-stu-id="af334-143">None</span></span>


## <a name="json-representation"></a><span data-ttu-id="af334-144">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="af334-144">JSON representation</span></span>

<span data-ttu-id="af334-145">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="af334-145">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.dataPolicyOperation"
}-->

```json
{
  "completedDateTime": "String (timestamp)",
  "id": "String (identifier)",
  "status": "string",
  "storageLocation": "String",
  "userId": "String",
  "submittedDateTime": "String (timestamp)"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "dataPolicyOperation resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
