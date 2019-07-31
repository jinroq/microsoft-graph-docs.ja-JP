---
title: governanceSchedule リソースの種類
description: 'GovernanceRoleAssignmentRequest のスケジュールを表します。 役割の割り当て要求の場合、スケジュールは、役割の割り当て操作を実行するタイミング、役割の割り当てを停止するタイミング、および役割の割り当て操作を実行する頻度を制御します。 '
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
author: ''
ms.openlocfilehash: 36a2b4c73f5f85439a34a42ea2aa23cfe861c4ab
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "36006375"
---
# <a name="governanceschedule-resource-type"></a><span data-ttu-id="14d94-104">governanceSchedule リソースの種類</span><span class="sxs-lookup"><span data-stu-id="14d94-104">governanceSchedule resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="14d94-105">[GovernanceRoleAssignmentRequest](../resources/governanceroleassignmentrequest.md)のスケジュールを表します。</span><span class="sxs-lookup"><span data-stu-id="14d94-105">Represents the schedule for a [governanceRoleAssignmentRequest](../resources/governanceroleassignmentrequest.md).</span></span> <span data-ttu-id="14d94-106">役割の割り当て要求の場合、スケジュールは、役割の割り当て操作を実行するタイミング、役割の割り当てを停止するタイミング、および役割の割り当て操作を実行する頻度を制御します。</span><span class="sxs-lookup"><span data-stu-id="14d94-106">For a role assignment request, the schedule controls when to perform the role assignment operation, when to stop the role assignment, and how frequently to do the role assignment operation.</span></span> 



## <a name="properties"></a><span data-ttu-id="14d94-107">プロパティ</span><span class="sxs-lookup"><span data-stu-id="14d94-107">Properties</span></span>
| <span data-ttu-id="14d94-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="14d94-108">Property</span></span>     | <span data-ttu-id="14d94-109">型</span><span class="sxs-lookup"><span data-stu-id="14d94-109">Type</span></span>   |<span data-ttu-id="14d94-110">説明</span><span class="sxs-lookup"><span data-stu-id="14d94-110">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="14d94-111">startDateTime</span><span class="sxs-lookup"><span data-stu-id="14d94-111">startDateTime</span></span>|<span data-ttu-id="14d94-112">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="14d94-112">DateTimeOffset</span></span>|<span data-ttu-id="14d94-113">役割の割り当ての開始時刻。</span><span class="sxs-lookup"><span data-stu-id="14d94-113">The start time of the role assignment.</span></span> <span data-ttu-id="14d94-114">Timestamp 型は、ISO 8601 形式を使用して日付と時刻の情報を表し、必ず UTC 時間です。</span><span class="sxs-lookup"><span data-stu-id="14d94-114">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="14d94-115">たとえば、2014 年 1 月 1 日午前 0 時 (UTC) は、次のようになります。`'2014-01-01T00:00:00Z'`</span><span class="sxs-lookup"><span data-stu-id="14d94-115">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|
|<span data-ttu-id="14d94-116">endDateTime</span><span class="sxs-lookup"><span data-stu-id="14d94-116">endDateTime</span></span>|<span data-ttu-id="14d94-117">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="14d94-117">DateTimeOffset</span></span>|<span data-ttu-id="14d94-118">役割の割り当ての終了時刻。</span><span class="sxs-lookup"><span data-stu-id="14d94-118">The end time of the role assignment.</span></span> <span data-ttu-id="14d94-119">Timestamp 型は、ISO 8601 形式を使用して日付と時刻の情報を表します。これは常に UTC 時間です。</span><span class="sxs-lookup"><span data-stu-id="14d94-119">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="14d94-120">たとえば、2014 年 1 月 1 日午前 0 時 (UTC) は、次のようになります。`'2014-01-01T00:00:00Z'`</span><span class="sxs-lookup"><span data-stu-id="14d94-120">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`.</span></span> <span data-ttu-id="14d94-121">*注: 値がの場合`null`は、永続的な割り当てを示します。*</span><span class="sxs-lookup"><span data-stu-id="14d94-121">*Note: if the value is `null`, it indicates a permanent assignment.*</span></span>|
|<span data-ttu-id="14d94-122">type</span><span class="sxs-lookup"><span data-stu-id="14d94-122">type</span></span>|<span data-ttu-id="14d94-123">String</span><span class="sxs-lookup"><span data-stu-id="14d94-123">String</span></span>|<span data-ttu-id="14d94-124">役割の割り当てスケジュールの種類。</span><span class="sxs-lookup"><span data-stu-id="14d94-124">The role assignment schedule type.</span></span> <span data-ttu-id="14d94-125">現時点`Once`でのみサポートされています。</span><span class="sxs-lookup"><span data-stu-id="14d94-125">Only `Once` is supported for now.</span></span>
|<span data-ttu-id="14d94-126">duration</span><span class="sxs-lookup"><span data-stu-id="14d94-126">duration</span></span>|<span data-ttu-id="14d94-127">期間</span><span class="sxs-lookup"><span data-stu-id="14d94-127">Duration</span></span>|<span data-ttu-id="14d94-128">役割の割り当ての期間。</span><span class="sxs-lookup"><span data-stu-id="14d94-128">The duration of a role assignment.</span></span> <span data-ttu-id="14d94-129">これは、TimeSpan の形式です。</span><span class="sxs-lookup"><span data-stu-id="14d94-129">It is in format of a TimeSpan.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="14d94-130">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="14d94-130">JSON representation</span></span>

<span data-ttu-id="14d94-131">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="14d94-131">Here is a JSON representation of the resource.</span></span>

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
  "suppressions": []
}
-->
