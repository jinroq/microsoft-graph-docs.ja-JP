---
title: shift リソースの種類
description: shift は、スケジュールのスケジュールされた作業の単位です。
author: nkramer
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: c392bfb4a1691ab99d852febdda27cdf1c3b8044
ms.sourcegitcommit: 081cacecb4960aabc9e1011d12f06fe9ecf7d188
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 03/16/2019
ms.locfileid: "30657897"
---
# <a name="shift-resource-type"></a><span data-ttu-id="8f1a9-103">shift リソースの種類</span><span class="sxs-lookup"><span data-stu-id="8f1a9-103">shift resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="8f1a9-104">[スケジュール](schedule.md)に含まれるスケジュールされた作業の単位。</span><span class="sxs-lookup"><span data-stu-id="8f1a9-104">A unit of scheduled work in a [schedule](schedule.md).</span></span> 

## <a name="methods"></a><span data-ttu-id="8f1a9-105">メソッド</span><span class="sxs-lookup"><span data-stu-id="8f1a9-105">Methods</span></span>

| <span data-ttu-id="8f1a9-106">メソッド</span><span class="sxs-lookup"><span data-stu-id="8f1a9-106">Method</span></span>       | <span data-ttu-id="8f1a9-107">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="8f1a9-107">Return Type</span></span>  |<span data-ttu-id="8f1a9-108">説明</span><span class="sxs-lookup"><span data-stu-id="8f1a9-108">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="8f1a9-109">shift を作成する</span><span class="sxs-lookup"><span data-stu-id="8f1a9-109">Create shift</span></span>](../api/schedule-post-shifts.md) | [<span data-ttu-id="8f1a9-110">制</span><span class="sxs-lookup"><span data-stu-id="8f1a9-110">shift</span></span>](shift.md) | <span data-ttu-id="8f1a9-111">新しい`shift`を作成します。</span><span class="sxs-lookup"><span data-stu-id="8f1a9-111">Create a new `shift`.</span></span>|
|[<span data-ttu-id="8f1a9-112">シフトの一覧表示</span><span class="sxs-lookup"><span data-stu-id="8f1a9-112">List shifts</span></span>](../api/schedule-list-shifts.md) | <span data-ttu-id="8f1a9-113">[shift](shift.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="8f1a9-113">[shift](shift.md) collection</span></span> | <span data-ttu-id="8f1a9-114">このスケジュール内の`shifts`のリストを取得します。</span><span class="sxs-lookup"><span data-stu-id="8f1a9-114">Get the list of `shifts` in this schedule.</span></span>|
|[<span data-ttu-id="8f1a9-115">shift を取得する</span><span class="sxs-lookup"><span data-stu-id="8f1a9-115">Get shift</span></span>](../api/shift-get.md) | [<span data-ttu-id="8f1a9-116">制</span><span class="sxs-lookup"><span data-stu-id="8f1a9-116">shift</span></span>](shift.md) | <span data-ttu-id="8f1a9-117">ID `shift`で取得します。</span><span class="sxs-lookup"><span data-stu-id="8f1a9-117">Get a `shift` by ID.</span></span>|
|[<span data-ttu-id="8f1a9-118">shift を置換する</span><span class="sxs-lookup"><span data-stu-id="8f1a9-118">Replace shift</span></span>](../api/shift-put.md) | [<span data-ttu-id="8f1a9-119">制</span><span class="sxs-lookup"><span data-stu-id="8f1a9-119">shift</span></span>](shift.md) | <span data-ttu-id="8f1a9-120">を`shift`置き換えます。</span><span class="sxs-lookup"><span data-stu-id="8f1a9-120">Replace a `shift`.</span></span>|
|[<span data-ttu-id="8f1a9-121">shift を削除する</span><span class="sxs-lookup"><span data-stu-id="8f1a9-121">Delete shift</span></span>](../api/shift-delete.md) | <span data-ttu-id="8f1a9-122">なし</span><span class="sxs-lookup"><span data-stu-id="8f1a9-122">None</span></span> | <span data-ttu-id="8f1a9-123">スケジュールから`shift`を削除します。</span><span class="sxs-lookup"><span data-stu-id="8f1a9-123">Delete a `shift` from the schedule.</span></span>|

## <a name="properties"></a><span data-ttu-id="8f1a9-124">プロパティ</span><span class="sxs-lookup"><span data-stu-id="8f1a9-124">Properties</span></span>
|<span data-ttu-id="8f1a9-125">名前</span><span class="sxs-lookup"><span data-stu-id="8f1a9-125">Name</span></span>          |<span data-ttu-id="8f1a9-126">型</span><span class="sxs-lookup"><span data-stu-id="8f1a9-126">Type</span></span>           |<span data-ttu-id="8f1a9-127">説明</span><span class="sxs-lookup"><span data-stu-id="8f1a9-127">Description</span></span>                                                                                                                                      |
|--------------|---------------|-------------------------------------------------------------------------------------------------------------------------------------------------|
| <span data-ttu-id="8f1a9-128">id</span><span class="sxs-lookup"><span data-stu-id="8f1a9-128">id</span></span>            |`string`      |<span data-ttu-id="8f1a9-129">の ID `shift`。</span><span class="sxs-lookup"><span data-stu-id="8f1a9-129">ID of the `shift`.</span></span>|
| <span data-ttu-id="8f1a9-130">userId</span><span class="sxs-lookup"><span data-stu-id="8f1a9-130">userId</span></span>            |`string`      |<span data-ttu-id="8f1a9-131">に割り当てられているユーザー `shift`の ID。</span><span class="sxs-lookup"><span data-stu-id="8f1a9-131">ID of the user assigned to the `shift`.</span></span> <span data-ttu-id="8f1a9-132">必須。</span><span class="sxs-lookup"><span data-stu-id="8f1a9-132">Required.</span></span> |
| <span data-ttu-id="8f1a9-133">schedulingGroupId</span><span class="sxs-lookup"><span data-stu-id="8f1a9-133">schedulingGroupId</span></span>         |`string`      |<span data-ttu-id="8f1a9-134">`shift`が含まれるスケジュールグループの ID。</span><span class="sxs-lookup"><span data-stu-id="8f1a9-134">ID of the scheduling group the `shift` is part of.</span></span> <span data-ttu-id="8f1a9-135">必須。</span><span class="sxs-lookup"><span data-stu-id="8f1a9-135">Required.</span></span> |
| <span data-ttu-id="8f1a9-136">sharedshift</span><span class="sxs-lookup"><span data-stu-id="8f1a9-136">sharedShift</span></span>   |`[shiftItem](shiftitem.md)`  |<span data-ttu-id="8f1a9-137">従業員とマネージャーの両方`shift`に表示される共有バージョン。</span><span class="sxs-lookup"><span data-stu-id="8f1a9-137">The shared version of this `shift` that is viewable by both employees and managers.</span></span> <span data-ttu-id="8f1a9-138">必須。</span><span class="sxs-lookup"><span data-stu-id="8f1a9-138">Required.</span></span> |
| <span data-ttu-id="8f1a9-139">draftShift</span><span class="sxs-lookup"><span data-stu-id="8f1a9-139">draftShift</span></span>        |`[shiftItem](shiftitem.md)`        |<span data-ttu-id="8f1a9-140">この`shift`の下書きバージョンは、マネージャーが表示できます。</span><span class="sxs-lookup"><span data-stu-id="8f1a9-140">The draft version of this `shift` that is viewable by managers.</span></span> <span data-ttu-id="8f1a9-141">必須。</span><span class="sxs-lookup"><span data-stu-id="8f1a9-141">Required.</span></span> |
| <span data-ttu-id="8f1a9-142">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="8f1a9-142">createdDateTime</span></span>       |`DateTimeOffset`        |<span data-ttu-id="8f1a9-143">最初に作成さ`shift`れたタイムスタンプ。</span><span class="sxs-lookup"><span data-stu-id="8f1a9-143">The timestamp on which this `shift` was first created.</span></span> <span data-ttu-id="8f1a9-144">Timestamp 型は、ISO 8601 形式を使用して日付と時刻の情報を表し、必ず UTC 時間です。</span><span class="sxs-lookup"><span data-stu-id="8f1a9-144">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="8f1a9-145">たとえば、2014年1月1日午前0時 (UTC) は次のようになります。 ' 2014-01-01t00:00: 00z ' のようになります。</span><span class="sxs-lookup"><span data-stu-id="8f1a9-145">For example, midnight UTC on Jan 1, 2014 would look like this: '2014-01-01T00:00:00Z'.</span></span> |
| <span data-ttu-id="8f1a9-146">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="8f1a9-146">lastModifiedDateTime</span></span>      |`DateTimeOffset`        |<span data-ttu-id="8f1a9-147">最後に更新され`shift`たタイムスタンプ。</span><span class="sxs-lookup"><span data-stu-id="8f1a9-147">The timestamp on which this `shift` was last updated.</span></span> <span data-ttu-id="8f1a9-148">Timestamp 型は、ISO 8601 形式を使用して日付と時刻の情報を表し、必ず UTC 時間です。</span><span class="sxs-lookup"><span data-stu-id="8f1a9-148">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="8f1a9-149">たとえば、2014年1月1日午前0時 (UTC) は次のようになります。 ' 2014-01-01t00:00: 00z ' のようになります。</span><span class="sxs-lookup"><span data-stu-id="8f1a9-149">For example, midnight UTC on Jan 1, 2014 would look like this: '2014-01-01T00:00:00Z'.</span></span> |
| <span data-ttu-id="8f1a9-150">lastModifiedBy</span><span class="sxs-lookup"><span data-stu-id="8f1a9-150">lastModifiedBy</span></span>        |`microsoft.graph.identitySet`        |<span data-ttu-id="8f1a9-151">最後に更新`shift`した id。</span><span class="sxs-lookup"><span data-stu-id="8f1a9-151">The identity that last updated this `shift`.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="8f1a9-152">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="8f1a9-152">JSON representation</span></span>

<span data-ttu-id="8f1a9-153">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="8f1a9-153">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.shift"
}-->

```json
{
  "id": "SHFT_577b75d2-a927-48c0-a5d1-dc984894e7b8",
  "createdDateTime": "2019-03-14T04:32:51.451Z",
  "lastModifiedDateTime": "2019-03-14T05:32:51.451Z",
  "userId": "c5d0c76b-80c4-481c-be50-923cd8d680a1",
  "schedulingGroupId": "TAG_228940ed-ff84-4e25-b129-1b395cf78be0",
  "lastModifiedBy": {
    "application": null,
    "device": null,
    "conversation": null,
    "user": {
      "id": "366c0b19-49b1-41b5-a03f-9f3887bd0ed8",
      "displayName": "John Doe"
    }
  },
  "sharedShift": {
    "displayName": "Day shift",
    "notes": "Please do inventory as part of your shift.",
    "startDateTime": "2019-03-11T15:00:00Z",
    "endDateTime": "2019-03-12T00:00:00Z",
    "theme": "blue",
    "activities": [
      {
        "isPaid": true,
        "startDateTime": "2019-03-11T15:00:00Z",
        "endDateTime": "2019-03-11T15:15:00Z",
        "code": "",
        "displayName": "Lunch"
      }
    ]
  },
  "draftShift": {
    "displayName": "Day shift",
    "notes": "Please do inventory as part of your shift.",
    "startDateTime": "2019-03-11T15:00:00Z",
    "endDateTime": "2019-03-12T00:00:00Z",
    "theme": "blue",
    "activities": [
      {
        "isPaid": true,
        "startDateTime": "2019-03-11T15:00:00Z",
        "endDateTime": "2019-03-11T15:30:00Z",
        "code": "",
        "displayName": "Lunch"
      }
    ]
  }
}
```


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "shift resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/shift.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
