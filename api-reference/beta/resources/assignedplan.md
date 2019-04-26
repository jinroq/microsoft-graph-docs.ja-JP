---
title: assignedPlan リソースの種類
description: '**ユーザー** エンティティと組織エンティティの両方の assignedPlans プロパティは、**assignedPlan** のコレクションです。'
localization_priority: Normal
ms.openlocfilehash: 0f44e96e5591d46d6a22b0cdd951b4dfb1e05e75
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/26/2019
ms.locfileid: "33339090"
---
# <a name="assignedplan-resource-type"></a><span data-ttu-id="91db4-103">assignedPlan リソースの種類</span><span class="sxs-lookup"><span data-stu-id="91db4-103">assignedPlan resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="91db4-104">**ユーザー** エンティティと[組織](user.md)エンティティの両方の [assignedPlans](organization.md) プロパティは、**assignedPlan** のコレクションです。</span><span class="sxs-lookup"><span data-stu-id="91db4-104">The **assignedPlans** property of both the [user](user.md) entity and the [organization](organization.md) entity is a collection of **assignedPlan**.</span></span>


## <a name="properties"></a><span data-ttu-id="91db4-105">プロパティ</span><span class="sxs-lookup"><span data-stu-id="91db4-105">Properties</span></span>
| <span data-ttu-id="91db4-106">プロパティ</span><span class="sxs-lookup"><span data-stu-id="91db4-106">Property</span></span>     | <span data-ttu-id="91db4-107">型</span><span class="sxs-lookup"><span data-stu-id="91db4-107">Type</span></span>   |<span data-ttu-id="91db4-108">説明</span><span class="sxs-lookup"><span data-stu-id="91db4-108">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="91db4-109">assignedDateTime</span><span class="sxs-lookup"><span data-stu-id="91db4-109">assignedDateTime</span></span>|<span data-ttu-id="91db4-110">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="91db4-110">DateTimeOffset</span></span>|<span data-ttu-id="91db4-p101">プランが割り当てられた日時です。例:2013-01-02T19:32:30Z。Timestamp 型は、ISO 8601 形式を使用して日付と時刻の情報を表し、必ず UTC 時間です。たとえば、2014 年 1 月 1 日午前 0 時 (UTC) は、次のようになります。`'2014-01-01T00:00:00Z'`</span><span class="sxs-lookup"><span data-stu-id="91db4-p101">The date and time at which the plan was assigned; for example: 2013-01-02T19:32:30Z. The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time. For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|
|<span data-ttu-id="91db4-114">capabilityStatus</span><span class="sxs-lookup"><span data-stu-id="91db4-114">capabilityStatus</span></span>|<span data-ttu-id="91db4-115">String</span><span class="sxs-lookup"><span data-stu-id="91db4-115">String</span></span>|<span data-ttu-id="91db4-116">「有効」など。</span><span class="sxs-lookup"><span data-stu-id="91db4-116">For example, “Enabled”.</span></span>|
|<span data-ttu-id="91db4-117">service</span><span class="sxs-lookup"><span data-stu-id="91db4-117">service</span></span>|<span data-ttu-id="91db4-118">String</span><span class="sxs-lookup"><span data-stu-id="91db4-118">String</span></span>|<span data-ttu-id="91db4-119">サービスの名前。「Exchange」など。</span><span class="sxs-lookup"><span data-stu-id="91db4-119">The name of the service; for example, “Exchange”.</span></span>|
|<span data-ttu-id="91db4-120">servicePlanId</span><span class="sxs-lookup"><span data-stu-id="91db4-120">servicePlanId</span></span>|<span data-ttu-id="91db4-121">Guid</span><span class="sxs-lookup"><span data-stu-id="91db4-121">Guid</span></span>|<span data-ttu-id="91db4-122">サービス プランを識別する GUID。</span><span class="sxs-lookup"><span data-stu-id="91db4-122">A GUID that identifies the service plan.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="91db4-123">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="91db4-123">JSON representation</span></span>

<span data-ttu-id="91db4-124">以下は、リソースの JSON 表記です</span><span class="sxs-lookup"><span data-stu-id="91db4-124">Here is a JSON representation of the resource</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.assignedPlan"
}-->

```json
{
  "assignedDateTime": "String (timestamp)",
  "capabilityStatus": "string",
  "service": "string",
  "servicePlanId": "guid"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "assignedPlan resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
