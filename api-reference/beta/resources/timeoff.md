---
title: リソースの種類の timeoff
description: スケジュールに含まれる非稼働時間の単位。
author: nkramer
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: 848365a812053b7788db37395bee8662d69cda37
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/26/2019
ms.locfileid: "33342035"
---
# <a name="timeoff-resource-type"></a><span data-ttu-id="333ab-103">リソースの種類の timeoff</span><span class="sxs-lookup"><span data-stu-id="333ab-103">timeOff resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="333ab-104">スケジュールに含まれる非稼働時間の単位。</span><span class="sxs-lookup"><span data-stu-id="333ab-104">A unit of non-work in the schedule.</span></span>

## <a name="methods"></a><span data-ttu-id="333ab-105">メソッド</span><span class="sxs-lookup"><span data-stu-id="333ab-105">Methods</span></span>

| <span data-ttu-id="333ab-106">メソッド</span><span class="sxs-lookup"><span data-stu-id="333ab-106">Method</span></span>       | <span data-ttu-id="333ab-107">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="333ab-107">Return Type</span></span>  |<span data-ttu-id="333ab-108">説明</span><span class="sxs-lookup"><span data-stu-id="333ab-108">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="333ab-109">timeoff の作成</span><span class="sxs-lookup"><span data-stu-id="333ab-109">Create timeOff</span></span>](../api/schedule-post-timesoff.md) | [<span data-ttu-id="333ab-110">timeoff</span><span class="sxs-lookup"><span data-stu-id="333ab-110">timeOff</span></span>](timeOff.md) | <span data-ttu-id="333ab-111">新しい `timeOff` オブジェクトを作成します。</span><span class="sxs-lookup"><span data-stu-id="333ab-111">Create a new `timeOff` object.</span></span>|
|[<span data-ttu-id="333ab-112">timeoffs のリスト</span><span class="sxs-lookup"><span data-stu-id="333ab-112">List timeOffs</span></span>](../api/schedule-list-timesoff.md) | <span data-ttu-id="333ab-113">[timeoff](timeOff.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="333ab-113">[timeOff](timeOff.md) collection</span></span> | <span data-ttu-id="333ab-114">このスケジュールでオブジェクト`timeOff`のリストを取得します。</span><span class="sxs-lookup"><span data-stu-id="333ab-114">Get the list of `timeOff` objects in this schedule.</span></span>|
|[<span data-ttu-id="333ab-115">timeoff を取得する</span><span class="sxs-lookup"><span data-stu-id="333ab-115">Get timeOff</span></span>](../api/timeoff-get.md) | [<span data-ttu-id="333ab-116">timeoff</span><span class="sxs-lookup"><span data-stu-id="333ab-116">timeOff</span></span>](timeOff.md) | <span data-ttu-id="333ab-117">ID で `timeOff` を取得します。</span><span class="sxs-lookup"><span data-stu-id="333ab-117">Get a `timeOff` by ID.</span></span>|
|[<span data-ttu-id="333ab-118">timeoff を置換する</span><span class="sxs-lookup"><span data-stu-id="333ab-118">Replace timeOff</span></span>](../api/timeoff-put.md) | [<span data-ttu-id="333ab-119">timeoff</span><span class="sxs-lookup"><span data-stu-id="333ab-119">timeOff</span></span>](timeOff.md) | <span data-ttu-id="333ab-120">`timeOff` を置き換えます。</span><span class="sxs-lookup"><span data-stu-id="333ab-120">Replace a `timeOff`.</span></span>|
|[<span data-ttu-id="333ab-121">timeoff の削除</span><span class="sxs-lookup"><span data-stu-id="333ab-121">Delete timeOff</span></span>](../api/timeoff-delete.md) | <span data-ttu-id="333ab-122">なし</span><span class="sxs-lookup"><span data-stu-id="333ab-122">None</span></span> | <span data-ttu-id="333ab-123">スケジュールから`timeOff`を削除します。</span><span class="sxs-lookup"><span data-stu-id="333ab-123">Delete a `timeOff` from the schedule.</span></span>|

## <a name="properties"></a><span data-ttu-id="333ab-124">プロパティ</span><span class="sxs-lookup"><span data-stu-id="333ab-124">Properties</span></span>
|<span data-ttu-id="333ab-125">名前</span><span class="sxs-lookup"><span data-stu-id="333ab-125">Name</span></span>          |<span data-ttu-id="333ab-126">型</span><span class="sxs-lookup"><span data-stu-id="333ab-126">Type</span></span>           |<span data-ttu-id="333ab-127">説明</span><span class="sxs-lookup"><span data-stu-id="333ab-127">Description</span></span>                                                                                                                                      |
|--------------|---------------|-------------------------------------------------------------------------------------------------------------------------------------------------|
| <span data-ttu-id="333ab-128">id</span><span class="sxs-lookup"><span data-stu-id="333ab-128">id</span></span>            |`string`      |<span data-ttu-id="333ab-129">`timeOff` の ID。</span><span class="sxs-lookup"><span data-stu-id="333ab-129">ID of the `timeOff`.</span></span>|
| <span data-ttu-id="333ab-130">userId</span><span class="sxs-lookup"><span data-stu-id="333ab-130">userId</span></span>            |`string`      |<span data-ttu-id="333ab-131">に割り当てられているユーザー `timeOff`の ID。</span><span class="sxs-lookup"><span data-stu-id="333ab-131">ID of the user assigned to the `timeOff`.</span></span> <span data-ttu-id="333ab-132">必須です。</span><span class="sxs-lookup"><span data-stu-id="333ab-132">Required.</span></span>|
| <span data-ttu-id="333ab-133">sharedtimeoff</span><span class="sxs-lookup"><span data-stu-id="333ab-133">sharedTimeOff</span></span>     | [<span data-ttu-id="333ab-134">timeoffitem</span><span class="sxs-lookup"><span data-stu-id="333ab-134">timeOffItem</span></span>](timeoffitem.md)  |<span data-ttu-id="333ab-135">従業員とマネージャーの両方`timeOff`に表示される共有バージョン。</span><span class="sxs-lookup"><span data-stu-id="333ab-135">The shared version of this `timeOff` that is viewable by both employees and managers.</span></span> <span data-ttu-id="333ab-136">必須です。</span><span class="sxs-lookup"><span data-stu-id="333ab-136">Required.</span></span>|
| <span data-ttu-id="333ab-137">draftTimeOff</span><span class="sxs-lookup"><span data-stu-id="333ab-137">draftTimeOff</span></span>      | [<span data-ttu-id="333ab-138">timeoffitem</span><span class="sxs-lookup"><span data-stu-id="333ab-138">timeOffItem</span></span>](timeoffitem.md)        |<span data-ttu-id="333ab-139">この`timeOff`の下書きバージョンは、マネージャーが表示できます。</span><span class="sxs-lookup"><span data-stu-id="333ab-139">The draft version of this `timeOff` that is viewable by managers.</span></span> <span data-ttu-id="333ab-140">必須。</span><span class="sxs-lookup"><span data-stu-id="333ab-140">Required.</span></span>|
| <span data-ttu-id="333ab-141">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="333ab-141">createdDateTime</span></span>       |`DateTimeOffset`        |<span data-ttu-id="333ab-142">これ`timeOff`が最初に作成されたタイムスタンプ。</span><span class="sxs-lookup"><span data-stu-id="333ab-142">The time stamp at which this `timeOff` was first created.</span></span> <span data-ttu-id="333ab-143">Timestamp 型は、ISO 8601 形式を使用して日付と時刻の情報を表します。これは常に UTC 時間です。</span><span class="sxs-lookup"><span data-stu-id="333ab-143">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="333ab-144">たとえば、2014 年 1 月 1 日午前 0 時 (UTC) は、'2014-01-01T00:00:00Z'.のようになります。</span><span class="sxs-lookup"><span data-stu-id="333ab-144">For example, midnight UTC on Jan 1, 2014 would look like this: '2014-01-01T00:00:00Z'.</span></span> |
| <span data-ttu-id="333ab-145">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="333ab-145">lastModifiedDateTime</span></span>      |`DateTimeOffset`        |<span data-ttu-id="333ab-146">これ`timeOff`が最後に更新されたタイムスタンプ。</span><span class="sxs-lookup"><span data-stu-id="333ab-146">The time stamp at which this `timeOff` was last updated.</span></span> <span data-ttu-id="333ab-147">Timestamp 型は、ISO 8601 形式を使用して日付と時刻の情報を表します。これは常に UTC 時間です。</span><span class="sxs-lookup"><span data-stu-id="333ab-147">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="333ab-148">たとえば、2014 年 1 月 1 日午前 0 時 (UTC) は、'2014-01-01T00:00:00Z'.のようになります。</span><span class="sxs-lookup"><span data-stu-id="333ab-148">For example, midnight UTC on Jan 1, 2014 would look like this: '2014-01-01T00:00:00Z'.</span></span> |
| <span data-ttu-id="333ab-149">lastModifiedBy</span><span class="sxs-lookup"><span data-stu-id="333ab-149">lastModifiedBy</span></span>        | [<span data-ttu-id="333ab-150">identitySet</span><span class="sxs-lookup"><span data-stu-id="333ab-150">identitySet</span></span>](identityset.md)        |<span data-ttu-id="333ab-151">この `timeOff` を最後に更新した ID。</span><span class="sxs-lookup"><span data-stu-id="333ab-151">The identity that last updated this `timeOff`.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="333ab-152">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="333ab-152">JSON representation</span></span>

<span data-ttu-id="333ab-153">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="333ab-153">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.timeOff",
   "baseType":"microsoft.graph.changeTrackedEntity"
}-->

```json
{
  "userId": "string (identifier)",
  "createdDateTime": "String (timestamp)",
  "lastModifiedDateTime": "String (timestamp)",
  "lastModifiedBy": {"@odata.type":"microsoft.graph.identitySet"},
  "sharedTimeOff": {"@odata.type":"microsoft.graph.timeOffItem"},
  "draftTimeOff": {"@odata.type":"microsoft.graph.timeOffItem"}
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
  "suppressions": []
}
-->
