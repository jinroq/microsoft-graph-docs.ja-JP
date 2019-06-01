---
title: dataPolicyOperation リソースの種類
description: 送信されたデータポリシー操作を表します。 操作の状態を追跡するために必要な情報が含まれています。 たとえば、会社の管理者は、従業員の会社のデータをエクスポートするためのデータポリシー操作要求を送信し、後でその要求を追跡できます。
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 07c708ac2d46e23cc4bdcea233587c910d30fc3e
ms.sourcegitcommit: 33f1cf5b3b79bfba6a06b52d34e558a6ba327d21
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/31/2019
ms.locfileid: "34657715"
---
# <a name="datapolicyoperation-resource-type"></a><span data-ttu-id="5b654-105">dataPolicyOperation リソースの種類</span><span class="sxs-lookup"><span data-stu-id="5b654-105">dataPolicyOperation resource type</span></span>

<span data-ttu-id="5b654-106">送信されたデータポリシー操作を表します。</span><span class="sxs-lookup"><span data-stu-id="5b654-106">Represents a submitted data policy operation.</span></span> <span data-ttu-id="5b654-107">操作の状態を追跡するために必要な情報が含まれています。</span><span class="sxs-lookup"><span data-stu-id="5b654-107">It contains necessary information for tracking the status of an operation.</span></span> <span data-ttu-id="5b654-108">たとえば、会社の管理者は、従業員の会社のデータをエクスポートするためのデータポリシー操作要求を送信し、後でその要求を追跡できます。</span><span class="sxs-lookup"><span data-stu-id="5b654-108">For example, a company administrator can submit a data policy operation request to export an employee's company data, and then later track that request.</span></span>

## <a name="methods"></a><span data-ttu-id="5b654-109">メソッド</span><span class="sxs-lookup"><span data-stu-id="5b654-109">Methods</span></span>

| <span data-ttu-id="5b654-110">メソッド</span><span class="sxs-lookup"><span data-stu-id="5b654-110">Method</span></span>           | <span data-ttu-id="5b654-111">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="5b654-111">Return Type</span></span>    |<span data-ttu-id="5b654-112">説明</span><span class="sxs-lookup"><span data-stu-id="5b654-112">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="5b654-113">DataPolicyOperation を取得する</span><span class="sxs-lookup"><span data-stu-id="5b654-113">Get dataPolicyOperation</span></span>](../api/datapolicyoperation-get.md) | [<span data-ttu-id="5b654-114">dataPolicyOperation</span><span class="sxs-lookup"><span data-stu-id="5b654-114">dataPolicyOperation</span></span>](datapolicyoperation.md) |<span data-ttu-id="5b654-115">DataPolicyOperation オブジェクトのプロパティを読み取ります。</span><span class="sxs-lookup"><span data-stu-id="5b654-115">Read properties of the dataPolicyOperation object.</span></span>|

## <a name="properties"></a><span data-ttu-id="5b654-116">プロパティ</span><span class="sxs-lookup"><span data-stu-id="5b654-116">Properties</span></span>

> <span data-ttu-id="5b654-117">**注:** このリソースのすべてのプロパティは読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="5b654-117">**Note:** All properties of this resource are read-only.</span></span>

| <span data-ttu-id="5b654-118">プロパティ</span><span class="sxs-lookup"><span data-stu-id="5b654-118">Property</span></span>     | <span data-ttu-id="5b654-119">型</span><span class="sxs-lookup"><span data-stu-id="5b654-119">Type</span></span>   |<span data-ttu-id="5b654-120">説明</span><span class="sxs-lookup"><span data-stu-id="5b654-120">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="5b654-121">CompletedDateTime</span><span class="sxs-lookup"><span data-stu-id="5b654-121">completedDateTime</span></span>|<span data-ttu-id="5b654-122">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="5b654-122">DateTimeOffset</span></span>|<span data-ttu-id="5b654-123">このデータポリシー操作の要求が完了すると、ISO 8601 形式を使用して UTC 時刻であることを表します。</span><span class="sxs-lookup"><span data-stu-id="5b654-123">Represents when the request for this data policy operation was completed, in UTC time, using the ISO 8601 format.</span></span> <span data-ttu-id="5b654-124">たとえば、2014 年 1 月 1 日午前 0 時 (UTC) は、次のようになります。`'2014-01-01T00:00:00Z'`</span><span class="sxs-lookup"><span data-stu-id="5b654-124">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`.</span></span> <span data-ttu-id="5b654-125">操作が完了するまで Null 値を返します。</span><span class="sxs-lookup"><span data-stu-id="5b654-125">Null until the operation completes.</span></span>|
|<span data-ttu-id="5b654-126">id</span><span class="sxs-lookup"><span data-stu-id="5b654-126">id</span></span>|<span data-ttu-id="5b654-127">文字列</span><span class="sxs-lookup"><span data-stu-id="5b654-127">String</span></span>| <span data-ttu-id="5b654-128">この操作の一意のキーです。</span><span class="sxs-lookup"><span data-stu-id="5b654-128">Unique key for this operation.</span></span> |
|<span data-ttu-id="5b654-129">status</span><span class="sxs-lookup"><span data-stu-id="5b654-129">status</span></span>|<span data-ttu-id="5b654-130">string</span><span class="sxs-lookup"><span data-stu-id="5b654-130">string</span></span>| <span data-ttu-id="5b654-131">可能な値は、`notStarted`、`running`、`complete`、`failed`、`unknownFutureValue` です。</span><span class="sxs-lookup"><span data-stu-id="5b654-131">Possible values are: `notStarted`, `running`, `complete`, `failed`, `unknownFutureValue`.</span></span>|
|<span data-ttu-id="5b654-132">storageLocation</span><span class="sxs-lookup"><span data-stu-id="5b654-132">storageLocation</span></span>|<span data-ttu-id="5b654-133">String</span><span class="sxs-lookup"><span data-stu-id="5b654-133">String</span></span>|<span data-ttu-id="5b654-134">エクスポート要求のためにデータがエクスポートされる場所の URL。</span><span class="sxs-lookup"><span data-stu-id="5b654-134">The URL location to where data is being exported for export requests.</span></span>|
|<span data-ttu-id="5b654-135">userId</span><span class="sxs-lookup"><span data-stu-id="5b654-135">userId</span></span>|<span data-ttu-id="5b654-136">String</span><span class="sxs-lookup"><span data-stu-id="5b654-136">String</span></span>|<span data-ttu-id="5b654-137">操作が実行されるユーザーの id。</span><span class="sxs-lookup"><span data-stu-id="5b654-137">The id for the user on whom the operation is performed.</span></span>|
|<span data-ttu-id="5b654-138">submittedDateTime</span><span class="sxs-lookup"><span data-stu-id="5b654-138">submittedDateTime</span></span>|<span data-ttu-id="5b654-139">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="5b654-139">DateTimeOffset</span></span>|<span data-ttu-id="5b654-140">このデータ操作の要求が送信された時点 (UTC 時間) を表す ISO 8601 形式を使用します。</span><span class="sxs-lookup"><span data-stu-id="5b654-140">Represents when the request for this data operation was submitted, in UTC time, using the ISO 8601 format.</span></span> <span data-ttu-id="5b654-141">たとえば、2014 年 1 月 1 日午前 0 時 (UTC) は、次のようになります。`'2014-01-01T00:00:00Z'`</span><span class="sxs-lookup"><span data-stu-id="5b654-141">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|
|<span data-ttu-id="5b654-142">progress</span><span class="sxs-lookup"><span data-stu-id="5b654-142">progress</span></span>|<span data-ttu-id="5b654-143">2 行分</span><span class="sxs-lookup"><span data-stu-id="5b654-143">Double</span></span>|<span data-ttu-id="5b654-144">操作の進行状況を指定します。</span><span class="sxs-lookup"><span data-stu-id="5b654-144">Specifies the progress of an operation.</span></span>|

## <a name="relationships"></a><span data-ttu-id="5b654-145">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="5b654-145">Relationships</span></span>
<span data-ttu-id="5b654-146">なし</span><span class="sxs-lookup"><span data-stu-id="5b654-146">None</span></span>


## <a name="json-representation"></a><span data-ttu-id="5b654-147">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="5b654-147">JSON representation</span></span>

<span data-ttu-id="5b654-148">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="5b654-148">Here is a JSON representation of the resource.</span></span>

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
  "submittedDateTime": "String (timestamp)",
  "progress": "Double"
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
