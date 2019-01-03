---
title: privilegedRoleSummary リソースの種類
description: 特定の役割の概要統計情報です。
ms.openlocfilehash: f6c66433651eff188ce6fdaa07c2422d3bb6e0ce
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27072986"
---
# <a name="privilegedrolesummary-resource-type"></a><span data-ttu-id="e230f-103">privilegedRoleSummary リソースの種類</span><span class="sxs-lookup"><span data-stu-id="e230f-103">privilegedRoleSummary resource type</span></span>

> <span data-ttu-id="e230f-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="e230f-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="e230f-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="e230f-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="e230f-106">特定の役割の概要統計情報です。</span><span class="sxs-lookup"><span data-stu-id="e230f-106">The statistics summary for a particular role.</span></span>


## <a name="methods"></a><span data-ttu-id="e230f-107">メソッド</span><span class="sxs-lookup"><span data-stu-id="e230f-107">Methods</span></span>

| <span data-ttu-id="e230f-108">メソッド</span><span class="sxs-lookup"><span data-stu-id="e230f-108">Method</span></span>           | <span data-ttu-id="e230f-109">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="e230f-109">Return Type</span></span>    |<span data-ttu-id="e230f-110">説明</span><span class="sxs-lookup"><span data-stu-id="e230f-110">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="e230f-111">PrivilegedRoleSummary を取得します。</span><span class="sxs-lookup"><span data-stu-id="e230f-111">Get privilegedRoleSummary</span></span>](../api/privilegedrolesummary-get.md) | [<span data-ttu-id="e230f-112">privilegedRoleSummary</span><span class="sxs-lookup"><span data-stu-id="e230f-112">privilegedRoleSummary</span></span>](privilegedrolesummary.md) |<span data-ttu-id="e230f-113">PrivilegedRoleSummary オブジェクトのプロパティと関係を参照してください。</span><span class="sxs-lookup"><span data-stu-id="e230f-113">Read properties and relationships of privilegedRoleSummary object.</span></span>|

## <a name="properties"></a><span data-ttu-id="e230f-114">プロパティ</span><span class="sxs-lookup"><span data-stu-id="e230f-114">Properties</span></span>
| <span data-ttu-id="e230f-115">プロパティ</span><span class="sxs-lookup"><span data-stu-id="e230f-115">Property</span></span>     | <span data-ttu-id="e230f-116">型</span><span class="sxs-lookup"><span data-stu-id="e230f-116">Type</span></span>   |<span data-ttu-id="e230f-117">説明</span><span class="sxs-lookup"><span data-stu-id="e230f-117">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="e230f-118">elevatedCount</span><span class="sxs-lookup"><span data-stu-id="e230f-118">elevatedCount</span></span>|<span data-ttu-id="e230f-119">int32</span><span class="sxs-lookup"><span data-stu-id="e230f-119">int32</span></span>|<span data-ttu-id="e230f-120">割り当てられているロールおよびロールを持つユーザーの数がアクティブになります。</span><span class="sxs-lookup"><span data-stu-id="e230f-120">The number of users that have the role assigned and the role is activated.</span></span>|
|<span data-ttu-id="e230f-121">ID</span><span class="sxs-lookup"><span data-stu-id="e230f-121">id</span></span>|<span data-ttu-id="e230f-122">文字列</span><span class="sxs-lookup"><span data-stu-id="e230f-122">string</span></span>| <span data-ttu-id="e230f-123">ロールの一意の識別子です。</span><span class="sxs-lookup"><span data-stu-id="e230f-123">The unique identifier for the role.</span></span> <span data-ttu-id="e230f-124">読み取り専用。</span><span class="sxs-lookup"><span data-stu-id="e230f-124">Read-only.</span></span>|
|<span data-ttu-id="e230f-125">managedCount</span><span class="sxs-lookup"><span data-stu-id="e230f-125">managedCount</span></span>|<span data-ttu-id="e230f-126">int32</span><span class="sxs-lookup"><span data-stu-id="e230f-126">int32</span></span>|<span data-ttu-id="e230f-127">役割が割り当てられているユーザーが、ロールの数が無効になります。</span><span class="sxs-lookup"><span data-stu-id="e230f-127">The number of users that have the role assigned but the role is deactivated.</span></span>|
|<span data-ttu-id="e230f-128">mfaEnabled</span><span class="sxs-lookup"><span data-stu-id="e230f-128">mfaEnabled</span></span>|<span data-ttu-id="e230f-129">ブール</span><span class="sxs-lookup"><span data-stu-id="e230f-129">boolean</span></span>|<span data-ttu-id="e230f-130">**真**の役割のアクティブ化には、MFA が必要な場合です。</span><span class="sxs-lookup"><span data-stu-id="e230f-130">**true** if the role activation requires MFA.</span></span> <span data-ttu-id="e230f-131">**false**の役割のアクティブ化は、MFA を必要としない場合。</span><span class="sxs-lookup"><span data-stu-id="e230f-131">**false** if the role activation doesn't require MFA.</span></span>|
|<span data-ttu-id="e230f-132">status</span><span class="sxs-lookup"><span data-stu-id="e230f-132">status</span></span>|<span data-ttu-id="e230f-133">文字列</span><span class="sxs-lookup"><span data-stu-id="e230f-133">string</span></span>| <span data-ttu-id="e230f-134">使用可能な値は、`ok`、`bad` です。</span><span class="sxs-lookup"><span data-stu-id="e230f-134">Possible values are: `ok`, `bad`.</span></span> <span data-ttu-id="e230f-135">値の比率によって異なります (managedCount/usersCount)。</span><span class="sxs-lookup"><span data-stu-id="e230f-135">The value depends on the ratio of (managedCount / usersCount).</span></span> <span data-ttu-id="e230f-136">割合は、定義済みのしきい値より小さい場合は、`ok`が返されます。</span><span class="sxs-lookup"><span data-stu-id="e230f-136">If the ratio is less than a predefined threshold, `ok` is returned.</span></span> <span data-ttu-id="e230f-137">それ以外の場合、`bad`が返されます。</span><span class="sxs-lookup"><span data-stu-id="e230f-137">Otherwise, `bad` is returned.</span></span>|
|<span data-ttu-id="e230f-138">usersCount</span><span class="sxs-lookup"><span data-stu-id="e230f-138">usersCount</span></span>|<span data-ttu-id="e230f-139">int32</span><span class="sxs-lookup"><span data-stu-id="e230f-139">int32</span></span>|<span data-ttu-id="e230f-140">ロールに割り当てられているユーザーの数です。</span><span class="sxs-lookup"><span data-stu-id="e230f-140">The number of users that are assigned with the role.</span></span>|

## <a name="relationships"></a><span data-ttu-id="e230f-141">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="e230f-141">Relationships</span></span>
<span data-ttu-id="e230f-142">なし</span><span class="sxs-lookup"><span data-stu-id="e230f-142">None</span></span>


## <a name="json-representation"></a><span data-ttu-id="e230f-143">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="e230f-143">JSON representation</span></span>

<span data-ttu-id="e230f-144">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="e230f-144">Here is a JSON representation of the resource.</span></span>

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
<!-- {
  "type": "#page.annotation",
  "description": "privilegedRoleSummary resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->