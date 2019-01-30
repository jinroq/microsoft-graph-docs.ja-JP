---
title: governanceSchedule リソースの種類
description: 'GovernanceRoleAssignmentRequest のスケジュールを表します。 役割の割り当て要求のスケジュールを制御、ロールの割り当て操作を実行する場合、役割の割り当てを停止するタイミングと役割の割り当て操作を実行する頻度です。 '
localization_priority: Normal
ms.openlocfilehash: d7ccfe74804166ad2204ea02c072d79341cf75e7
ms.sourcegitcommit: d95f6d39a0479da6e531f3734c4029dc596b9a3f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/30/2019
ms.locfileid: "29643413"
---
# <a name="governanceschedule-resource-type"></a><span data-ttu-id="c0863-104">governanceSchedule リソースの種類</span><span class="sxs-lookup"><span data-stu-id="c0863-104">governanceSchedule resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="c0863-105">の[governanceRoleAssignmentRequest](../resources/governanceroleassignmentrequest.md)のスケジュールを表します。</span><span class="sxs-lookup"><span data-stu-id="c0863-105">Represents the schedule for a [governanceRoleAssignmentRequest](../resources/governanceroleassignmentrequest.md).</span></span> <span data-ttu-id="c0863-106">役割の割り当て要求のスケジュールを制御、ロールの割り当て操作を実行する場合、役割の割り当てを停止するタイミングと役割の割り当て操作を実行する頻度です。</span><span class="sxs-lookup"><span data-stu-id="c0863-106">For a role assignment request, the schedule controls when to perform the role assignment operation, when to stop the role assignment, and how frequently to do the role assignment operation.</span></span> 



## <a name="properties"></a><span data-ttu-id="c0863-107">プロパティ</span><span class="sxs-lookup"><span data-stu-id="c0863-107">Properties</span></span>
| <span data-ttu-id="c0863-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="c0863-108">Property</span></span>     | <span data-ttu-id="c0863-109">型</span><span class="sxs-lookup"><span data-stu-id="c0863-109">Type</span></span>   |<span data-ttu-id="c0863-110">説明</span><span class="sxs-lookup"><span data-stu-id="c0863-110">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="c0863-111">startDateTime</span><span class="sxs-lookup"><span data-stu-id="c0863-111">startDateTime</span></span>|<span data-ttu-id="c0863-112">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="c0863-112">DateTimeOffset</span></span>|<span data-ttu-id="c0863-113">役割の割り当ての開始時刻。</span><span class="sxs-lookup"><span data-stu-id="c0863-113">The start time of the role assignment.</span></span> <span data-ttu-id="c0863-114">Timestamp 型は、ISO 8601 形式を使用して日付と時刻の情報を表し、常に UTC 時間です。</span><span class="sxs-lookup"><span data-stu-id="c0863-114">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="c0863-115">たとえば、2014 年 1 月 1 日午前 0 時 (UTC) は、次のようになります。`'2014-01-01T00:00:00Z'`</span><span class="sxs-lookup"><span data-stu-id="c0863-115">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|
|<span data-ttu-id="c0863-116">endDateTime</span><span class="sxs-lookup"><span data-stu-id="c0863-116">endDateTime</span></span>|<span data-ttu-id="c0863-117">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="c0863-117">DateTimeOffset</span></span>|<span data-ttu-id="c0863-118">役割の割り当ての終了時間です。</span><span class="sxs-lookup"><span data-stu-id="c0863-118">The end time of the role assignment.</span></span> <span data-ttu-id="c0863-119">Timestamp 型は、ISO 8601 形式を使用して日付と時刻の情報を表し、常に UTC 時間です。</span><span class="sxs-lookup"><span data-stu-id="c0863-119">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="c0863-120">たとえば、2014 年 1 月 1 日午前 0 時 (UTC) は、`'2014-01-01T00:00:00Z'` のようになります。</span><span class="sxs-lookup"><span data-stu-id="c0863-120">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`.</span></span> <span data-ttu-id="c0863-121">*注: 場合は、値は、 `null`、永続的な割り当てを示します。*</span><span class="sxs-lookup"><span data-stu-id="c0863-121">*Note: if the value is `null`, it indicates a permanent assignment.*</span></span>|
|<span data-ttu-id="c0863-122">type</span><span class="sxs-lookup"><span data-stu-id="c0863-122">type</span></span>|<span data-ttu-id="c0863-123">String</span><span class="sxs-lookup"><span data-stu-id="c0863-123">String</span></span>|<span data-ttu-id="c0863-124">ロールの割り当てスケジュールの種類です。</span><span class="sxs-lookup"><span data-stu-id="c0863-124">The role assignment schedule type.</span></span> <span data-ttu-id="c0863-125">のみ`Once`ここではサポートされています。</span><span class="sxs-lookup"><span data-stu-id="c0863-125">Only `Once` is supported for now.</span></span>
|<span data-ttu-id="c0863-126">duration</span><span class="sxs-lookup"><span data-stu-id="c0863-126">duration</span></span>|<span data-ttu-id="c0863-127">Duration</span><span class="sxs-lookup"><span data-stu-id="c0863-127">Duration</span></span>|<span data-ttu-id="c0863-128">役割の割り当ての期間です。</span><span class="sxs-lookup"><span data-stu-id="c0863-128">The duration of a role assignment.</span></span> <span data-ttu-id="c0863-129">TimeSpan の形式であります。</span><span class="sxs-lookup"><span data-stu-id="c0863-129">It is in format of a TimeSpan.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="c0863-130">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="c0863-130">JSON representation</span></span>

<span data-ttu-id="c0863-131">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="c0863-131">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.governanceSchedule"
}-->

```json
{
  "duration": "String (timespan)",
  "startDateTime": "String (timestamp)",
  "endDateTime": "String (timestamp)",
  "type": "String"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "governanceSchedule",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/governanceschedule.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
