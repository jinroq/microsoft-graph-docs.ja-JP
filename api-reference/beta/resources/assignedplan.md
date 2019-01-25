---
title: assignedPlan リソースの種類
description: '**ユーザー** エンティティと組織エンティティの両方の assignedPlans プロパティは、assignedPlan のコレクションです。'
localization_priority: Normal
ms.openlocfilehash: 3e06894fa71f81993b94d174d6cde8a54126fd62
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/24/2019
ms.locfileid: "29525137"
---
# <a name="assignedplan-resource-type"></a><span data-ttu-id="c39bb-103">assignedPlan リソースの種類</span><span class="sxs-lookup"><span data-stu-id="c39bb-103">assignedPlan resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="c39bb-104">[ユーザー](user.md) エンティティと[組織](organization.md)エンティティの両方の **assignedPlans** プロパティは、**assignedPlan** のコレクションです。</span><span class="sxs-lookup"><span data-stu-id="c39bb-104">The **assignedPlans** property of both the [user](user.md) entity and the [organization](organization.md) entity is a collection of **assignedPlan**.</span></span>


## <a name="properties"></a><span data-ttu-id="c39bb-105">プロパティ</span><span class="sxs-lookup"><span data-stu-id="c39bb-105">Properties</span></span>
| <span data-ttu-id="c39bb-106">プロパティ</span><span class="sxs-lookup"><span data-stu-id="c39bb-106">Property</span></span>     | <span data-ttu-id="c39bb-107">型</span><span class="sxs-lookup"><span data-stu-id="c39bb-107">Type</span></span>   |<span data-ttu-id="c39bb-108">説明</span><span class="sxs-lookup"><span data-stu-id="c39bb-108">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="c39bb-109">assignedDateTime</span><span class="sxs-lookup"><span data-stu-id="c39bb-109">assignedDateTime</span></span>|<span data-ttu-id="c39bb-110">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="c39bb-110">DateTimeOffset</span></span>|<span data-ttu-id="c39bb-p101">プランが割り当てられた日時です。例:2013-01-02T19:32:30Z。Timestamp 型は、ISO 8601 形式を使用して日付と時刻の情報を表し、必ず UTC 時間です。たとえば、2014 年 1 月 1 日午前 0 時 (UTC) は、次のようになります。`'2014-01-01T00:00:00Z'`</span><span class="sxs-lookup"><span data-stu-id="c39bb-p101">The date and time at which the plan was assigned; for example: 2013-01-02T19:32:30Z. The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time. For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|
|<span data-ttu-id="c39bb-114">capabilityStatus</span><span class="sxs-lookup"><span data-stu-id="c39bb-114">capabilityStatus</span></span>|<span data-ttu-id="c39bb-115">String</span><span class="sxs-lookup"><span data-stu-id="c39bb-115">String</span></span>|<span data-ttu-id="c39bb-116">「有効」など。</span><span class="sxs-lookup"><span data-stu-id="c39bb-116">For example, “Enabled”.</span></span>|
|<span data-ttu-id="c39bb-117">service</span><span class="sxs-lookup"><span data-stu-id="c39bb-117">service</span></span>|<span data-ttu-id="c39bb-118">String</span><span class="sxs-lookup"><span data-stu-id="c39bb-118">String</span></span>|<span data-ttu-id="c39bb-119">サービスの名前。「Exchange」など。</span><span class="sxs-lookup"><span data-stu-id="c39bb-119">The name of the service; for example, “Exchange”.</span></span>|
|<span data-ttu-id="c39bb-120">servicePlanId</span><span class="sxs-lookup"><span data-stu-id="c39bb-120">servicePlanId</span></span>|<span data-ttu-id="c39bb-121">Guid</span><span class="sxs-lookup"><span data-stu-id="c39bb-121">Guid</span></span>|<span data-ttu-id="c39bb-122">サービス プランを識別する GUID。</span><span class="sxs-lookup"><span data-stu-id="c39bb-122">A GUID that identifies the service plan.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="c39bb-123">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="c39bb-123">JSON representation</span></span>

<span data-ttu-id="c39bb-124">以下は、リソースの JSON 表記です</span><span class="sxs-lookup"><span data-stu-id="c39bb-124">Here is a JSON representation of the resource</span></span>

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
  "suppressions": [
    "Error: /api-reference/beta/resources/assignedplan.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
