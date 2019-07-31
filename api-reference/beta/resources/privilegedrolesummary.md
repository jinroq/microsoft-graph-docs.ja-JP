---
title: privilegedRoleSummary リソースの種類
description: 特定の役割の統計の概要。
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
author: ''
ms.openlocfilehash: 30c9cfb93f8d20d30ad86d0f36019e87eae0ab65
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "35965720"
---
# <a name="privilegedrolesummary-resource-type"></a><span data-ttu-id="64f38-103">privilegedRoleSummary リソースの種類</span><span class="sxs-lookup"><span data-stu-id="64f38-103">privilegedRoleSummary resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="64f38-104">特定の役割の統計の概要。</span><span class="sxs-lookup"><span data-stu-id="64f38-104">The statistics summary for a particular role.</span></span>


## <a name="methods"></a><span data-ttu-id="64f38-105">メソッド</span><span class="sxs-lookup"><span data-stu-id="64f38-105">Methods</span></span>

| <span data-ttu-id="64f38-106">メソッド</span><span class="sxs-lookup"><span data-stu-id="64f38-106">Method</span></span>           | <span data-ttu-id="64f38-107">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="64f38-107">Return Type</span></span>    |<span data-ttu-id="64f38-108">説明</span><span class="sxs-lookup"><span data-stu-id="64f38-108">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="64f38-109">privilegedRoleSummary を取得する</span><span class="sxs-lookup"><span data-stu-id="64f38-109">Get privilegedRoleSummary</span></span>](../api/privilegedrolesummary-get.md) | [<span data-ttu-id="64f38-110">privilegedRoleSummary</span><span class="sxs-lookup"><span data-stu-id="64f38-110">privilegedRoleSummary</span></span>](privilegedrolesummary.md) |<span data-ttu-id="64f38-111">PrivilegedRoleSummary オブジェクトのプロパティとリレーションシップを読み取ります。</span><span class="sxs-lookup"><span data-stu-id="64f38-111">Read properties and relationships of privilegedRoleSummary object.</span></span>|

## <a name="properties"></a><span data-ttu-id="64f38-112">プロパティ</span><span class="sxs-lookup"><span data-stu-id="64f38-112">Properties</span></span>
| <span data-ttu-id="64f38-113">プロパティ</span><span class="sxs-lookup"><span data-stu-id="64f38-113">Property</span></span>     | <span data-ttu-id="64f38-114">型</span><span class="sxs-lookup"><span data-stu-id="64f38-114">Type</span></span>   |<span data-ttu-id="64f38-115">説明</span><span class="sxs-lookup"><span data-stu-id="64f38-115">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="64f38-116">elevatedCount</span><span class="sxs-lookup"><span data-stu-id="64f38-116">elevatedCount</span></span>|<span data-ttu-id="64f38-117">int32</span><span class="sxs-lookup"><span data-stu-id="64f38-117">int32</span></span>|<span data-ttu-id="64f38-118">役割が割り当てられていて、役割がアクティブ化されているユーザーの数。</span><span class="sxs-lookup"><span data-stu-id="64f38-118">The number of users that have the role assigned and the role is activated.</span></span>|
|<span data-ttu-id="64f38-119">id</span><span class="sxs-lookup"><span data-stu-id="64f38-119">id</span></span>|<span data-ttu-id="64f38-120">string</span><span class="sxs-lookup"><span data-stu-id="64f38-120">string</span></span>| <span data-ttu-id="64f38-121">ロールの一意識別子。</span><span class="sxs-lookup"><span data-stu-id="64f38-121">The unique identifier for the role.</span></span> <span data-ttu-id="64f38-122">読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="64f38-122">Read-only.</span></span>|
|<span data-ttu-id="64f38-123">managedCount</span><span class="sxs-lookup"><span data-stu-id="64f38-123">managedCount</span></span>|<span data-ttu-id="64f38-124">int32</span><span class="sxs-lookup"><span data-stu-id="64f38-124">int32</span></span>|<span data-ttu-id="64f38-125">役割が割り当てられているが、その役割が非アクティブ化されたユーザーの数。</span><span class="sxs-lookup"><span data-stu-id="64f38-125">The number of users that have the role assigned but the role is deactivated.</span></span>|
|<span data-ttu-id="64f38-126">mfaEnabled</span><span class="sxs-lookup"><span data-stu-id="64f38-126">mfaEnabled</span></span>|<span data-ttu-id="64f38-127">ブール値</span><span class="sxs-lookup"><span data-stu-id="64f38-127">boolean</span></span>|<span data-ttu-id="64f38-128">役割のライセンス認証が MFA を必要とする場合は**true** 。</span><span class="sxs-lookup"><span data-stu-id="64f38-128">**true** if the role activation requires MFA.</span></span> <span data-ttu-id="64f38-129">役割のライセンス認証が MFA を必要としない場合は**false** 。</span><span class="sxs-lookup"><span data-stu-id="64f38-129">**false** if the role activation doesn't require MFA.</span></span>|
|<span data-ttu-id="64f38-130">status</span><span class="sxs-lookup"><span data-stu-id="64f38-130">status</span></span>|<span data-ttu-id="64f38-131">string</span><span class="sxs-lookup"><span data-stu-id="64f38-131">string</span></span>| <span data-ttu-id="64f38-132">可能な値は、`ok`、`bad` です。</span><span class="sxs-lookup"><span data-stu-id="64f38-132">Possible values are: `ok`, `bad`.</span></span> <span data-ttu-id="64f38-133">値は、の比率 (managedCount/ユーザーカウント) によって決まります。</span><span class="sxs-lookup"><span data-stu-id="64f38-133">The value depends on the ratio of (managedCount / usersCount).</span></span> <span data-ttu-id="64f38-134">比率が定義済みのしきい値よりも小さい`ok`場合は、が返されます。</span><span class="sxs-lookup"><span data-stu-id="64f38-134">If the ratio is less than a predefined threshold, `ok` is returned.</span></span> <span data-ttu-id="64f38-135">それ以外`bad`の場合は、が返されます。</span><span class="sxs-lookup"><span data-stu-id="64f38-135">Otherwise, `bad` is returned.</span></span>|
|<span data-ttu-id="64f38-136">usersCount</span><span class="sxs-lookup"><span data-stu-id="64f38-136">usersCount</span></span>|<span data-ttu-id="64f38-137">int32</span><span class="sxs-lookup"><span data-stu-id="64f38-137">int32</span></span>|<span data-ttu-id="64f38-138">役割に割り当てられているユーザーの数。</span><span class="sxs-lookup"><span data-stu-id="64f38-138">The number of users that are assigned with the role.</span></span>|

## <a name="relationships"></a><span data-ttu-id="64f38-139">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="64f38-139">Relationships</span></span>
<span data-ttu-id="64f38-140">なし</span><span class="sxs-lookup"><span data-stu-id="64f38-140">None</span></span>


## <a name="json-representation"></a><span data-ttu-id="64f38-141">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="64f38-141">JSON representation</span></span>

<span data-ttu-id="64f38-142">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="64f38-142">Here is a JSON representation of the resource.</span></span>

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
