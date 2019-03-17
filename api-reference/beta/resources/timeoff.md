---
title: リソースの種類の timeoff
description: スケジュールに含まれる非稼働時間の単位。
author: nkramer
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: 933c940e25c772cede7918dabf62b52ee58f18d2
ms.sourcegitcommit: 081cacecb4960aabc9e1011d12f06fe9ecf7d188
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 03/16/2019
ms.locfileid: "30657799"
---
# <a name="timeoff-resource-type"></a><span data-ttu-id="d51d9-103">リソースの種類の timeoff</span><span class="sxs-lookup"><span data-stu-id="d51d9-103">timeOff resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="d51d9-104">スケジュールに含まれる非稼働時間の単位。</span><span class="sxs-lookup"><span data-stu-id="d51d9-104">A unit of non-work in the schedule.</span></span>

## <a name="methods"></a><span data-ttu-id="d51d9-105">メソッド</span><span class="sxs-lookup"><span data-stu-id="d51d9-105">Methods</span></span>

| <span data-ttu-id="d51d9-106">メソッド</span><span class="sxs-lookup"><span data-stu-id="d51d9-106">Method</span></span>       | <span data-ttu-id="d51d9-107">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="d51d9-107">Return Type</span></span>  |<span data-ttu-id="d51d9-108">説明</span><span class="sxs-lookup"><span data-stu-id="d51d9-108">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="d51d9-109">timeoff の作成</span><span class="sxs-lookup"><span data-stu-id="d51d9-109">Create timeOff</span></span>](../api/schedule-post-timesoff.md) | [<span data-ttu-id="d51d9-110">timeoff</span><span class="sxs-lookup"><span data-stu-id="d51d9-110">timeOff</span></span>](timeOff.md) | <span data-ttu-id="d51d9-111">新しい `timeOff` オブジェクトを作成します。</span><span class="sxs-lookup"><span data-stu-id="d51d9-111">Create a new `timeOff` object.</span></span>|
|[<span data-ttu-id="d51d9-112">timeoffs のリスト</span><span class="sxs-lookup"><span data-stu-id="d51d9-112">List timeOffs</span></span>](../api/schedule-list-timesoff.md) | <span data-ttu-id="d51d9-113">[timeoff](timeOff.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="d51d9-113">[timeOff](timeOff.md) collection</span></span> | <span data-ttu-id="d51d9-114">このスケジュールでオブジェクト`timeOff`のリストを取得します。</span><span class="sxs-lookup"><span data-stu-id="d51d9-114">Get the list of `timeOff` objects in this schedule.</span></span>|
|[<span data-ttu-id="d51d9-115">timeoff を取得する</span><span class="sxs-lookup"><span data-stu-id="d51d9-115">Get timeOff</span></span>](../api/timeoff-get.md) | [<span data-ttu-id="d51d9-116">timeoff</span><span class="sxs-lookup"><span data-stu-id="d51d9-116">timeOff</span></span>](timeOff.md) | <span data-ttu-id="d51d9-117">ID `timeOff`で取得します。</span><span class="sxs-lookup"><span data-stu-id="d51d9-117">Get a `timeOff` by ID.</span></span>|
|[<span data-ttu-id="d51d9-118">timeoff を置換する</span><span class="sxs-lookup"><span data-stu-id="d51d9-118">Replace timeOff</span></span>](../api/timeoff-put.md) | [<span data-ttu-id="d51d9-119">timeoff</span><span class="sxs-lookup"><span data-stu-id="d51d9-119">timeOff</span></span>](timeOff.md) | <span data-ttu-id="d51d9-120">を`timeOff`置き換えます。</span><span class="sxs-lookup"><span data-stu-id="d51d9-120">Replace a `timeOff`.</span></span>|
|[<span data-ttu-id="d51d9-121">timeoff の削除</span><span class="sxs-lookup"><span data-stu-id="d51d9-121">Delete timeOff</span></span>](../api/timeoff-delete.md) | <span data-ttu-id="d51d9-122">なし</span><span class="sxs-lookup"><span data-stu-id="d51d9-122">None</span></span> | <span data-ttu-id="d51d9-123">スケジュールから`timeOff`を削除します。</span><span class="sxs-lookup"><span data-stu-id="d51d9-123">Delete a `timeOff` from the schedule.</span></span>|

## <a name="properties"></a><span data-ttu-id="d51d9-124">プロパティ</span><span class="sxs-lookup"><span data-stu-id="d51d9-124">Properties</span></span>
|<span data-ttu-id="d51d9-125">名前</span><span class="sxs-lookup"><span data-stu-id="d51d9-125">Name</span></span>          |<span data-ttu-id="d51d9-126">型</span><span class="sxs-lookup"><span data-stu-id="d51d9-126">Type</span></span>           |<span data-ttu-id="d51d9-127">説明</span><span class="sxs-lookup"><span data-stu-id="d51d9-127">Description</span></span>                                                                                                                                      |
|--------------|---------------|-------------------------------------------------------------------------------------------------------------------------------------------------|
| <span data-ttu-id="d51d9-128">id</span><span class="sxs-lookup"><span data-stu-id="d51d9-128">id</span></span>            |`string`      |<span data-ttu-id="d51d9-129">の ID `timeOff`。</span><span class="sxs-lookup"><span data-stu-id="d51d9-129">ID of the `timeOff`.</span></span>|
| <span data-ttu-id="d51d9-130">userId</span><span class="sxs-lookup"><span data-stu-id="d51d9-130">userId</span></span>            |`string`      |<span data-ttu-id="d51d9-131">に割り当てられているユーザー `timeOff`の ID。</span><span class="sxs-lookup"><span data-stu-id="d51d9-131">ID of the user assigned to the `timeOff`.</span></span> <span data-ttu-id="d51d9-132">必須。</span><span class="sxs-lookup"><span data-stu-id="d51d9-132">Required.</span></span>|
| <span data-ttu-id="d51d9-133">sharedtimeoff</span><span class="sxs-lookup"><span data-stu-id="d51d9-133">sharedTimeOff</span></span>     |`[timeOffItem](timeoffitem.md)`  |<span data-ttu-id="d51d9-134">従業員とマネージャーの両方`timeOff`に表示される共有バージョン。</span><span class="sxs-lookup"><span data-stu-id="d51d9-134">The shared version of this `timeOff` that is viewable by both employees and managers.</span></span> <span data-ttu-id="d51d9-135">必須。</span><span class="sxs-lookup"><span data-stu-id="d51d9-135">Required.</span></span>|
| <span data-ttu-id="d51d9-136">draftTimeOff</span><span class="sxs-lookup"><span data-stu-id="d51d9-136">draftTimeOff</span></span>      |`[timeOffItem](timeoffitem.md)`        |<span data-ttu-id="d51d9-137">この`timeOff`の下書きバージョンは、マネージャーが表示できます。</span><span class="sxs-lookup"><span data-stu-id="d51d9-137">The draft version of this `timeOff` that is viewable by managers.</span></span> <span data-ttu-id="d51d9-138">必須。</span><span class="sxs-lookup"><span data-stu-id="d51d9-138">Required.</span></span>|
| <span data-ttu-id="d51d9-139">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="d51d9-139">createdDateTime</span></span>       |`DateTimeOffset`        |<span data-ttu-id="d51d9-140">これ`timeOff`が最初に作成されたタイムスタンプ。</span><span class="sxs-lookup"><span data-stu-id="d51d9-140">The time stamp at which this `timeOff` was first created.</span></span> <span data-ttu-id="d51d9-141">Timestamp 型は、ISO 8601 形式を使用して日付と時刻の情報を表し、必ず UTC 時間です。</span><span class="sxs-lookup"><span data-stu-id="d51d9-141">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="d51d9-142">たとえば、2014年1月1日午前0時 (UTC) は次のようになります。 ' 2014-01-01t00:00: 00z ' のようになります。</span><span class="sxs-lookup"><span data-stu-id="d51d9-142">For example, midnight UTC on Jan 1, 2014 would look like this: '2014-01-01T00:00:00Z'.</span></span> |
| <span data-ttu-id="d51d9-143">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="d51d9-143">lastModifiedDateTime</span></span>      |`DateTimeOffset`        |<span data-ttu-id="d51d9-144">これ`timeOff`が最後に更新されたタイムスタンプ。</span><span class="sxs-lookup"><span data-stu-id="d51d9-144">The time stamp at which this `timeOff` was last updated.</span></span> <span data-ttu-id="d51d9-145">Timestamp 型は、ISO 8601 形式を使用して日付と時刻の情報を表し、必ず UTC 時間です。</span><span class="sxs-lookup"><span data-stu-id="d51d9-145">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="d51d9-146">たとえば、2014年1月1日午前0時 (UTC) は次のようになります。 ' 2014-01-01t00:00: 00z ' のようになります。</span><span class="sxs-lookup"><span data-stu-id="d51d9-146">For example, midnight UTC on Jan 1, 2014 would look like this: '2014-01-01T00:00:00Z'.</span></span> |
| <span data-ttu-id="d51d9-147">lastModifiedBy</span><span class="sxs-lookup"><span data-stu-id="d51d9-147">lastModifiedBy</span></span>        |`microsoft.graph.identitySet`        |<span data-ttu-id="d51d9-148">最後に更新`timeOff`した id。</span><span class="sxs-lookup"><span data-stu-id="d51d9-148">The identity that last updated this `timeOff`.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="d51d9-149">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="d51d9-149">JSON representation</span></span>

<span data-ttu-id="d51d9-150">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="d51d9-150">Here is a JSON representation of the resource.</span></span>

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
