---
title: スケジュールリソースの種類
description: チーム内の schedulingGroups、シフト、timeoffreasons 各理由と timesoff のコレクション。
author: nkramer
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: de3662fcf3c5a8e50493e365f6a10a8641a451df
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32563143"
---
# <a name="schedule-resource-type"></a><span data-ttu-id="361f7-103">スケジュールリソースの種類</span><span class="sxs-lookup"><span data-stu-id="361f7-103">schedule resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="361f7-104">[チーム](../resources/team.md)内の[schedulingGroup](schedulinggroup.md)オブジェクト、 [shift](shift.md)オブジェクト、 [timeoffreason](timeoffreason.md)オブジェクト、および[timeoff](timeoff.md)オブジェクトのコレクションです。</span><span class="sxs-lookup"><span data-stu-id="361f7-104">A collection of [schedulingGroup](schedulinggroup.md) objects, [shift](shift.md) objects, [timeOffReason](timeoffreason.md) objects, and [timeOff](timeoff.md) objects within a [team](../resources/team.md).</span></span> 

## <a name="methods"></a><span data-ttu-id="361f7-105">メソッド</span><span class="sxs-lookup"><span data-stu-id="361f7-105">Methods</span></span>

| <span data-ttu-id="361f7-106">メソッド</span><span class="sxs-lookup"><span data-stu-id="361f7-106">Method</span></span>       | <span data-ttu-id="361f7-107">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="361f7-107">Return Type</span></span>  |<span data-ttu-id="361f7-108">説明</span><span class="sxs-lookup"><span data-stu-id="361f7-108">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="361f7-109">スケジュールを作成または置換する</span><span class="sxs-lookup"><span data-stu-id="361f7-109">Create or replace schedule</span></span>](../api/team-put-schedule.md) | [<span data-ttu-id="361f7-110">スケジューリング</span><span class="sxs-lookup"><span data-stu-id="361f7-110">schedule</span></span>](schedule.md) | <span data-ttu-id="361f7-111">を`schedule`作成または置換します。</span><span class="sxs-lookup"><span data-stu-id="361f7-111">Create or replace a `schedule`.</span></span>|
|[<span data-ttu-id="361f7-112">スケジュールを取得する</span><span class="sxs-lookup"><span data-stu-id="361f7-112">Get schedule</span></span>](../api/schedule-get.md) | [<span data-ttu-id="361f7-113">スケジューリング</span><span class="sxs-lookup"><span data-stu-id="361f7-113">schedule</span></span>](schedule.md) | <span data-ttu-id="361f7-114">を`schedule`取得します。</span><span class="sxs-lookup"><span data-stu-id="361f7-114">Get a `schedule`.</span></span>|
|[<span data-ttu-id="361f7-115">share</span><span class="sxs-lookup"><span data-stu-id="361f7-115">share</span></span>](../api/schedule-share.md) | <span data-ttu-id="361f7-116">なし</span><span class="sxs-lookup"><span data-stu-id="361f7-116">None</span></span> | <span data-ttu-id="361f7-117">スケジュールメンバー `schedule`で時間範囲を共有します。</span><span class="sxs-lookup"><span data-stu-id="361f7-117">Share a `schedule` time range with schedule members.</span></span>|

## <a name="properties"></a><span data-ttu-id="361f7-118">プロパティ</span><span class="sxs-lookup"><span data-stu-id="361f7-118">Properties</span></span>
|<span data-ttu-id="361f7-119">名前</span><span class="sxs-lookup"><span data-stu-id="361f7-119">Name</span></span>                   |<span data-ttu-id="361f7-120">型</span><span class="sxs-lookup"><span data-stu-id="361f7-120">Type</span></span>           |<span data-ttu-id="361f7-121">説明</span><span class="sxs-lookup"><span data-stu-id="361f7-121">Description</span></span>                                                                                                                                      |
|-----------------------|---------------|-------------------------------------------------------------------------------------------------------------------------------------------------|
| <span data-ttu-id="361f7-122">id</span><span class="sxs-lookup"><span data-stu-id="361f7-122">id</span></span>                    |`string`  |<span data-ttu-id="361f7-123">`schedule` の ID。</span><span class="sxs-lookup"><span data-stu-id="361f7-123">ID of the `schedule`.</span></span>|
| <span data-ttu-id="361f7-124">enabled</span><span class="sxs-lookup"><span data-stu-id="361f7-124">enabled</span></span>               |`bool`    | <span data-ttu-id="361f7-125">スケジュールがチームに対して有効になっているかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="361f7-125">Indicates whether the schedule is enabled for the team.</span></span> <span data-ttu-id="361f7-126">必須です。</span><span class="sxs-lookup"><span data-stu-id="361f7-126">Required.</span></span>|
| <span data-ttu-id="361f7-127">timeZone</span><span class="sxs-lookup"><span data-stu-id="361f7-127">timeZone</span></span>              |`string`  | <span data-ttu-id="361f7-128">tz データベース形式を使用して、スケジュールチームのタイムゾーンを示します。</span><span class="sxs-lookup"><span data-stu-id="361f7-128">Indicates the time zone of the schedule team using tz database format.</span></span> <span data-ttu-id="361f7-129">必須です。</span><span class="sxs-lookup"><span data-stu-id="361f7-129">Required.</span></span>|
| <span data-ttu-id="361f7-130">provisionStatus</span><span class="sxs-lookup"><span data-stu-id="361f7-130">provisionStatus</span></span>       |`enum`    | <span data-ttu-id="361f7-131">スケジュールの準備の状態。</span><span class="sxs-lookup"><span data-stu-id="361f7-131">The status of the schedule provisioning.</span></span> |
| <span data-ttu-id="361f7-132">provisionStatusCode</span><span class="sxs-lookup"><span data-stu-id="361f7-132">provisionStatusCode</span></span>   |`string`  | <span data-ttu-id="361f7-133">スケジュールプロビジョニングが失敗した理由に関する追加情報。</span><span class="sxs-lookup"><span data-stu-id="361f7-133">Additional information about why schedule provisioning failed.</span></span> |


## <a name="relationships"></a><span data-ttu-id="361f7-134">関係</span><span class="sxs-lookup"><span data-stu-id="361f7-134">Relationships</span></span>
|<span data-ttu-id="361f7-135">名前</span><span class="sxs-lookup"><span data-stu-id="361f7-135">Name</span></span>                   |<span data-ttu-id="361f7-136">型</span><span class="sxs-lookup"><span data-stu-id="361f7-136">Type</span></span>           |<span data-ttu-id="361f7-137">説明</span><span class="sxs-lookup"><span data-stu-id="361f7-137">Description</span></span>                                                                                                                                      |
|-----------------------|---------------|-------------------------------------------------------------------------------------------------------------------------------------------------|
| <span data-ttu-id="361f7-138">移す</span><span class="sxs-lookup"><span data-stu-id="361f7-138">shifts</span></span>   |`collection(shift)`  | <span data-ttu-id="361f7-139">スケジュールのシフト。</span><span class="sxs-lookup"><span data-stu-id="361f7-139">The shifts in the schedule.</span></span> |
| <span data-ttu-id="361f7-140">timesoff</span><span class="sxs-lookup"><span data-stu-id="361f7-140">timesOff</span></span>   |`collection(timeOff)`  | <span data-ttu-id="361f7-141">スケジュールでオフにされた回数のインスタンス。</span><span class="sxs-lookup"><span data-stu-id="361f7-141">The instances of times off in the schedule.</span></span> |
| <span data-ttu-id="361f7-142">timeoffreasons</span><span class="sxs-lookup"><span data-stu-id="361f7-142">timeOffReasons</span></span>   |`collection(timeOffReason)`  | <span data-ttu-id="361f7-143">スケジュールで時間切れがある理由のセット。</span><span class="sxs-lookup"><span data-stu-id="361f7-143">The set of reasons for a time off in the schedule.</span></span> |
| <span data-ttu-id="361f7-144">schedulingGroups</span><span class="sxs-lookup"><span data-stu-id="361f7-144">schedulingGroups</span></span>   |`collection(schedulingGroup)`  | <span data-ttu-id="361f7-145">スケジュールに含まれるユーザーの論理グループ (通常は、役割別)。</span><span class="sxs-lookup"><span data-stu-id="361f7-145">The logical grouping of users in the schedule (usually by role).</span></span> |


## <a name="json-representation"></a><span data-ttu-id="361f7-146">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="361f7-146">JSON representation</span></span>

<span data-ttu-id="361f7-147">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="361f7-147">Here is a JSON representation of the resource.</span></span>

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
  "suppressions": [
    "Error: /api-reference/beta/resources/schedule.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
