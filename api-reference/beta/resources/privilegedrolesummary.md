---
title: privilegedRoleSummary リソースの種類
description: 特定の役割の概要統計情報です。
localization_priority: Normal
ms.openlocfilehash: 2ed34f556f52c41729bfa108fbb6eb0c608f6b67
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/24/2019
ms.locfileid: "29513740"
---
# <a name="privilegedrolesummary-resource-type"></a><span data-ttu-id="7f151-103">privilegedRoleSummary リソースの種類</span><span class="sxs-lookup"><span data-stu-id="7f151-103">privilegedRoleSummary resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="7f151-104">特定の役割の概要統計情報です。</span><span class="sxs-lookup"><span data-stu-id="7f151-104">The statistics summary for a particular role.</span></span>


## <a name="methods"></a><span data-ttu-id="7f151-105">メソッド</span><span class="sxs-lookup"><span data-stu-id="7f151-105">Methods</span></span>

| <span data-ttu-id="7f151-106">メソッド</span><span class="sxs-lookup"><span data-stu-id="7f151-106">Method</span></span>           | <span data-ttu-id="7f151-107">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="7f151-107">Return Type</span></span>    |<span data-ttu-id="7f151-108">説明</span><span class="sxs-lookup"><span data-stu-id="7f151-108">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="7f151-109">PrivilegedRoleSummary を取得します。</span><span class="sxs-lookup"><span data-stu-id="7f151-109">Get privilegedRoleSummary</span></span>](../api/privilegedrolesummary-get.md) | [<span data-ttu-id="7f151-110">privilegedRoleSummary</span><span class="sxs-lookup"><span data-stu-id="7f151-110">privilegedRoleSummary</span></span>](privilegedrolesummary.md) |<span data-ttu-id="7f151-111">PrivilegedRoleSummary オブジェクトのプロパティと関係を参照してください。</span><span class="sxs-lookup"><span data-stu-id="7f151-111">Read properties and relationships of privilegedRoleSummary object.</span></span>|

## <a name="properties"></a><span data-ttu-id="7f151-112">プロパティ</span><span class="sxs-lookup"><span data-stu-id="7f151-112">Properties</span></span>
| <span data-ttu-id="7f151-113">プロパティ</span><span class="sxs-lookup"><span data-stu-id="7f151-113">Property</span></span>     | <span data-ttu-id="7f151-114">型</span><span class="sxs-lookup"><span data-stu-id="7f151-114">Type</span></span>   |<span data-ttu-id="7f151-115">説明</span><span class="sxs-lookup"><span data-stu-id="7f151-115">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="7f151-116">elevatedCount</span><span class="sxs-lookup"><span data-stu-id="7f151-116">elevatedCount</span></span>|<span data-ttu-id="7f151-117">int32</span><span class="sxs-lookup"><span data-stu-id="7f151-117">int32</span></span>|<span data-ttu-id="7f151-118">割り当てられているロールおよびロールを持つユーザーの数がアクティブになります。</span><span class="sxs-lookup"><span data-stu-id="7f151-118">The number of users that have the role assigned and the role is activated.</span></span>|
|<span data-ttu-id="7f151-119">id</span><span class="sxs-lookup"><span data-stu-id="7f151-119">id</span></span>|<span data-ttu-id="7f151-120">string</span><span class="sxs-lookup"><span data-stu-id="7f151-120">string</span></span>| <span data-ttu-id="7f151-121">ロールの一意の識別子です。</span><span class="sxs-lookup"><span data-stu-id="7f151-121">The unique identifier for the role.</span></span> <span data-ttu-id="7f151-122">読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="7f151-122">Read-only.</span></span>|
|<span data-ttu-id="7f151-123">managedCount</span><span class="sxs-lookup"><span data-stu-id="7f151-123">managedCount</span></span>|<span data-ttu-id="7f151-124">int32</span><span class="sxs-lookup"><span data-stu-id="7f151-124">int32</span></span>|<span data-ttu-id="7f151-125">役割が割り当てられているユーザーが、ロールの数が無効になります。</span><span class="sxs-lookup"><span data-stu-id="7f151-125">The number of users that have the role assigned but the role is deactivated.</span></span>|
|<span data-ttu-id="7f151-126">mfaEnabled</span><span class="sxs-lookup"><span data-stu-id="7f151-126">mfaEnabled</span></span>|<span data-ttu-id="7f151-127">boolean</span><span class="sxs-lookup"><span data-stu-id="7f151-127">boolean</span></span>|<span data-ttu-id="7f151-128">**真**の役割のアクティブ化には、MFA が必要な場合です。</span><span class="sxs-lookup"><span data-stu-id="7f151-128">**true** if the role activation requires MFA.</span></span> <span data-ttu-id="7f151-129">**false**の役割のアクティブ化は、MFA を必要としない場合。</span><span class="sxs-lookup"><span data-stu-id="7f151-129">**false** if the role activation doesn't require MFA.</span></span>|
|<span data-ttu-id="7f151-130">status</span><span class="sxs-lookup"><span data-stu-id="7f151-130">status</span></span>|<span data-ttu-id="7f151-131">string</span><span class="sxs-lookup"><span data-stu-id="7f151-131">string</span></span>| <span data-ttu-id="7f151-132">使用可能な値は、`ok`、`bad` です。</span><span class="sxs-lookup"><span data-stu-id="7f151-132">Possible values are: `ok`, `bad`.</span></span> <span data-ttu-id="7f151-133">値の比率によって異なります (managedCount/usersCount)。</span><span class="sxs-lookup"><span data-stu-id="7f151-133">The value depends on the ratio of (managedCount / usersCount).</span></span> <span data-ttu-id="7f151-134">割合は、定義済みのしきい値より小さい場合は、`ok`が返されます。</span><span class="sxs-lookup"><span data-stu-id="7f151-134">If the ratio is less than a predefined threshold, `ok` is returned.</span></span> <span data-ttu-id="7f151-135">それ以外の場合、`bad`が返されます。</span><span class="sxs-lookup"><span data-stu-id="7f151-135">Otherwise, `bad` is returned.</span></span>|
|<span data-ttu-id="7f151-136">usersCount</span><span class="sxs-lookup"><span data-stu-id="7f151-136">usersCount</span></span>|<span data-ttu-id="7f151-137">int32</span><span class="sxs-lookup"><span data-stu-id="7f151-137">int32</span></span>|<span data-ttu-id="7f151-138">ロールに割り当てられているユーザーの数です。</span><span class="sxs-lookup"><span data-stu-id="7f151-138">The number of users that are assigned with the role.</span></span>|

## <a name="relationships"></a><span data-ttu-id="7f151-139">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="7f151-139">Relationships</span></span>
<span data-ttu-id="7f151-140">なし</span><span class="sxs-lookup"><span data-stu-id="7f151-140">None</span></span>


## <a name="json-representation"></a><span data-ttu-id="7f151-141">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="7f151-141">JSON representation</span></span>

<span data-ttu-id="7f151-142">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="7f151-142">Here is a JSON representation of the resource.</span></span>

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
  "suppressions": [
    "Error: /api-reference/beta/resources/privilegedrolesummary.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
