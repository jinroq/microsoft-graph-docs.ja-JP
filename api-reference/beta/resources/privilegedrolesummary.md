---
title: privilegedRoleSummary リソースの種類
description: 特定の役割の統計の概要。
localization_priority: Normal
ms.openlocfilehash: 2ed34f556f52c41729bfa108fbb6eb0c608f6b67
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32563435"
---
# <a name="privilegedrolesummary-resource-type"></a><span data-ttu-id="d70ae-103">privilegedRoleSummary リソースの種類</span><span class="sxs-lookup"><span data-stu-id="d70ae-103">privilegedRoleSummary resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="d70ae-104">特定の役割の統計の概要。</span><span class="sxs-lookup"><span data-stu-id="d70ae-104">The statistics summary for a particular role.</span></span>


## <a name="methods"></a><span data-ttu-id="d70ae-105">メソッド</span><span class="sxs-lookup"><span data-stu-id="d70ae-105">Methods</span></span>

| <span data-ttu-id="d70ae-106">メソッド</span><span class="sxs-lookup"><span data-stu-id="d70ae-106">Method</span></span>           | <span data-ttu-id="d70ae-107">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="d70ae-107">Return Type</span></span>    |<span data-ttu-id="d70ae-108">説明</span><span class="sxs-lookup"><span data-stu-id="d70ae-108">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="d70ae-109">privilegedRoleSummary を取得する</span><span class="sxs-lookup"><span data-stu-id="d70ae-109">Get privilegedRoleSummary</span></span>](../api/privilegedrolesummary-get.md) | [<span data-ttu-id="d70ae-110">privilegedRoleSummary</span><span class="sxs-lookup"><span data-stu-id="d70ae-110">privilegedRoleSummary</span></span>](privilegedrolesummary.md) |<span data-ttu-id="d70ae-111">privilegedRoleSummary オブジェクトのプロパティとリレーションシップを読み取ります。</span><span class="sxs-lookup"><span data-stu-id="d70ae-111">Read properties and relationships of privilegedRoleSummary object.</span></span>|

## <a name="properties"></a><span data-ttu-id="d70ae-112">プロパティ</span><span class="sxs-lookup"><span data-stu-id="d70ae-112">Properties</span></span>
| <span data-ttu-id="d70ae-113">プロパティ</span><span class="sxs-lookup"><span data-stu-id="d70ae-113">Property</span></span>     | <span data-ttu-id="d70ae-114">型</span><span class="sxs-lookup"><span data-stu-id="d70ae-114">Type</span></span>   |<span data-ttu-id="d70ae-115">説明</span><span class="sxs-lookup"><span data-stu-id="d70ae-115">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="d70ae-116">elevatedCount</span><span class="sxs-lookup"><span data-stu-id="d70ae-116">elevatedCount</span></span>|<span data-ttu-id="d70ae-117">int32</span><span class="sxs-lookup"><span data-stu-id="d70ae-117">int32</span></span>|<span data-ttu-id="d70ae-118">役割が割り当てられていて、役割がアクティブ化されているユーザーの数。</span><span class="sxs-lookup"><span data-stu-id="d70ae-118">The number of users that have the role assigned and the role is activated.</span></span>|
|<span data-ttu-id="d70ae-119">id</span><span class="sxs-lookup"><span data-stu-id="d70ae-119">id</span></span>|<span data-ttu-id="d70ae-120">string</span><span class="sxs-lookup"><span data-stu-id="d70ae-120">string</span></span>| <span data-ttu-id="d70ae-121">ロールの一意識別子。</span><span class="sxs-lookup"><span data-stu-id="d70ae-121">The unique identifier for the role.</span></span> <span data-ttu-id="d70ae-122">読み取り専用。</span><span class="sxs-lookup"><span data-stu-id="d70ae-122">Read-only.</span></span>|
|<span data-ttu-id="d70ae-123">managedcount</span><span class="sxs-lookup"><span data-stu-id="d70ae-123">managedCount</span></span>|<span data-ttu-id="d70ae-124">int32</span><span class="sxs-lookup"><span data-stu-id="d70ae-124">int32</span></span>|<span data-ttu-id="d70ae-125">役割が割り当てられているが、その役割が非アクティブ化されたユーザーの数。</span><span class="sxs-lookup"><span data-stu-id="d70ae-125">The number of users that have the role assigned but the role is deactivated.</span></span>|
|<span data-ttu-id="d70ae-126">mfaenabled</span><span class="sxs-lookup"><span data-stu-id="d70ae-126">mfaEnabled</span></span>|<span data-ttu-id="d70ae-127">ブール値</span><span class="sxs-lookup"><span data-stu-id="d70ae-127">boolean</span></span>|<span data-ttu-id="d70ae-128">役割のライセンス認証が MFA を必要とする場合は**true** 。</span><span class="sxs-lookup"><span data-stu-id="d70ae-128">**true** if the role activation requires MFA.</span></span> <span data-ttu-id="d70ae-129">役割のライセンス認証が MFA を必要としない場合は**false** 。</span><span class="sxs-lookup"><span data-stu-id="d70ae-129">**false** if the role activation doesn't require MFA.</span></span>|
|<span data-ttu-id="d70ae-130">status</span><span class="sxs-lookup"><span data-stu-id="d70ae-130">status</span></span>|<span data-ttu-id="d70ae-131">string</span><span class="sxs-lookup"><span data-stu-id="d70ae-131">string</span></span>| <span data-ttu-id="d70ae-132">可能な値は、`ok`、`bad` です。</span><span class="sxs-lookup"><span data-stu-id="d70ae-132">Possible values are: `ok`, `bad`.</span></span> <span data-ttu-id="d70ae-133">値は、の比率 (managedcount/ユーザーカウント) によって決まります。</span><span class="sxs-lookup"><span data-stu-id="d70ae-133">The value depends on the ratio of (managedCount / usersCount).</span></span> <span data-ttu-id="d70ae-134">比率が定義済みのしきい値よりも小さい`ok`場合は、が返されます。</span><span class="sxs-lookup"><span data-stu-id="d70ae-134">If the ratio is less than a predefined threshold, `ok` is returned.</span></span> <span data-ttu-id="d70ae-135">それ以外`bad`の場合は、が返されます。</span><span class="sxs-lookup"><span data-stu-id="d70ae-135">Otherwise, `bad` is returned.</span></span>|
|<span data-ttu-id="d70ae-136">usersCount</span><span class="sxs-lookup"><span data-stu-id="d70ae-136">usersCount</span></span>|<span data-ttu-id="d70ae-137">int32</span><span class="sxs-lookup"><span data-stu-id="d70ae-137">int32</span></span>|<span data-ttu-id="d70ae-138">役割に割り当てられているユーザーの数。</span><span class="sxs-lookup"><span data-stu-id="d70ae-138">The number of users that are assigned with the role.</span></span>|

## <a name="relationships"></a><span data-ttu-id="d70ae-139">関係</span><span class="sxs-lookup"><span data-stu-id="d70ae-139">Relationships</span></span>
<span data-ttu-id="d70ae-140">なし</span><span class="sxs-lookup"><span data-stu-id="d70ae-140">None</span></span>


## <a name="json-representation"></a><span data-ttu-id="d70ae-141">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="d70ae-141">JSON representation</span></span>

<span data-ttu-id="d70ae-142">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="d70ae-142">Here is a JSON representation of the resource.</span></span>

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
