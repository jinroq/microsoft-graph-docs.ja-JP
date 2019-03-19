---
title: リソースの種類の timeoff
description: スケジュールに含まれる非稼働時間の単位。
author: nkramer
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: c15d65c6d0a5a9749654698a51996cb21c254a9d
ms.sourcegitcommit: f58ff560fa02ac95e296375c143b0922fb6a425c
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 03/19/2019
ms.locfileid: "30676990"
---
# <a name="timeoff-resource-type"></a><span data-ttu-id="65f2f-103">リソースの種類の timeoff</span><span class="sxs-lookup"><span data-stu-id="65f2f-103">timeOff resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="65f2f-104">スケジュールに含まれる非稼働時間の単位。</span><span class="sxs-lookup"><span data-stu-id="65f2f-104">A unit of non-work in the schedule.</span></span>

## <a name="methods"></a><span data-ttu-id="65f2f-105">メソッド</span><span class="sxs-lookup"><span data-stu-id="65f2f-105">Methods</span></span>

| <span data-ttu-id="65f2f-106">メソッド</span><span class="sxs-lookup"><span data-stu-id="65f2f-106">Method</span></span>       | <span data-ttu-id="65f2f-107">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="65f2f-107">Return Type</span></span>  |<span data-ttu-id="65f2f-108">説明</span><span class="sxs-lookup"><span data-stu-id="65f2f-108">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="65f2f-109">timeoff の作成</span><span class="sxs-lookup"><span data-stu-id="65f2f-109">Create timeOff</span></span>](../api/schedule-post-timesoff.md) | [<span data-ttu-id="65f2f-110">timeoff</span><span class="sxs-lookup"><span data-stu-id="65f2f-110">timeOff</span></span>](timeOff.md) | <span data-ttu-id="65f2f-111">新しい `timeOff` オブジェクトを作成します。</span><span class="sxs-lookup"><span data-stu-id="65f2f-111">Create a new `timeOff` object.</span></span>|
|[<span data-ttu-id="65f2f-112">timeoffs のリスト</span><span class="sxs-lookup"><span data-stu-id="65f2f-112">List timeOffs</span></span>](../api/schedule-list-timesoff.md) | <span data-ttu-id="65f2f-113">[timeoff](timeOff.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="65f2f-113">[timeOff](timeOff.md) collection</span></span> | <span data-ttu-id="65f2f-114">このスケジュールでオブジェクト`timeOff`のリストを取得します。</span><span class="sxs-lookup"><span data-stu-id="65f2f-114">Get the list of `timeOff` objects in this schedule.</span></span>|
|[<span data-ttu-id="65f2f-115">timeoff を取得する</span><span class="sxs-lookup"><span data-stu-id="65f2f-115">Get timeOff</span></span>](../api/timeoff-get.md) | [<span data-ttu-id="65f2f-116">timeoff</span><span class="sxs-lookup"><span data-stu-id="65f2f-116">timeOff</span></span>](timeOff.md) | <span data-ttu-id="65f2f-117">ID で `timeOff` を取得します。</span><span class="sxs-lookup"><span data-stu-id="65f2f-117">Get a `timeOff` by ID.</span></span>|
|[<span data-ttu-id="65f2f-118">timeoff を置換する</span><span class="sxs-lookup"><span data-stu-id="65f2f-118">Replace timeOff</span></span>](../api/timeoff-put.md) | [<span data-ttu-id="65f2f-119">timeoff</span><span class="sxs-lookup"><span data-stu-id="65f2f-119">timeOff</span></span>](timeOff.md) | <span data-ttu-id="65f2f-120">`timeOff` を置き換えます。</span><span class="sxs-lookup"><span data-stu-id="65f2f-120">Replace a `timeOff`.</span></span>|
|[<span data-ttu-id="65f2f-121">timeoff の削除</span><span class="sxs-lookup"><span data-stu-id="65f2f-121">Delete timeOff</span></span>](../api/timeoff-delete.md) | <span data-ttu-id="65f2f-122">なし</span><span class="sxs-lookup"><span data-stu-id="65f2f-122">None</span></span> | <span data-ttu-id="65f2f-123">スケジュールから`timeOff`を削除します。</span><span class="sxs-lookup"><span data-stu-id="65f2f-123">Delete a `timeOff` from the schedule.</span></span>|

## <a name="properties"></a><span data-ttu-id="65f2f-124">プロパティ</span><span class="sxs-lookup"><span data-stu-id="65f2f-124">Properties</span></span>
|<span data-ttu-id="65f2f-125">名前</span><span class="sxs-lookup"><span data-stu-id="65f2f-125">Name</span></span>          |<span data-ttu-id="65f2f-126">種類</span><span class="sxs-lookup"><span data-stu-id="65f2f-126">Type</span></span>           |<span data-ttu-id="65f2f-127">説明</span><span class="sxs-lookup"><span data-stu-id="65f2f-127">Description</span></span>                                                                                                                                      |
|--------------|---------------|-------------------------------------------------------------------------------------------------------------------------------------------------|
| <span data-ttu-id="65f2f-128">id</span><span class="sxs-lookup"><span data-stu-id="65f2f-128">id</span></span>            |`string`      |<span data-ttu-id="65f2f-129">`timeOff` の ID。</span><span class="sxs-lookup"><span data-stu-id="65f2f-129">ID of the `timeOff`.</span></span>|
| <span data-ttu-id="65f2f-130">userId</span><span class="sxs-lookup"><span data-stu-id="65f2f-130">userId</span></span>            |`string`      |<span data-ttu-id="65f2f-131">に割り当てられているユーザー `timeOff`の ID。</span><span class="sxs-lookup"><span data-stu-id="65f2f-131">ID of the user assigned to the `timeOff`.</span></span> <span data-ttu-id="65f2f-132">必須。</span><span class="sxs-lookup"><span data-stu-id="65f2f-132">Required.</span></span>|
| <span data-ttu-id="65f2f-133">sharedtimeoff</span><span class="sxs-lookup"><span data-stu-id="65f2f-133">sharedTimeOff</span></span>     |[<span data-ttu-id="65f2f-134">timeoffitem</span><span class="sxs-lookup"><span data-stu-id="65f2f-134">timeOffItem</span></span>](timeoffitem.md)  |<span data-ttu-id="65f2f-135">従業員とマネージャーの両方`timeOff`に表示される共有バージョン。</span><span class="sxs-lookup"><span data-stu-id="65f2f-135">The shared version of this `timeOff` that is viewable by both employees and managers.</span></span> <span data-ttu-id="65f2f-136">必須。</span><span class="sxs-lookup"><span data-stu-id="65f2f-136">Required.</span></span>|
| <span data-ttu-id="65f2f-137">draftTimeOff</span><span class="sxs-lookup"><span data-stu-id="65f2f-137">draftTimeOff</span></span>      |[<span data-ttu-id="65f2f-138">timeoffitem</span><span class="sxs-lookup"><span data-stu-id="65f2f-138">timeOffItem</span></span>](timeoffitem.md)        |<span data-ttu-id="65f2f-139">この`timeOff`の下書きバージョンは、マネージャーが表示できます。</span><span class="sxs-lookup"><span data-stu-id="65f2f-139">The draft version of this `timeOff` that is viewable by managers.</span></span> <span data-ttu-id="65f2f-140">必須。</span><span class="sxs-lookup"><span data-stu-id="65f2f-140">Required.</span></span>|
| <span data-ttu-id="65f2f-141">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="65f2f-141">createdDateTime</span></span>       |`DateTimeOffset`        |<span data-ttu-id="65f2f-142">これ`timeOff`が最初に作成されたタイムスタンプ。</span><span class="sxs-lookup"><span data-stu-id="65f2f-142">The time stamp at which this `timeOff` was first created.</span></span> <span data-ttu-id="65f2f-143">Timestamp 型は、ISO 8601 形式を使用して日付と時刻の情報を表します。これは常に UTC 時間です。</span><span class="sxs-lookup"><span data-stu-id="65f2f-143">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="65f2f-144">たとえば、2014 年 1 月 1 日午前 0 時 (UTC) は、'2014-01-01T00:00:00Z'.のようになります。</span><span class="sxs-lookup"><span data-stu-id="65f2f-144">For example, midnight UTC on Jan 1, 2014 would look like this: '2014-01-01T00:00:00Z'.</span></span> |
| <span data-ttu-id="65f2f-145">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="65f2f-145">lastModifiedDateTime</span></span>      |`DateTimeOffset`        |<span data-ttu-id="65f2f-146">これ`timeOff`が最後に更新されたタイムスタンプ。</span><span class="sxs-lookup"><span data-stu-id="65f2f-146">The time stamp at which this `timeOff` was last updated.</span></span> <span data-ttu-id="65f2f-147">Timestamp 型は、ISO 8601 形式を使用して日付と時刻の情報を表します。これは常に UTC 時間です。</span><span class="sxs-lookup"><span data-stu-id="65f2f-147">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="65f2f-148">たとえば、2014 年 1 月 1 日午前 0 時 (UTC) は、'2014-01-01T00:00:00Z'.のようになります。</span><span class="sxs-lookup"><span data-stu-id="65f2f-148">For example, midnight UTC on Jan 1, 2014 would look like this: '2014-01-01T00:00:00Z'.</span></span> |
| <span data-ttu-id="65f2f-149">lastModifiedBy</span><span class="sxs-lookup"><span data-stu-id="65f2f-149">lastModifiedBy</span></span>        |`microsoft.graph.identitySet`        |<span data-ttu-id="65f2f-150">この `timeOff` を最後に更新した ID。</span><span class="sxs-lookup"><span data-stu-id="65f2f-150">The identity that last updated this `timeOff`.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="65f2f-151">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="65f2f-151">JSON representation</span></span>

<span data-ttu-id="65f2f-152">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="65f2f-152">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.timeOff"
}-->

```json
{
  "userId": "c5d0c76b-80c4-481c-be50-923cd8d680a1",
  "createdDateTime": "2019-03-14T05:35:57.755Z",
  "lastModifiedDateTime": "2019-03-14T05:36:08.381Z",
  "lastModifiedBy": {
    "application": null,
    "device": null,
    "conversation": null,
    "user": {
      "id": "366c0b19-49b1-41b5-a03f-9f3887bd0ed8",
      "displayName": "John Doe"
    }
  },
  "sharedTimeOff": {
    "timeOffReasonId": "TOR_891045ca-b5d2-406b-aa06-a3c8921245d7",
    "startDateTime": "2019-03-11T07:00:00Z",
    "endDateTime": "2019-03-12T07:00:00Z",
    "theme": "white"
  },
  "draftTimeOff": {
    "timeOffReasonId": "TOR_891045ca-b5d2-406b-aa06-a3c8921245d7",
    "startDateTime": "2019-03-11T07:00:00Z",
    "endDateTime": "2019-03-12T07:00:00Z",
    "theme": "pink"
  }
}
```


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "timeOff resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/timeoff.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
