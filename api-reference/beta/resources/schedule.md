---
title: スケジュールリソースの種類
description: チーム内の schedulingGroups、シフト、timeoffreasons 各理由と timesoff のコレクション。
author: nkramer
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: de3662fcf3c5a8e50493e365f6a10a8641a451df
ms.sourcegitcommit: 081cacecb4960aabc9e1011d12f06fe9ecf7d188
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 03/16/2019
ms.locfileid: "30657512"
---
# <a name="schedule-resource-type"></a><span data-ttu-id="b1d59-103">スケジュールリソースの種類</span><span class="sxs-lookup"><span data-stu-id="b1d59-103">schedule resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="b1d59-104">[チーム](../resources/team.md)内の[schedulingGroup](schedulinggroup.md)オブジェクト、 [shift](shift.md)オブジェクト、 [timeoffreason](timeoffreason.md)オブジェクト、および[timeoff](timeoff.md)オブジェクトのコレクションです。</span><span class="sxs-lookup"><span data-stu-id="b1d59-104">A collection of [schedulingGroup](schedulinggroup.md) objects, [shift](shift.md) objects, [timeOffReason](timeoffreason.md) objects, and [timeOff](timeoff.md) objects within a [team](../resources/team.md).</span></span> 

## <a name="methods"></a><span data-ttu-id="b1d59-105">メソッド</span><span class="sxs-lookup"><span data-stu-id="b1d59-105">Methods</span></span>

| <span data-ttu-id="b1d59-106">メソッド</span><span class="sxs-lookup"><span data-stu-id="b1d59-106">Method</span></span>       | <span data-ttu-id="b1d59-107">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="b1d59-107">Return Type</span></span>  |<span data-ttu-id="b1d59-108">説明</span><span class="sxs-lookup"><span data-stu-id="b1d59-108">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="b1d59-109">スケジュールを作成または置換する</span><span class="sxs-lookup"><span data-stu-id="b1d59-109">Create or replace schedule</span></span>](../api/team-put-schedule.md) | [<span data-ttu-id="b1d59-110">スケジューリング</span><span class="sxs-lookup"><span data-stu-id="b1d59-110">schedule</span></span>](schedule.md) | <span data-ttu-id="b1d59-111">を`schedule`作成または置換します。</span><span class="sxs-lookup"><span data-stu-id="b1d59-111">Create or replace a `schedule`.</span></span>|
|[<span data-ttu-id="b1d59-112">スケジュールを取得する</span><span class="sxs-lookup"><span data-stu-id="b1d59-112">Get schedule</span></span>](../api/schedule-get.md) | [<span data-ttu-id="b1d59-113">スケジューリング</span><span class="sxs-lookup"><span data-stu-id="b1d59-113">schedule</span></span>](schedule.md) | <span data-ttu-id="b1d59-114">を`schedule`取得します。</span><span class="sxs-lookup"><span data-stu-id="b1d59-114">Get a `schedule`.</span></span>|
|[<span data-ttu-id="b1d59-115">share</span><span class="sxs-lookup"><span data-stu-id="b1d59-115">share</span></span>](../api/schedule-share.md) | <span data-ttu-id="b1d59-116">なし</span><span class="sxs-lookup"><span data-stu-id="b1d59-116">None</span></span> | <span data-ttu-id="b1d59-117">スケジュールメンバー `schedule`で時間範囲を共有します。</span><span class="sxs-lookup"><span data-stu-id="b1d59-117">Share a `schedule` time range with schedule members.</span></span>|

## <a name="properties"></a><span data-ttu-id="b1d59-118">プロパティ</span><span class="sxs-lookup"><span data-stu-id="b1d59-118">Properties</span></span>
|<span data-ttu-id="b1d59-119">名前</span><span class="sxs-lookup"><span data-stu-id="b1d59-119">Name</span></span>                   |<span data-ttu-id="b1d59-120">型</span><span class="sxs-lookup"><span data-stu-id="b1d59-120">Type</span></span>           |<span data-ttu-id="b1d59-121">説明</span><span class="sxs-lookup"><span data-stu-id="b1d59-121">Description</span></span>                                                                                                                                      |
|-----------------------|---------------|-------------------------------------------------------------------------------------------------------------------------------------------------|
| <span data-ttu-id="b1d59-122">id</span><span class="sxs-lookup"><span data-stu-id="b1d59-122">id</span></span>                    |`string`  |<span data-ttu-id="b1d59-123">の ID `schedule`。</span><span class="sxs-lookup"><span data-stu-id="b1d59-123">ID of the `schedule`.</span></span>|
| <span data-ttu-id="b1d59-124">enabled</span><span class="sxs-lookup"><span data-stu-id="b1d59-124">enabled</span></span>               |`bool`    | <span data-ttu-id="b1d59-125">スケジュールがチームに対して有効になっているかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="b1d59-125">Indicates whether the schedule is enabled for the team.</span></span> <span data-ttu-id="b1d59-126">必須。</span><span class="sxs-lookup"><span data-stu-id="b1d59-126">Required.</span></span>|
| <span data-ttu-id="b1d59-127">timeZone</span><span class="sxs-lookup"><span data-stu-id="b1d59-127">timeZone</span></span>              |`string`  | <span data-ttu-id="b1d59-128">tz データベース形式を使用して、スケジュールチームのタイムゾーンを示します。</span><span class="sxs-lookup"><span data-stu-id="b1d59-128">Indicates the time zone of the schedule team using tz database format.</span></span> <span data-ttu-id="b1d59-129">必須。</span><span class="sxs-lookup"><span data-stu-id="b1d59-129">Required.</span></span>|
| <span data-ttu-id="b1d59-130">provisionStatus</span><span class="sxs-lookup"><span data-stu-id="b1d59-130">provisionStatus</span></span>       |`enum`    | <span data-ttu-id="b1d59-131">スケジュールの準備の状態。</span><span class="sxs-lookup"><span data-stu-id="b1d59-131">The status of the schedule provisioning.</span></span> |
| <span data-ttu-id="b1d59-132">provisionStatusCode</span><span class="sxs-lookup"><span data-stu-id="b1d59-132">provisionStatusCode</span></span>   |`string`  | <span data-ttu-id="b1d59-133">スケジュールプロビジョニングが失敗した理由に関する追加情報。</span><span class="sxs-lookup"><span data-stu-id="b1d59-133">Additional information about why schedule provisioning failed.</span></span> |


## <a name="relationships"></a><span data-ttu-id="b1d59-134">関係</span><span class="sxs-lookup"><span data-stu-id="b1d59-134">Relationships</span></span>
|<span data-ttu-id="b1d59-135">名前</span><span class="sxs-lookup"><span data-stu-id="b1d59-135">Name</span></span>                   |<span data-ttu-id="b1d59-136">型</span><span class="sxs-lookup"><span data-stu-id="b1d59-136">Type</span></span>           |<span data-ttu-id="b1d59-137">説明</span><span class="sxs-lookup"><span data-stu-id="b1d59-137">Description</span></span>                                                                                                                                      |
|-----------------------|---------------|-------------------------------------------------------------------------------------------------------------------------------------------------|
| <span data-ttu-id="b1d59-138">移す</span><span class="sxs-lookup"><span data-stu-id="b1d59-138">shifts</span></span>   |`collection(shift)`  | <span data-ttu-id="b1d59-139">スケジュールのシフト。</span><span class="sxs-lookup"><span data-stu-id="b1d59-139">The shifts in the schedule.</span></span> |
| <span data-ttu-id="b1d59-140">timesoff</span><span class="sxs-lookup"><span data-stu-id="b1d59-140">timesOff</span></span>   |`collection(timeOff)`  | <span data-ttu-id="b1d59-141">スケジュールでオフにされた回数のインスタンス。</span><span class="sxs-lookup"><span data-stu-id="b1d59-141">The instances of times off in the schedule.</span></span> |
| <span data-ttu-id="b1d59-142">timeoffreasons</span><span class="sxs-lookup"><span data-stu-id="b1d59-142">timeOffReasons</span></span>   |`collection(timeOffReason)`  | <span data-ttu-id="b1d59-143">スケジュールで時間切れがある理由のセット。</span><span class="sxs-lookup"><span data-stu-id="b1d59-143">The set of reasons for a time off in the schedule.</span></span> |
| <span data-ttu-id="b1d59-144">schedulingGroups</span><span class="sxs-lookup"><span data-stu-id="b1d59-144">schedulingGroups</span></span>   |`collection(schedulingGroup)`  | <span data-ttu-id="b1d59-145">スケジュールに含まれるユーザーの論理グループ (通常は、役割別)。</span><span class="sxs-lookup"><span data-stu-id="b1d59-145">The logical grouping of users in the schedule (usually by role).</span></span> |


## <a name="json-representation"></a><span data-ttu-id="b1d59-146">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="b1d59-146">JSON representation</span></span>

<span data-ttu-id="b1d59-147">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="b1d59-147">Here is a JSON representation of the resource.</span></span>

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
