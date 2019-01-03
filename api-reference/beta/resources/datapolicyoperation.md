---
title: dataPolicyOperation リソースの種類
description: 送信されたデータ ポリシー操作を表します。 操作のステータスを追跡するために必要な情報が含まれています。 など、企業の管理者は、従業員の会社のデータをエクスポートするのにはデータのポリシーの操作要求を送信し、その要求を後で追跡できます。
ms.openlocfilehash: 6e896fdfa60b733dd91e9da573d998c1949f0d9c
ms.sourcegitcommit: 4a46cfd112c8089fc07e4e5ccdccaf415a3a0e7f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 12/05/2018
ms.locfileid: "27156034"
---
# <a name="datapolicyoperation-resource-type"></a><span data-ttu-id="9f4d6-105">dataPolicyOperation リソースの種類</span><span class="sxs-lookup"><span data-stu-id="9f4d6-105">dataPolicyOperation resource type</span></span>

<span data-ttu-id="9f4d6-106">送信されたデータ ポリシー操作を表します。</span><span class="sxs-lookup"><span data-stu-id="9f4d6-106">Represents a submitted data policy operation.</span></span> <span data-ttu-id="9f4d6-107">操作のステータスを追跡するために必要な情報が含まれています。</span><span class="sxs-lookup"><span data-stu-id="9f4d6-107">It contains necessary information for tracking the status of an operation.</span></span> <span data-ttu-id="9f4d6-108">など、企業の管理者は、従業員の会社のデータをエクスポートするのにはデータのポリシーの操作要求を送信し、その要求を後で追跡できます。</span><span class="sxs-lookup"><span data-stu-id="9f4d6-108">For example, a company administrator can submit a data policy operation request to export an employee's company data, and then later track that request.</span></span>

## <a name="methods"></a><span data-ttu-id="9f4d6-109">Methods</span><span class="sxs-lookup"><span data-stu-id="9f4d6-109">Methods</span></span>

| <span data-ttu-id="9f4d6-110">メソッド</span><span class="sxs-lookup"><span data-stu-id="9f4d6-110">Method</span></span>           | <span data-ttu-id="9f4d6-111">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="9f4d6-111">Return Type</span></span>    |<span data-ttu-id="9f4d6-112">説明</span><span class="sxs-lookup"><span data-stu-id="9f4d6-112">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="9f4d6-113">DataPolicyOperation を取得します。</span><span class="sxs-lookup"><span data-stu-id="9f4d6-113">Get dataPolicyOperation</span></span>](../api/datapolicyoperation-get.md) | [<span data-ttu-id="9f4d6-114">dataPolicyOperation</span><span class="sxs-lookup"><span data-stu-id="9f4d6-114">dataPolicyOperation</span></span>](datapolicyoperation.md) |<span data-ttu-id="9f4d6-115">DataPolicyOperation オブジェクトのプロパティを参照します。</span><span class="sxs-lookup"><span data-stu-id="9f4d6-115">Read properties of the dataPolicyOperation object.</span></span>|

## <a name="properties"></a><span data-ttu-id="9f4d6-116">プロパティ</span><span class="sxs-lookup"><span data-stu-id="9f4d6-116">Properties</span></span>

> <span data-ttu-id="9f4d6-117">**注:** このリソースのすべてのプロパティは、読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="9f4d6-117">**Note:** All properties of this resource are read-only.</span></span>

| <span data-ttu-id="9f4d6-118">プロパティ</span><span class="sxs-lookup"><span data-stu-id="9f4d6-118">Property</span></span>     | <span data-ttu-id="9f4d6-119">種類</span><span class="sxs-lookup"><span data-stu-id="9f4d6-119">Type</span></span>   |<span data-ttu-id="9f4d6-120">説明</span><span class="sxs-lookup"><span data-stu-id="9f4d6-120">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="9f4d6-121">CompletedDateTime</span><span class="sxs-lookup"><span data-stu-id="9f4d6-121">completedDateTime</span></span>|<span data-ttu-id="9f4d6-122">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="9f4d6-122">DateTimeOffset</span></span>|<span data-ttu-id="9f4d6-123">このデータ ポリシーの操作の要求が完了すると、UTC 時刻での ISO 8601 形式を使用して表します。</span><span class="sxs-lookup"><span data-stu-id="9f4d6-123">Represents when the request for this data policy operation was completed, in UTC time, using the ISO 8601 format.</span></span> <span data-ttu-id="9f4d6-124">たとえば、2014 年 1 月 1 日午前 0 時 (UTC) は、次のようになります。`'2014-01-01T00:00:00Z'`</span><span class="sxs-lookup"><span data-stu-id="9f4d6-124">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`.</span></span> <span data-ttu-id="9f4d6-125">操作が完了するまで null になります。</span><span class="sxs-lookup"><span data-stu-id="9f4d6-125">Null until the operation completes.</span></span>|
|<span data-ttu-id="9f4d6-126">id</span><span class="sxs-lookup"><span data-stu-id="9f4d6-126">id</span></span>|<span data-ttu-id="9f4d6-127">String</span><span class="sxs-lookup"><span data-stu-id="9f4d6-127">String</span></span>| <span data-ttu-id="9f4d6-128">この操作に固有のキーです。</span><span class="sxs-lookup"><span data-stu-id="9f4d6-128">Unique key for this operation.</span></span> |
|<span data-ttu-id="9f4d6-129">status</span><span class="sxs-lookup"><span data-stu-id="9f4d6-129">status</span></span>|<span data-ttu-id="9f4d6-130">文字列</span><span class="sxs-lookup"><span data-stu-id="9f4d6-130">string</span></span>| <span data-ttu-id="9f4d6-131">可能な値は、`notStarted`、`running`、`complete`、`failed`、`unknownFutureValue` です。</span><span class="sxs-lookup"><span data-stu-id="9f4d6-131">Possible values are: `notStarted`, `running`, `complete`, `failed`, `unknownFutureValue`.</span></span>|
|<span data-ttu-id="9f4d6-132">storageLocation</span><span class="sxs-lookup"><span data-stu-id="9f4d6-132">storageLocation</span></span>|<span data-ttu-id="9f4d6-133">String</span><span class="sxs-lookup"><span data-stu-id="9f4d6-133">String</span></span>|<span data-ttu-id="9f4d6-134">URL の場所のデータをエクスポートするのには、要求をエクスポートします。</span><span class="sxs-lookup"><span data-stu-id="9f4d6-134">The URL location to where data is being exported for export requests.</span></span>|
|<span data-ttu-id="9f4d6-135">userId</span><span class="sxs-lookup"><span data-stu-id="9f4d6-135">userId</span></span>|<span data-ttu-id="9f4d6-136">String</span><span class="sxs-lookup"><span data-stu-id="9f4d6-136">String</span></span>|<span data-ttu-id="9f4d6-137">操作を実行するユーザーのユーザーの id。</span><span class="sxs-lookup"><span data-stu-id="9f4d6-137">The id for the user on whom the operation is performed.</span></span>|
|<span data-ttu-id="9f4d6-138">submittedDateTime</span><span class="sxs-lookup"><span data-stu-id="9f4d6-138">submittedDateTime</span></span>|<span data-ttu-id="9f4d6-139">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="9f4d6-139">DateTimeOffset</span></span>|<span data-ttu-id="9f4d6-140">このデータの操作の要求が送信された UTC 時刻での ISO 8601 形式を使用する場合を表します。</span><span class="sxs-lookup"><span data-stu-id="9f4d6-140">Represents when the request for this data operation was submitted, in UTC time, using the ISO 8601 format.</span></span> <span data-ttu-id="9f4d6-141">たとえば、2014 年 1 月 1 日午前 0 時 (UTC) は、次のようになります。`'2014-01-01T00:00:00Z'`</span><span class="sxs-lookup"><span data-stu-id="9f4d6-141">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|
|<span data-ttu-id="9f4d6-142">進行状況</span><span class="sxs-lookup"><span data-stu-id="9f4d6-142">progress</span></span>|<span data-ttu-id="9f4d6-143">倍精度浮動小数点数</span><span class="sxs-lookup"><span data-stu-id="9f4d6-143">Double</span></span>|<span data-ttu-id="9f4d6-144">操作の進行状況を指定します。</span><span class="sxs-lookup"><span data-stu-id="9f4d6-144">Specifies the progress of an operation.</span></span>|

## <a name="relationships"></a><span data-ttu-id="9f4d6-145">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="9f4d6-145">Relationships</span></span>
<span data-ttu-id="9f4d6-146">なし</span><span class="sxs-lookup"><span data-stu-id="9f4d6-146">None</span></span>


## <a name="json-representation"></a><span data-ttu-id="9f4d6-147">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="9f4d6-147">JSON representation</span></span>

<span data-ttu-id="9f4d6-148">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="9f4d6-148">Here is a JSON representation of the resource.</span></span>

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