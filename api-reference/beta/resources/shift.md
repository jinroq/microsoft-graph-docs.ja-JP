---
title: shift リソースの種類
description: Shift は、スケジュールのスケジュールされた作業の単位です。
author: nkramer
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: resourcePageType_
ms.openlocfilehash: f76cd25a36ba070d9fa8281f31a1520a0d7b4435
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "36008349"
---
# <a name="shift-resource-type"></a><span data-ttu-id="104f8-103">shift リソースの種類</span><span class="sxs-lookup"><span data-stu-id="104f8-103">shift resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="104f8-104">[スケジュール](schedule.md)に含まれるスケジュールされた作業の単位。</span><span class="sxs-lookup"><span data-stu-id="104f8-104">A unit of scheduled work in a [schedule](schedule.md).</span></span> 

## <a name="methods"></a><span data-ttu-id="104f8-105">メソッド</span><span class="sxs-lookup"><span data-stu-id="104f8-105">Methods</span></span>

| <span data-ttu-id="104f8-106">メソッド</span><span class="sxs-lookup"><span data-stu-id="104f8-106">Method</span></span>       | <span data-ttu-id="104f8-107">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="104f8-107">Return Type</span></span>  |<span data-ttu-id="104f8-108">説明</span><span class="sxs-lookup"><span data-stu-id="104f8-108">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="104f8-109">Shift を作成する</span><span class="sxs-lookup"><span data-stu-id="104f8-109">Create shift</span></span>](../api/schedule-post-shifts.md) | [<span data-ttu-id="104f8-110">制</span><span class="sxs-lookup"><span data-stu-id="104f8-110">shift</span></span>](shift.md) | <span data-ttu-id="104f8-111">新しい `shift` を作成します。</span><span class="sxs-lookup"><span data-stu-id="104f8-111">Create a new `shift`.</span></span>|
|[<span data-ttu-id="104f8-112">シフトの一覧表示</span><span class="sxs-lookup"><span data-stu-id="104f8-112">List shifts</span></span>](../api/schedule-list-shifts.md) | <span data-ttu-id="104f8-113">[shift](shift.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="104f8-113">[shift](shift.md) collection</span></span> | <span data-ttu-id="104f8-114">このスケジュール内の`shifts`のリストを取得します。</span><span class="sxs-lookup"><span data-stu-id="104f8-114">Get the list of `shifts` in this schedule.</span></span>|
|[<span data-ttu-id="104f8-115">Shift を取得する</span><span class="sxs-lookup"><span data-stu-id="104f8-115">Get shift</span></span>](../api/shift-get.md) | [<span data-ttu-id="104f8-116">制</span><span class="sxs-lookup"><span data-stu-id="104f8-116">shift</span></span>](shift.md) | <span data-ttu-id="104f8-117">ID で `shift` を取得します。</span><span class="sxs-lookup"><span data-stu-id="104f8-117">Get a `shift` by ID.</span></span>|
|[<span data-ttu-id="104f8-118">Shift を置換する</span><span class="sxs-lookup"><span data-stu-id="104f8-118">Replace shift</span></span>](../api/shift-put.md) | [<span data-ttu-id="104f8-119">制</span><span class="sxs-lookup"><span data-stu-id="104f8-119">shift</span></span>](shift.md) | <span data-ttu-id="104f8-120">`shift` を置き換えます。</span><span class="sxs-lookup"><span data-stu-id="104f8-120">Replace a `shift`.</span></span>|
|[<span data-ttu-id="104f8-121">Shift を削除する</span><span class="sxs-lookup"><span data-stu-id="104f8-121">Delete shift</span></span>](../api/shift-delete.md) | <span data-ttu-id="104f8-122">None</span><span class="sxs-lookup"><span data-stu-id="104f8-122">None</span></span> | <span data-ttu-id="104f8-123">スケジュールから`shift`を削除します。</span><span class="sxs-lookup"><span data-stu-id="104f8-123">Delete a `shift` from the schedule.</span></span>|

## <a name="properties"></a><span data-ttu-id="104f8-124">プロパティ</span><span class="sxs-lookup"><span data-stu-id="104f8-124">Properties</span></span>
|<span data-ttu-id="104f8-125">名前</span><span class="sxs-lookup"><span data-stu-id="104f8-125">Name</span></span>          |<span data-ttu-id="104f8-126">型</span><span class="sxs-lookup"><span data-stu-id="104f8-126">Type</span></span>           |<span data-ttu-id="104f8-127">説明</span><span class="sxs-lookup"><span data-stu-id="104f8-127">Description</span></span>                                                                                                                                      |
|--------------|---------------|-------------------------------------------------------------------------------------------------------------------------------------------------|
| <span data-ttu-id="104f8-128">id</span><span class="sxs-lookup"><span data-stu-id="104f8-128">id</span></span>            |`string`      |<span data-ttu-id="104f8-129">`shift` の ID。</span><span class="sxs-lookup"><span data-stu-id="104f8-129">ID of the `shift`.</span></span>|
| <span data-ttu-id="104f8-130">userId</span><span class="sxs-lookup"><span data-stu-id="104f8-130">userId</span></span>            |`string`      |<span data-ttu-id="104f8-131">に割り当てられているユーザー `shift`の ID。</span><span class="sxs-lookup"><span data-stu-id="104f8-131">ID of the user assigned to the `shift`.</span></span> <span data-ttu-id="104f8-132">必須です。</span><span class="sxs-lookup"><span data-stu-id="104f8-132">Required.</span></span> |
| <span data-ttu-id="104f8-133">schedulingGroupId</span><span class="sxs-lookup"><span data-stu-id="104f8-133">schedulingGroupId</span></span>         |`string`      |<span data-ttu-id="104f8-134">`shift`が含まれるスケジュールグループの ID。</span><span class="sxs-lookup"><span data-stu-id="104f8-134">ID of the scheduling group the `shift` is part of.</span></span> <span data-ttu-id="104f8-135">必須です。</span><span class="sxs-lookup"><span data-stu-id="104f8-135">Required.</span></span> |
| <span data-ttu-id="104f8-136">sharedShift</span><span class="sxs-lookup"><span data-stu-id="104f8-136">sharedShift</span></span>   |[<span data-ttu-id="104f8-137">佐々木</span><span class="sxs-lookup"><span data-stu-id="104f8-137">shiftItem</span></span>](shiftitem.md)  |<span data-ttu-id="104f8-138">従業員とマネージャーの両方`shift`に表示される共有バージョン。</span><span class="sxs-lookup"><span data-stu-id="104f8-138">The shared version of this `shift` that is viewable by both employees and managers.</span></span> <span data-ttu-id="104f8-139">必須です。</span><span class="sxs-lookup"><span data-stu-id="104f8-139">Required.</span></span> |
| <span data-ttu-id="104f8-140">draftShift</span><span class="sxs-lookup"><span data-stu-id="104f8-140">draftShift</span></span>        |[<span data-ttu-id="104f8-141">佐々木</span><span class="sxs-lookup"><span data-stu-id="104f8-141">shiftItem</span></span>](shiftitem.md)        |<span data-ttu-id="104f8-142">この`shift`の下書きバージョンは、マネージャーが表示できます。</span><span class="sxs-lookup"><span data-stu-id="104f8-142">The draft version of this `shift` that is viewable by managers.</span></span> <span data-ttu-id="104f8-143">必須。</span><span class="sxs-lookup"><span data-stu-id="104f8-143">Required.</span></span> |
| <span data-ttu-id="104f8-144">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="104f8-144">createdDateTime</span></span>       |`DateTimeOffset`        |<span data-ttu-id="104f8-145">最初に作成さ`shift`れたタイムスタンプ。</span><span class="sxs-lookup"><span data-stu-id="104f8-145">The timestamp on which this `shift` was first created.</span></span> <span data-ttu-id="104f8-146">Timestamp 型は、ISO 8601 形式を使用して日付と時刻の情報を表します。これは常に UTC 時間です。</span><span class="sxs-lookup"><span data-stu-id="104f8-146">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="104f8-147">たとえば、2014 年 1 月 1 日午前 0 時 (UTC) は、'2014-01-01T00:00:00Z'.のようになります。</span><span class="sxs-lookup"><span data-stu-id="104f8-147">For example, midnight UTC on Jan 1, 2014 would look like this: '2014-01-01T00:00:00Z'.</span></span> |
| <span data-ttu-id="104f8-148">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="104f8-148">lastModifiedDateTime</span></span>      |`DateTimeOffset`        |<span data-ttu-id="104f8-149">最後に更新され`shift`たタイムスタンプ。</span><span class="sxs-lookup"><span data-stu-id="104f8-149">The timestamp on which this `shift` was last updated.</span></span> <span data-ttu-id="104f8-150">Timestamp 型は、ISO 8601 形式を使用して日付と時刻の情報を表します。これは常に UTC 時間です。</span><span class="sxs-lookup"><span data-stu-id="104f8-150">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="104f8-151">たとえば、2014 年 1 月 1 日午前 0 時 (UTC) は、'2014-01-01T00:00:00Z'.のようになります。</span><span class="sxs-lookup"><span data-stu-id="104f8-151">For example, midnight UTC on Jan 1, 2014 would look like this: '2014-01-01T00:00:00Z'.</span></span> |
| <span data-ttu-id="104f8-152">lastModifiedBy</span><span class="sxs-lookup"><span data-stu-id="104f8-152">lastModifiedBy</span></span>        | [<span data-ttu-id="104f8-153">identitySet</span><span class="sxs-lookup"><span data-stu-id="104f8-153">identitySet</span></span>](identityset.md)        |<span data-ttu-id="104f8-154">この `shift` を最後に更新した ID。</span><span class="sxs-lookup"><span data-stu-id="104f8-154">The identity that last updated this `shift`.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="104f8-155">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="104f8-155">JSON representation</span></span>

<span data-ttu-id="104f8-156">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="104f8-156">Here is a JSON representation of the resource.</span></span>

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
  "lastModifiedBy": {"@odata.type":"microsoft.graph.identitySet"},
  "sharedShift": {"@odata.type":"microsoft.graph.shiftItem"},
  "draftShift": {"@odata.type":"microsoft.graph.shiftItem"}
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
  "suppressions": []
}
-->
