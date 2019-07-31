---
title: スケジュールリソースの種類
description: チーム内の schedulingGroups、シフト、timeOffReasons 各理由と timesOff のコレクション。
author: nkramer
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: resourcePageType_
ms.openlocfilehash: a404c620b20cfcb69076ecc3bac25f907a12216c
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "35965328"
---
# <a name="schedule-resource-type"></a><span data-ttu-id="ceead-103">スケジュールリソースの種類</span><span class="sxs-lookup"><span data-stu-id="ceead-103">schedule resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="ceead-104">[チーム](../resources/team.md)内の[schedulingGroup](schedulinggroup.md)オブジェクト、 [Shift](shift.md)オブジェクト、 [Timeoffreason](timeoffreason.md)オブジェクト、および[timeoff](timeoff.md)オブジェクトのコレクションです。</span><span class="sxs-lookup"><span data-stu-id="ceead-104">A collection of [schedulingGroup](schedulinggroup.md) objects, [shift](shift.md) objects, [timeOffReason](timeoffreason.md) objects, and [timeOff](timeoff.md) objects within a [team](../resources/team.md).</span></span> 

## <a name="methods"></a><span data-ttu-id="ceead-105">メソッド</span><span class="sxs-lookup"><span data-stu-id="ceead-105">Methods</span></span>

| <span data-ttu-id="ceead-106">メソッド</span><span class="sxs-lookup"><span data-stu-id="ceead-106">Method</span></span>       | <span data-ttu-id="ceead-107">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="ceead-107">Return Type</span></span>  |<span data-ttu-id="ceead-108">説明</span><span class="sxs-lookup"><span data-stu-id="ceead-108">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="ceead-109">スケジュールを作成または置換する</span><span class="sxs-lookup"><span data-stu-id="ceead-109">Create or replace schedule</span></span>](../api/team-put-schedule.md) | [<span data-ttu-id="ceead-110">schedule</span><span class="sxs-lookup"><span data-stu-id="ceead-110">schedule</span></span>](schedule.md) | <span data-ttu-id="ceead-111">を`schedule`作成または置換します。</span><span class="sxs-lookup"><span data-stu-id="ceead-111">Create or replace a `schedule`.</span></span>|
|[<span data-ttu-id="ceead-112">スケジュールを取得する</span><span class="sxs-lookup"><span data-stu-id="ceead-112">Get schedule</span></span>](../api/schedule-get.md) | [<span data-ttu-id="ceead-113">schedule</span><span class="sxs-lookup"><span data-stu-id="ceead-113">schedule</span></span>](schedule.md) | <span data-ttu-id="ceead-114">を`schedule`取得します。</span><span class="sxs-lookup"><span data-stu-id="ceead-114">Get a `schedule`.</span></span>|
|[<span data-ttu-id="ceead-115">share</span><span class="sxs-lookup"><span data-stu-id="ceead-115">share</span></span>](../api/schedule-share.md) | <span data-ttu-id="ceead-116">None</span><span class="sxs-lookup"><span data-stu-id="ceead-116">None</span></span> | <span data-ttu-id="ceead-117">スケジュールメンバー `schedule`で時間範囲を共有します。</span><span class="sxs-lookup"><span data-stu-id="ceead-117">Share a `schedule` time range with schedule members.</span></span>|

## <a name="properties"></a><span data-ttu-id="ceead-118">プロパティ</span><span class="sxs-lookup"><span data-stu-id="ceead-118">Properties</span></span>
|<span data-ttu-id="ceead-119">名前</span><span class="sxs-lookup"><span data-stu-id="ceead-119">Name</span></span>                   |<span data-ttu-id="ceead-120">型</span><span class="sxs-lookup"><span data-stu-id="ceead-120">Type</span></span>           |<span data-ttu-id="ceead-121">説明</span><span class="sxs-lookup"><span data-stu-id="ceead-121">Description</span></span>                                                                                                                                      |
|-----------------------|---------------|-------------------------------------------------------------------------------------------------------------------------------------------------|
| <span data-ttu-id="ceead-122">id</span><span class="sxs-lookup"><span data-stu-id="ceead-122">id</span></span>                    |`string`  |<span data-ttu-id="ceead-123">`schedule` の ID。</span><span class="sxs-lookup"><span data-stu-id="ceead-123">ID of the `schedule`.</span></span>|
| <span data-ttu-id="ceead-124">enabled</span><span class="sxs-lookup"><span data-stu-id="ceead-124">enabled</span></span>               |`bool`    | <span data-ttu-id="ceead-125">スケジュールがチームに対して有効になっているかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="ceead-125">Indicates whether the schedule is enabled for the team.</span></span> <span data-ttu-id="ceead-126">必須です。</span><span class="sxs-lookup"><span data-stu-id="ceead-126">Required.</span></span>|
| <span data-ttu-id="ceead-127">timeZone</span><span class="sxs-lookup"><span data-stu-id="ceead-127">timeZone</span></span>              |`string`  | <span data-ttu-id="ceead-128">Tz データベース形式を使用して、スケジュールチームのタイムゾーンを示します。</span><span class="sxs-lookup"><span data-stu-id="ceead-128">Indicates the time zone of the schedule team using tz database format.</span></span> <span data-ttu-id="ceead-129">必須です。</span><span class="sxs-lookup"><span data-stu-id="ceead-129">Required.</span></span>|
| <span data-ttu-id="ceead-130">provisionStatus</span><span class="sxs-lookup"><span data-stu-id="ceead-130">provisionStatus</span></span>       |`operationStatus`    | <span data-ttu-id="ceead-131">スケジュールの準備の状態。</span><span class="sxs-lookup"><span data-stu-id="ceead-131">The status of the schedule provisioning.</span></span> <span data-ttu-id="ceead-132">使用可能な値`notStarted`は`running` `completed`、、 `failed`、です。</span><span class="sxs-lookup"><span data-stu-id="ceead-132">The possible values are `notStarted`, `running`, `completed`, `failed`.</span></span> |
| <span data-ttu-id="ceead-133">provisionStatusCode</span><span class="sxs-lookup"><span data-stu-id="ceead-133">provisionStatusCode</span></span>   |`string`  | <span data-ttu-id="ceead-134">スケジュールプロビジョニングが失敗した理由に関する追加情報。</span><span class="sxs-lookup"><span data-stu-id="ceead-134">Additional information about why schedule provisioning failed.</span></span> |


## <a name="relationships"></a><span data-ttu-id="ceead-135">関係</span><span class="sxs-lookup"><span data-stu-id="ceead-135">Relationships</span></span>
|<span data-ttu-id="ceead-136">名前</span><span class="sxs-lookup"><span data-stu-id="ceead-136">Name</span></span>                   |<span data-ttu-id="ceead-137">型</span><span class="sxs-lookup"><span data-stu-id="ceead-137">Type</span></span>           |<span data-ttu-id="ceead-138">説明</span><span class="sxs-lookup"><span data-stu-id="ceead-138">Description</span></span>                                                                                                                                      |
|-----------------------|---------------|-------------------------------------------------------------------------------------------------------------------------------------------------|
| <span data-ttu-id="ceead-139">移す</span><span class="sxs-lookup"><span data-stu-id="ceead-139">shifts</span></span>   |`collection(shift)`  | <span data-ttu-id="ceead-140">スケジュールのシフト。</span><span class="sxs-lookup"><span data-stu-id="ceead-140">The shifts in the schedule.</span></span> |
| <span data-ttu-id="ceead-141">timesOff</span><span class="sxs-lookup"><span data-stu-id="ceead-141">timesOff</span></span>   |`collection(timeOff)`  | <span data-ttu-id="ceead-142">スケジュールでオフにされた回数のインスタンス。</span><span class="sxs-lookup"><span data-stu-id="ceead-142">The instances of times off in the schedule.</span></span> |
| <span data-ttu-id="ceead-143">timeOffReasons</span><span class="sxs-lookup"><span data-stu-id="ceead-143">timeOffReasons</span></span>   |`collection(timeOffReason)`  | <span data-ttu-id="ceead-144">スケジュールで時間切れがある理由のセット。</span><span class="sxs-lookup"><span data-stu-id="ceead-144">The set of reasons for a time off in the schedule.</span></span> |
| <span data-ttu-id="ceead-145">schedulingGroups</span><span class="sxs-lookup"><span data-stu-id="ceead-145">schedulingGroups</span></span>   |`collection(schedulingGroup)`  | <span data-ttu-id="ceead-146">スケジュールに含まれるユーザーの論理グループ (通常は、役割別)。</span><span class="sxs-lookup"><span data-stu-id="ceead-146">The logical grouping of users in the schedule (usually by role).</span></span> |


## <a name="json-representation"></a><span data-ttu-id="ceead-147">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="ceead-147">JSON representation</span></span>

<span data-ttu-id="ceead-148">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="ceead-148">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.schedule"
}-->

```json
{
  "id": "833fc4df-c88b-4398-992f-d8afcfe41df2",
  "enabled": true,
  "timeZone": "America/Chicago",
  "provisionStatus": "Completed",
  "provisionStatusCode": null
}
```


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "schedule resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
