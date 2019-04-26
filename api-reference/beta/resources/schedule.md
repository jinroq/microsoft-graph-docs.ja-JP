---
title: スケジュールリソースの種類
description: チーム内の schedulingGroups、シフト、timeoffreasons 各理由と timesoff のコレクション。
author: nkramer
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: 48b3b5c118a39442469bc6155068664fcebe0ec2
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/26/2019
ms.locfileid: "33343522"
---
# <a name="schedule-resource-type"></a><span data-ttu-id="d8537-103">スケジュールリソースの種類</span><span class="sxs-lookup"><span data-stu-id="d8537-103">schedule resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="d8537-104">[チーム](../resources/team.md)内の[schedulingGroup](schedulinggroup.md)オブジェクト、 [shift](shift.md)オブジェクト、 [timeoffreason](timeoffreason.md)オブジェクト、および[timeoff](timeoff.md)オブジェクトのコレクションです。</span><span class="sxs-lookup"><span data-stu-id="d8537-104">A collection of [schedulingGroup](schedulinggroup.md) objects, [shift](shift.md) objects, [timeOffReason](timeoffreason.md) objects, and [timeOff](timeoff.md) objects within a [team](../resources/team.md).</span></span> 

## <a name="methods"></a><span data-ttu-id="d8537-105">メソッド</span><span class="sxs-lookup"><span data-stu-id="d8537-105">Methods</span></span>

| <span data-ttu-id="d8537-106">メソッド</span><span class="sxs-lookup"><span data-stu-id="d8537-106">Method</span></span>       | <span data-ttu-id="d8537-107">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="d8537-107">Return Type</span></span>  |<span data-ttu-id="d8537-108">説明</span><span class="sxs-lookup"><span data-stu-id="d8537-108">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="d8537-109">スケジュールを作成または置換する</span><span class="sxs-lookup"><span data-stu-id="d8537-109">Create or replace schedule</span></span>](../api/team-put-schedule.md) | [<span data-ttu-id="d8537-110">スケジューリング</span><span class="sxs-lookup"><span data-stu-id="d8537-110">schedule</span></span>](schedule.md) | <span data-ttu-id="d8537-111">を`schedule`作成または置換します。</span><span class="sxs-lookup"><span data-stu-id="d8537-111">Create or replace a `schedule`.</span></span>|
|[<span data-ttu-id="d8537-112">スケジュールを取得する</span><span class="sxs-lookup"><span data-stu-id="d8537-112">Get schedule</span></span>](../api/schedule-get.md) | [<span data-ttu-id="d8537-113">スケジューリング</span><span class="sxs-lookup"><span data-stu-id="d8537-113">schedule</span></span>](schedule.md) | <span data-ttu-id="d8537-114">を`schedule`取得します。</span><span class="sxs-lookup"><span data-stu-id="d8537-114">Get a `schedule`.</span></span>|
|[<span data-ttu-id="d8537-115">share</span><span class="sxs-lookup"><span data-stu-id="d8537-115">share</span></span>](../api/schedule-share.md) | <span data-ttu-id="d8537-116">なし</span><span class="sxs-lookup"><span data-stu-id="d8537-116">None</span></span> | <span data-ttu-id="d8537-117">スケジュールメンバー `schedule`で時間範囲を共有します。</span><span class="sxs-lookup"><span data-stu-id="d8537-117">Share a `schedule` time range with schedule members.</span></span>|

## <a name="properties"></a><span data-ttu-id="d8537-118">プロパティ</span><span class="sxs-lookup"><span data-stu-id="d8537-118">Properties</span></span>
|<span data-ttu-id="d8537-119">名前</span><span class="sxs-lookup"><span data-stu-id="d8537-119">Name</span></span>                   |<span data-ttu-id="d8537-120">型</span><span class="sxs-lookup"><span data-stu-id="d8537-120">Type</span></span>           |<span data-ttu-id="d8537-121">説明</span><span class="sxs-lookup"><span data-stu-id="d8537-121">Description</span></span>                                                                                                                                      |
|-----------------------|---------------|-------------------------------------------------------------------------------------------------------------------------------------------------|
| <span data-ttu-id="d8537-122">id</span><span class="sxs-lookup"><span data-stu-id="d8537-122">id</span></span>                    |`string`  |<span data-ttu-id="d8537-123">`schedule` の ID。</span><span class="sxs-lookup"><span data-stu-id="d8537-123">ID of the `schedule`.</span></span>|
| <span data-ttu-id="d8537-124">enabled</span><span class="sxs-lookup"><span data-stu-id="d8537-124">enabled</span></span>               |`bool`    | <span data-ttu-id="d8537-125">スケジュールがチームに対して有効になっているかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="d8537-125">Indicates whether the schedule is enabled for the team.</span></span> <span data-ttu-id="d8537-126">必須です。</span><span class="sxs-lookup"><span data-stu-id="d8537-126">Required.</span></span>|
| <span data-ttu-id="d8537-127">timeZone</span><span class="sxs-lookup"><span data-stu-id="d8537-127">timeZone</span></span>              |`string`  | <span data-ttu-id="d8537-128">tz データベース形式を使用して、スケジュールチームのタイムゾーンを示します。</span><span class="sxs-lookup"><span data-stu-id="d8537-128">Indicates the time zone of the schedule team using tz database format.</span></span> <span data-ttu-id="d8537-129">必須です。</span><span class="sxs-lookup"><span data-stu-id="d8537-129">Required.</span></span>|
| <span data-ttu-id="d8537-130">provisionStatus</span><span class="sxs-lookup"><span data-stu-id="d8537-130">provisionStatus</span></span>       |`operationStatus`    | <span data-ttu-id="d8537-131">スケジュールの準備の状態。</span><span class="sxs-lookup"><span data-stu-id="d8537-131">The status of the schedule provisioning.</span></span> <span data-ttu-id="d8537-132">使用可能な値`notStarted`は`running` `completed`、、 `failed`、です。</span><span class="sxs-lookup"><span data-stu-id="d8537-132">The possible values are `notStarted`, `running`, `completed`, `failed`.</span></span> |
| <span data-ttu-id="d8537-133">provisionStatusCode</span><span class="sxs-lookup"><span data-stu-id="d8537-133">provisionStatusCode</span></span>   |`string`  | <span data-ttu-id="d8537-134">スケジュールプロビジョニングが失敗した理由に関する追加情報。</span><span class="sxs-lookup"><span data-stu-id="d8537-134">Additional information about why schedule provisioning failed.</span></span> |


## <a name="relationships"></a><span data-ttu-id="d8537-135">関係</span><span class="sxs-lookup"><span data-stu-id="d8537-135">Relationships</span></span>
|<span data-ttu-id="d8537-136">名前</span><span class="sxs-lookup"><span data-stu-id="d8537-136">Name</span></span>                   |<span data-ttu-id="d8537-137">型</span><span class="sxs-lookup"><span data-stu-id="d8537-137">Type</span></span>           |<span data-ttu-id="d8537-138">説明</span><span class="sxs-lookup"><span data-stu-id="d8537-138">Description</span></span>                                                                                                                                      |
|-----------------------|---------------|-------------------------------------------------------------------------------------------------------------------------------------------------|
| <span data-ttu-id="d8537-139">移す</span><span class="sxs-lookup"><span data-stu-id="d8537-139">shifts</span></span>   |`collection(shift)`  | <span data-ttu-id="d8537-140">スケジュールのシフト。</span><span class="sxs-lookup"><span data-stu-id="d8537-140">The shifts in the schedule.</span></span> |
| <span data-ttu-id="d8537-141">timesoff</span><span class="sxs-lookup"><span data-stu-id="d8537-141">timesOff</span></span>   |`collection(timeOff)`  | <span data-ttu-id="d8537-142">スケジュールでオフにされた回数のインスタンス。</span><span class="sxs-lookup"><span data-stu-id="d8537-142">The instances of times off in the schedule.</span></span> |
| <span data-ttu-id="d8537-143">timeoffreasons</span><span class="sxs-lookup"><span data-stu-id="d8537-143">timeOffReasons</span></span>   |`collection(timeOffReason)`  | <span data-ttu-id="d8537-144">スケジュールで時間切れがある理由のセット。</span><span class="sxs-lookup"><span data-stu-id="d8537-144">The set of reasons for a time off in the schedule.</span></span> |
| <span data-ttu-id="d8537-145">schedulingGroups</span><span class="sxs-lookup"><span data-stu-id="d8537-145">schedulingGroups</span></span>   |`collection(schedulingGroup)`  | <span data-ttu-id="d8537-146">スケジュールに含まれるユーザーの論理グループ (通常は、役割別)。</span><span class="sxs-lookup"><span data-stu-id="d8537-146">The logical grouping of users in the schedule (usually by role).</span></span> |


## <a name="json-representation"></a><span data-ttu-id="d8537-147">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="d8537-147">JSON representation</span></span>

<span data-ttu-id="d8537-148">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="d8537-148">Here is a JSON representation of the resource.</span></span>

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
