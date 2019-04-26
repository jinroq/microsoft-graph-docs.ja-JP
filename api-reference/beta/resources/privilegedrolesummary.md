---
title: privilegedRoleSummary リソースの種類
description: 特定の役割の統計の概要。
localization_priority: Normal
ms.openlocfilehash: 3e7b447f63c5f8545021508ae2dc137bef845210
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/26/2019
ms.locfileid: "33344282"
---
# <a name="privilegedrolesummary-resource-type"></a><span data-ttu-id="bf729-103">privilegedRoleSummary リソースの種類</span><span class="sxs-lookup"><span data-stu-id="bf729-103">privilegedRoleSummary resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="bf729-104">特定の役割の統計の概要。</span><span class="sxs-lookup"><span data-stu-id="bf729-104">The statistics summary for a particular role.</span></span>


## <a name="methods"></a><span data-ttu-id="bf729-105">メソッド</span><span class="sxs-lookup"><span data-stu-id="bf729-105">Methods</span></span>

| <span data-ttu-id="bf729-106">メソッド</span><span class="sxs-lookup"><span data-stu-id="bf729-106">Method</span></span>           | <span data-ttu-id="bf729-107">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="bf729-107">Return Type</span></span>    |<span data-ttu-id="bf729-108">説明</span><span class="sxs-lookup"><span data-stu-id="bf729-108">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="bf729-109">privilegedRoleSummary を取得する</span><span class="sxs-lookup"><span data-stu-id="bf729-109">Get privilegedRoleSummary</span></span>](../api/privilegedrolesummary-get.md) | [<span data-ttu-id="bf729-110">privilegedRoleSummary</span><span class="sxs-lookup"><span data-stu-id="bf729-110">privilegedRoleSummary</span></span>](privilegedrolesummary.md) |<span data-ttu-id="bf729-111">privilegedRoleSummary オブジェクトのプロパティとリレーションシップを読み取ります。</span><span class="sxs-lookup"><span data-stu-id="bf729-111">Read properties and relationships of privilegedRoleSummary object.</span></span>|

## <a name="properties"></a><span data-ttu-id="bf729-112">プロパティ</span><span class="sxs-lookup"><span data-stu-id="bf729-112">Properties</span></span>
| <span data-ttu-id="bf729-113">プロパティ</span><span class="sxs-lookup"><span data-stu-id="bf729-113">Property</span></span>     | <span data-ttu-id="bf729-114">型</span><span class="sxs-lookup"><span data-stu-id="bf729-114">Type</span></span>   |<span data-ttu-id="bf729-115">説明</span><span class="sxs-lookup"><span data-stu-id="bf729-115">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="bf729-116">elevatedCount</span><span class="sxs-lookup"><span data-stu-id="bf729-116">elevatedCount</span></span>|<span data-ttu-id="bf729-117">int32</span><span class="sxs-lookup"><span data-stu-id="bf729-117">int32</span></span>|<span data-ttu-id="bf729-118">役割が割り当てられていて、役割がアクティブ化されているユーザーの数。</span><span class="sxs-lookup"><span data-stu-id="bf729-118">The number of users that have the role assigned and the role is activated.</span></span>|
|<span data-ttu-id="bf729-119">id</span><span class="sxs-lookup"><span data-stu-id="bf729-119">id</span></span>|<span data-ttu-id="bf729-120">string</span><span class="sxs-lookup"><span data-stu-id="bf729-120">string</span></span>| <span data-ttu-id="bf729-121">ロールの一意識別子。</span><span class="sxs-lookup"><span data-stu-id="bf729-121">The unique identifier for the role.</span></span> <span data-ttu-id="bf729-122">読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="bf729-122">Read-only.</span></span>|
|<span data-ttu-id="bf729-123">managedcount</span><span class="sxs-lookup"><span data-stu-id="bf729-123">managedCount</span></span>|<span data-ttu-id="bf729-124">int32</span><span class="sxs-lookup"><span data-stu-id="bf729-124">int32</span></span>|<span data-ttu-id="bf729-125">役割が割り当てられているが、その役割が非アクティブ化されたユーザーの数。</span><span class="sxs-lookup"><span data-stu-id="bf729-125">The number of users that have the role assigned but the role is deactivated.</span></span>|
|<span data-ttu-id="bf729-126">mfaenabled</span><span class="sxs-lookup"><span data-stu-id="bf729-126">mfaEnabled</span></span>|<span data-ttu-id="bf729-127">boolean</span><span class="sxs-lookup"><span data-stu-id="bf729-127">boolean</span></span>|<span data-ttu-id="bf729-128">役割のライセンス認証が MFA を必要とする場合は**true** 。</span><span class="sxs-lookup"><span data-stu-id="bf729-128">**true** if the role activation requires MFA.</span></span> <span data-ttu-id="bf729-129">役割のライセンス認証が MFA を必要としない場合は**false** 。</span><span class="sxs-lookup"><span data-stu-id="bf729-129">**false** if the role activation doesn't require MFA.</span></span>|
|<span data-ttu-id="bf729-130">status</span><span class="sxs-lookup"><span data-stu-id="bf729-130">status</span></span>|<span data-ttu-id="bf729-131">string</span><span class="sxs-lookup"><span data-stu-id="bf729-131">string</span></span>| <span data-ttu-id="bf729-132">可能な値は、`ok`、`bad` です。</span><span class="sxs-lookup"><span data-stu-id="bf729-132">Possible values are: `ok`, `bad`.</span></span> <span data-ttu-id="bf729-133">値は、の比率 (managedcount/ユーザーカウント) によって決まります。</span><span class="sxs-lookup"><span data-stu-id="bf729-133">The value depends on the ratio of (managedCount / usersCount).</span></span> <span data-ttu-id="bf729-134">比率が定義済みのしきい値よりも小さい`ok`場合は、が返されます。</span><span class="sxs-lookup"><span data-stu-id="bf729-134">If the ratio is less than a predefined threshold, `ok` is returned.</span></span> <span data-ttu-id="bf729-135">それ以外`bad`の場合は、が返されます。</span><span class="sxs-lookup"><span data-stu-id="bf729-135">Otherwise, `bad` is returned.</span></span>|
|<span data-ttu-id="bf729-136">usersCount</span><span class="sxs-lookup"><span data-stu-id="bf729-136">usersCount</span></span>|<span data-ttu-id="bf729-137">int32</span><span class="sxs-lookup"><span data-stu-id="bf729-137">int32</span></span>|<span data-ttu-id="bf729-138">役割に割り当てられているユーザーの数。</span><span class="sxs-lookup"><span data-stu-id="bf729-138">The number of users that are assigned with the role.</span></span>|

## <a name="relationships"></a><span data-ttu-id="bf729-139">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="bf729-139">Relationships</span></span>
<span data-ttu-id="bf729-140">なし</span><span class="sxs-lookup"><span data-stu-id="bf729-140">None</span></span>


## <a name="json-representation"></a><span data-ttu-id="bf729-141">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="bf729-141">JSON representation</span></span>

<span data-ttu-id="bf729-142">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="bf729-142">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.privilegedRoleSummary"
}-->

```json
{
  "elevatedCount": 1024,
  "id": "string (identifier)",
  "managedCount": 1024,
  "mfaEnabled": true,
  "status": "string",
  "usersCount": 1024
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "privilegedRoleSummary resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
