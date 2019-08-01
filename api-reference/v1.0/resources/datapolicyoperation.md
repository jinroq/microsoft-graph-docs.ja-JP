---
title: dataPolicyOperation リソースの種類
description: 送信されたデータポリシー操作を表します。 操作の状態を追跡するために必要な情報が含まれています。 たとえば、会社の管理者は、従業員の会社のデータをエクスポートするためのデータポリシー操作要求を送信し、後でその要求を追跡できます。
author: ''
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 3c73bef8a640c950b6d85eb74ad93089aaad4f74
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "36029555"
---
# <a name="datapolicyoperation-resource-type"></a><span data-ttu-id="58817-105">dataPolicyOperation リソースの種類</span><span class="sxs-lookup"><span data-stu-id="58817-105">dataPolicyOperation resource type</span></span>

<span data-ttu-id="58817-106">送信されたデータポリシー操作を表します。</span><span class="sxs-lookup"><span data-stu-id="58817-106">Represents a submitted data policy operation.</span></span> <span data-ttu-id="58817-107">操作の状態を追跡するために必要な情報が含まれています。</span><span class="sxs-lookup"><span data-stu-id="58817-107">It contains necessary information for tracking the status of an operation.</span></span> <span data-ttu-id="58817-108">たとえば、会社の管理者は、従業員の会社のデータをエクスポートするためのデータポリシー操作要求を送信し、後でその要求を追跡できます。</span><span class="sxs-lookup"><span data-stu-id="58817-108">For example, a company administrator can submit a data policy operation request to export an employee's company data, and then later track that request.</span></span>

## <a name="methods"></a><span data-ttu-id="58817-109">メソッド</span><span class="sxs-lookup"><span data-stu-id="58817-109">Methods</span></span>

| <span data-ttu-id="58817-110">メソッド</span><span class="sxs-lookup"><span data-stu-id="58817-110">Method</span></span>           | <span data-ttu-id="58817-111">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="58817-111">Return Type</span></span>    |<span data-ttu-id="58817-112">説明</span><span class="sxs-lookup"><span data-stu-id="58817-112">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="58817-113">DataPolicyOperation を取得する</span><span class="sxs-lookup"><span data-stu-id="58817-113">Get dataPolicyOperation</span></span>](../api/datapolicyoperation-get.md) | [<span data-ttu-id="58817-114">dataPolicyOperation</span><span class="sxs-lookup"><span data-stu-id="58817-114">dataPolicyOperation</span></span>](datapolicyoperation.md) |<span data-ttu-id="58817-115">**DataPolicyOperation**オブジェクトのプロパティを取得します。</span><span class="sxs-lookup"><span data-stu-id="58817-115">Retrieve properties of the **dataPolicyOperation** object.</span></span>|
|[<span data-ttu-id="58817-116">個人データをエクスポートする</span><span class="sxs-lookup"><span data-stu-id="58817-116">Export personal data</span></span>](../api/user-exportpersonaldata.md) | <span data-ttu-id="58817-117">None</span><span class="sxs-lookup"><span data-stu-id="58817-117">None</span></span> |<span data-ttu-id="58817-118">データポリシー操作要求を送信します。組織ユーザーのデータをエクスポートするには、後で[Get dataPolicyOperation](../api/datapolicyoperation-get.md)を使用して読み取ることができます。</span><span class="sxs-lookup"><span data-stu-id="58817-118">Submit a data policy operation request to export organizational user's data which can later be read using [Get dataPolicyOperation](../api/datapolicyoperation-get.md)</span></span>|

## <a name="properties"></a><span data-ttu-id="58817-119">プロパティ</span><span class="sxs-lookup"><span data-stu-id="58817-119">Properties</span></span>

> <span data-ttu-id="58817-120">**注:** このリソースのすべてのプロパティは読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="58817-120">**Note:** All properties of this resource are read-only.</span></span>

| <span data-ttu-id="58817-121">プロパティ</span><span class="sxs-lookup"><span data-stu-id="58817-121">Property</span></span>     | <span data-ttu-id="58817-122">型</span><span class="sxs-lookup"><span data-stu-id="58817-122">Type</span></span>   |<span data-ttu-id="58817-123">説明</span><span class="sxs-lookup"><span data-stu-id="58817-123">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="58817-124">CompletedDateTime</span><span class="sxs-lookup"><span data-stu-id="58817-124">completedDateTime</span></span>|<span data-ttu-id="58817-125">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="58817-125">DateTimeOffset</span></span>|<span data-ttu-id="58817-126">このデータポリシー操作の要求が完了すると、ISO 8601 形式を使用して UTC 時刻であることを表します。</span><span class="sxs-lookup"><span data-stu-id="58817-126">Represents when the request for this data policy operation was completed, in UTC time, using the ISO 8601 format.</span></span> <span data-ttu-id="58817-127">たとえば、2014 年 1 月 1 日午前 0 時 (UTC) は、次のようになります。`'2014-01-01T00:00:00Z'`</span><span class="sxs-lookup"><span data-stu-id="58817-127">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`.</span></span> <span data-ttu-id="58817-128">操作が完了するまで Null 値を返します。</span><span class="sxs-lookup"><span data-stu-id="58817-128">Null until the operation completes.</span></span>|
|<span data-ttu-id="58817-129">id</span><span class="sxs-lookup"><span data-stu-id="58817-129">id</span></span>|<span data-ttu-id="58817-130">文字列</span><span class="sxs-lookup"><span data-stu-id="58817-130">String</span></span>| <span data-ttu-id="58817-131">この操作の一意のキーです。</span><span class="sxs-lookup"><span data-stu-id="58817-131">Unique key for this operation.</span></span> |
|<span data-ttu-id="58817-132">status</span><span class="sxs-lookup"><span data-stu-id="58817-132">status</span></span>|<span data-ttu-id="58817-133">string</span><span class="sxs-lookup"><span data-stu-id="58817-133">string</span></span>| <span data-ttu-id="58817-134">可能な値は、`notStarted`、`running`、`complete`、`failed`、`unknownFutureValue` です。</span><span class="sxs-lookup"><span data-stu-id="58817-134">Possible values are: `notStarted`, `running`, `complete`, `failed`, `unknownFutureValue`.</span></span>|
|<span data-ttu-id="58817-135">storageLocation</span><span class="sxs-lookup"><span data-stu-id="58817-135">storageLocation</span></span>|<span data-ttu-id="58817-136">String</span><span class="sxs-lookup"><span data-stu-id="58817-136">String</span></span>|<span data-ttu-id="58817-137">エクスポート要求のためにデータがエクスポートされる場所の URL。</span><span class="sxs-lookup"><span data-stu-id="58817-137">The URL location to where data is being exported for export requests.</span></span>|
|<span data-ttu-id="58817-138">userId</span><span class="sxs-lookup"><span data-stu-id="58817-138">userId</span></span>|<span data-ttu-id="58817-139">String</span><span class="sxs-lookup"><span data-stu-id="58817-139">String</span></span>|<span data-ttu-id="58817-140">操作が実行されるユーザーの id。</span><span class="sxs-lookup"><span data-stu-id="58817-140">The id for the user on whom the operation is performed.</span></span>|
|<span data-ttu-id="58817-141">submittedDateTime</span><span class="sxs-lookup"><span data-stu-id="58817-141">submittedDateTime</span></span>|<span data-ttu-id="58817-142">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="58817-142">DateTimeOffset</span></span>|<span data-ttu-id="58817-143">このデータ操作の要求が送信された時点 (UTC 時間) を表す ISO 8601 形式を使用します。</span><span class="sxs-lookup"><span data-stu-id="58817-143">Represents when the request for this data operation was submitted, in UTC time, using the ISO 8601 format.</span></span> <span data-ttu-id="58817-144">たとえば、2014 年 1 月 1 日午前 0 時 (UTC) は、次のようになります。`'2014-01-01T00:00:00Z'`</span><span class="sxs-lookup"><span data-stu-id="58817-144">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|
|<span data-ttu-id="58817-145">progress</span><span class="sxs-lookup"><span data-stu-id="58817-145">progress</span></span>|<span data-ttu-id="58817-146">String</span><span class="sxs-lookup"><span data-stu-id="58817-146">String</span></span>|<span data-ttu-id="58817-147">操作の進行状況を指定します。</span><span class="sxs-lookup"><span data-stu-id="58817-147">Specifies the progress of an operation.</span></span>|

## <a name="relationships"></a><span data-ttu-id="58817-148">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="58817-148">Relationships</span></span>
<span data-ttu-id="58817-149">なし。</span><span class="sxs-lookup"><span data-stu-id="58817-149">None.</span></span>


## <a name="json-representation"></a><span data-ttu-id="58817-150">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="58817-150">JSON representation</span></span>

<span data-ttu-id="58817-151">リソースの JSON 表記を次に示します。</span><span class="sxs-lookup"><span data-stu-id="58817-151">The following is a JSON representation of the resource.</span></span>

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
  "progress": "String (double)"
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
