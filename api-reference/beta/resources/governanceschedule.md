---
title: governanceSchedule リソースの種類
description: 'GovernanceRoleAssignmentRequest のスケジュールを表します。 役割の割り当て要求のスケジュールを制御、ロールの割り当て操作を実行する場合、役割の割り当てを停止するタイミングと役割の割り当て操作を実行する頻度です。 '
localization_priority: Normal
ms.openlocfilehash: 8bf36b786adbd8064ee0c00c0ce293408c6e2b7f
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/11/2019
ms.locfileid: "27882314"
---
# <a name="governanceschedule-resource-type"></a><span data-ttu-id="61c03-104">governanceSchedule リソースの種類</span><span class="sxs-lookup"><span data-stu-id="61c03-104">governanceSchedule resource type</span></span>

> <span data-ttu-id="61c03-105">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="61c03-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="61c03-106">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="61c03-106">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="61c03-107">の[governanceRoleAssignmentRequest](../resources/governanceroleassignmentrequest.md)のスケジュールを表します。</span><span class="sxs-lookup"><span data-stu-id="61c03-107">Represents the schedule for a [governanceRoleAssignmentRequest](../resources/governanceroleassignmentrequest.md).</span></span> <span data-ttu-id="61c03-108">役割の割り当て要求のスケジュールを制御、ロールの割り当て操作を実行する場合、役割の割り当てを停止するタイミングと役割の割り当て操作を実行する頻度です。</span><span class="sxs-lookup"><span data-stu-id="61c03-108">For a role assignment request, the schedule controls when to perform the role assignment operation, when to stop the role assignment, and how frequently to do the role assignment operation.</span></span> 



## <a name="properties"></a><span data-ttu-id="61c03-109">プロパティ</span><span class="sxs-lookup"><span data-stu-id="61c03-109">Properties</span></span>
| <span data-ttu-id="61c03-110">プロパティ</span><span class="sxs-lookup"><span data-stu-id="61c03-110">Property</span></span>     | <span data-ttu-id="61c03-111">種類</span><span class="sxs-lookup"><span data-stu-id="61c03-111">Type</span></span>   |<span data-ttu-id="61c03-112">説明</span><span class="sxs-lookup"><span data-stu-id="61c03-112">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="61c03-113">startDateTime</span><span class="sxs-lookup"><span data-stu-id="61c03-113">startDateTime</span></span>|<span data-ttu-id="61c03-114">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="61c03-114">DateTimeOffset</span></span>|<span data-ttu-id="61c03-115">役割の割り当ての開始時刻。</span><span class="sxs-lookup"><span data-stu-id="61c03-115">The start time of the role assignment.</span></span> <span data-ttu-id="61c03-116">Timestamp 型は、ISO 8601 形式を使用して日付と時刻の情報を表し、常に UTC 時間です。</span><span class="sxs-lookup"><span data-stu-id="61c03-116">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="61c03-117">たとえば、2014 年 1 月 1 日午前 0 時 (UTC) は、次のようになります。`'2014-01-01T00:00:00Z'`</span><span class="sxs-lookup"><span data-stu-id="61c03-117">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|
|<span data-ttu-id="61c03-118">endDateTime</span><span class="sxs-lookup"><span data-stu-id="61c03-118">endDateTime</span></span>|<span data-ttu-id="61c03-119">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="61c03-119">DateTimeOffset</span></span>|<span data-ttu-id="61c03-120">役割の割り当ての終了時間です。</span><span class="sxs-lookup"><span data-stu-id="61c03-120">The end time of the role assignment.</span></span> <span data-ttu-id="61c03-121">Timestamp 型は、ISO 8601 形式を使用して日付と時刻の情報を表し、常に UTC 時間です。</span><span class="sxs-lookup"><span data-stu-id="61c03-121">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="61c03-122">たとえば、2014 年 1 月 1 日午前 0 時 (UTC) は、次のようになります。`'2014-01-01T00:00:00Z'`</span><span class="sxs-lookup"><span data-stu-id="61c03-122">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`.</span></span> <span data-ttu-id="61c03-123">*注: 場合は、値は、 `null`、永続的な割り当てを示します。*</span><span class="sxs-lookup"><span data-stu-id="61c03-123">*Note: if the value is `null`, it indicates a permanent assignment.*</span></span>|
|<span data-ttu-id="61c03-124">type</span><span class="sxs-lookup"><span data-stu-id="61c03-124">type</span></span>|<span data-ttu-id="61c03-125">String</span><span class="sxs-lookup"><span data-stu-id="61c03-125">String</span></span>|<span data-ttu-id="61c03-126">ロールの割り当てスケジュールの種類です。</span><span class="sxs-lookup"><span data-stu-id="61c03-126">The role assignment schedule type.</span></span> <span data-ttu-id="61c03-127">のみ`Once`ここではサポートされています。</span><span class="sxs-lookup"><span data-stu-id="61c03-127">Only `Once` is supported for now.</span></span>
|<span data-ttu-id="61c03-128">duration</span><span class="sxs-lookup"><span data-stu-id="61c03-128">duration</span></span>|<span data-ttu-id="61c03-129">Duration</span><span class="sxs-lookup"><span data-stu-id="61c03-129">Duration</span></span>|<span data-ttu-id="61c03-130">役割の割り当ての期間です。</span><span class="sxs-lookup"><span data-stu-id="61c03-130">The duration of a role assignment.</span></span> <span data-ttu-id="61c03-131">TimeSpan の形式であります。</span><span class="sxs-lookup"><span data-stu-id="61c03-131">It is in format of a TimeSpan.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="61c03-132">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="61c03-132">JSON representation</span></span>

<span data-ttu-id="61c03-133">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="61c03-133">Here is a JSON representation of the resource.</span></span>

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
<!-- {
  "type": "#page.annotation",
  "description": "governanceSchedule",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
