---
title: timeoffreason リソースの種類
description: スケジュールでタイムアウトになる有効な理由。
author: nkramer
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: 72597fa1678110a40b9dd1a0ea6e6235625144ab
ms.sourcegitcommit: 081cacecb4960aabc9e1011d12f06fe9ecf7d188
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 03/16/2019
ms.locfileid: "30657533"
---
# <a name="timeoffreason-resource-type"></a><span data-ttu-id="b8da7-103">timeoffreason リソースの種類</span><span class="sxs-lookup"><span data-stu-id="b8da7-103">timeOffReason resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="b8da7-104">[スケジュール](schedule.md)内の[timeoff](timeoff.md)インスタンスの有効な理由。</span><span class="sxs-lookup"><span data-stu-id="b8da7-104">A valid reason to for a [timeOff](timeoff.md) instance in a [schedule](schedule.md).</span></span>

## <a name="methods"></a><span data-ttu-id="b8da7-105">メソッド</span><span class="sxs-lookup"><span data-stu-id="b8da7-105">Methods</span></span>

| <span data-ttu-id="b8da7-106">メソッド</span><span class="sxs-lookup"><span data-stu-id="b8da7-106">Method</span></span>       | <span data-ttu-id="b8da7-107">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="b8da7-107">Return Type</span></span>  |<span data-ttu-id="b8da7-108">説明</span><span class="sxs-lookup"><span data-stu-id="b8da7-108">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="b8da7-109">timeoffreason の作成</span><span class="sxs-lookup"><span data-stu-id="b8da7-109">Create timeOffReason</span></span>](../api/schedule-post-timeoffreasons.md) | [<span data-ttu-id="b8da7-110">timeoffreason</span><span class="sxs-lookup"><span data-stu-id="b8da7-110">timeOffReason</span></span>](timeoffreason.md) | <span data-ttu-id="b8da7-111">新しい`timeOffReason`を作成します。</span><span class="sxs-lookup"><span data-stu-id="b8da7-111">Create a new `timeOffReason`.</span></span>|
|[<span data-ttu-id="b8da7-112">リスト timeoffreason</span><span class="sxs-lookup"><span data-stu-id="b8da7-112">List timeOffReason</span></span>](../api/schedule-list-timeoffreasons.md) | <span data-ttu-id="b8da7-113">[timeoffreason](timeoffreason.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="b8da7-113">[timeOffReason](timeoffreason.md) collection</span></span> | <span data-ttu-id="b8da7-114">スケジュールに含まれる`timeOffReasons`のリストを取得します。</span><span class="sxs-lookup"><span data-stu-id="b8da7-114">Get the list of `timeOffReasons` in a schedule.</span></span>|
|[<span data-ttu-id="b8da7-115">timeoffreason を取得する</span><span class="sxs-lookup"><span data-stu-id="b8da7-115">Get timeOffReason</span></span>](../api/timeoffreason-get.md) | [<span data-ttu-id="b8da7-116">timeoffreason</span><span class="sxs-lookup"><span data-stu-id="b8da7-116">timeOffReason</span></span>](timeoffreason.md) | <span data-ttu-id="b8da7-117">ID `timeOffReason`で取得します。</span><span class="sxs-lookup"><span data-stu-id="b8da7-117">Get a `timeOffReason` by ID.</span></span>|
|[<span data-ttu-id="b8da7-118">timeoffreason を置換する</span><span class="sxs-lookup"><span data-stu-id="b8da7-118">Replace timeOffReason</span></span>](../api/timeoffreason-put.md) | [<span data-ttu-id="b8da7-119">timeoffreason</span><span class="sxs-lookup"><span data-stu-id="b8da7-119">timeOffReason</span></span>](timeoffreason.md) | <span data-ttu-id="b8da7-120">を`timeOffReason`置き換えます。</span><span class="sxs-lookup"><span data-stu-id="b8da7-120">Replace a `timeOffReason`.</span></span>|
|[<span data-ttu-id="b8da7-121">timeoffreason の削除</span><span class="sxs-lookup"><span data-stu-id="b8da7-121">Delete timeOffReason</span></span>](../api/timeoffreason-delete.md) | <span data-ttu-id="b8da7-122">なし</span><span class="sxs-lookup"><span data-stu-id="b8da7-122">None</span></span> | <span data-ttu-id="b8da7-123">非`timeOffReason`アクティブとしてマークします。</span><span class="sxs-lookup"><span data-stu-id="b8da7-123">Mark `timeOffReason` as inactive.</span></span>|

## <a name="properties"></a><span data-ttu-id="b8da7-124">プロパティ</span><span class="sxs-lookup"><span data-stu-id="b8da7-124">Properties</span></span>
|<span data-ttu-id="b8da7-125">名前</span><span class="sxs-lookup"><span data-stu-id="b8da7-125">Name</span></span>          |<span data-ttu-id="b8da7-126">型</span><span class="sxs-lookup"><span data-stu-id="b8da7-126">Type</span></span>           |<span data-ttu-id="b8da7-127">説明</span><span class="sxs-lookup"><span data-stu-id="b8da7-127">Description</span></span>                                                                                 |
|--------------|---------------|--------------------------------------------------------------------------------------------|
| <span data-ttu-id="b8da7-128">id</span><span class="sxs-lookup"><span data-stu-id="b8da7-128">id</span></span>            |`string`      |<span data-ttu-id="b8da7-129">の ID `timeOffReason`。</span><span class="sxs-lookup"><span data-stu-id="b8da7-129">ID of the `timeOffReason`.</span></span>|
| <span data-ttu-id="b8da7-130">displayName</span><span class="sxs-lookup"><span data-stu-id="b8da7-130">displayName</span></span>               | `string`                  | <span data-ttu-id="b8da7-131">の名前`timeOffReason`。</span><span class="sxs-lookup"><span data-stu-id="b8da7-131">The name of the `timeOffReason`.</span></span> <span data-ttu-id="b8da7-132">必須。</span><span class="sxs-lookup"><span data-stu-id="b8da7-132">Required.</span></span> |
| <span data-ttu-id="b8da7-133">icontype</span><span class="sxs-lookup"><span data-stu-id="b8da7-133">iconType</span></span> | `enum`   | <span data-ttu-id="b8da7-134">サポートされているアイコンの種類: なし、故障]起動平面ファイヤな id;診察notworking;レコーダーjuryDuty;世界中カップ代わり天気予報付piggyBank;エサケーキtrafficCone;pin晴れ.</span><span class="sxs-lookup"><span data-stu-id="b8da7-134">Supported icon types: none; car; calendar; running; plane; firstAid; doctor; notWorking; clock; juryDuty; globe; cup; phone; weather; umbrella; piggyBank; dog; cake; trafficCone; pin; sunny.</span></span> <span data-ttu-id="b8da7-135">必須。</span><span class="sxs-lookup"><span data-stu-id="b8da7-135">Required.</span></span> |
| <span data-ttu-id="b8da7-136">isActive</span><span class="sxs-lookup"><span data-stu-id="b8da7-136">isActive</span></span>          |`bool`      | <span data-ttu-id="b8da7-137">新しいエンティティを`timeOffReason`作成するとき、または既存のエンティティを更新するときに、を使用できるかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="b8da7-137">Indicates whether the `timeOffReason` can be used when creating new entities or updating existing ones.</span></span> <span data-ttu-id="b8da7-138">必須。</span><span class="sxs-lookup"><span data-stu-id="b8da7-138">Required.</span></span> |
| <span data-ttu-id="b8da7-139">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="b8da7-139">createdDateTime</span></span>       |`DateTimeOffset`        |<span data-ttu-id="b8da7-140">これ`timeOffReason`が最初に作成されたタイムスタンプ。</span><span class="sxs-lookup"><span data-stu-id="b8da7-140">The time stamp on which this `timeOffReason` was first created.</span></span> <span data-ttu-id="b8da7-141">Timestamp 型は、ISO 8601 形式を使用して日付と時刻の情報を表し、必ず UTC 時間です。</span><span class="sxs-lookup"><span data-stu-id="b8da7-141">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="b8da7-142">たとえば、2014年1月1日午前0時 (UTC) は次のようになります。 ' 2014-01-01t00:00: 00z ' のようになります。</span><span class="sxs-lookup"><span data-stu-id="b8da7-142">For example, midnight UTC on Jan 1, 2014 would look like this: '2014-01-01T00:00:00Z'.</span></span> |
| <span data-ttu-id="b8da7-143">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="b8da7-143">lastModifiedDateTime</span></span>      |`DateTimeOffset`         |<span data-ttu-id="b8da7-144">これ`timeOffReason`が最後に更新されたタイムスタンプ。</span><span class="sxs-lookup"><span data-stu-id="b8da7-144">The time stamp on which this `timeOffReason` was last updated.</span></span> <span data-ttu-id="b8da7-145">Timestamp 型は、ISO 8601 形式を使用して日付と時刻の情報を表し、必ず UTC 時間です。</span><span class="sxs-lookup"><span data-stu-id="b8da7-145">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="b8da7-146">たとえば、2014年1月1日午前0時 (UTC) は次のようになります。 ' 2014-01-01t00:00: 00z ' のようになります。</span><span class="sxs-lookup"><span data-stu-id="b8da7-146">For example, midnight UTC on Jan 1, 2014 would look like this: '2014-01-01T00:00:00Z'.</span></span> |
| <span data-ttu-id="b8da7-147">lastModifiedBy</span><span class="sxs-lookup"><span data-stu-id="b8da7-147">lastModifiedBy</span></span>        |`microsoft.graph.identitySet`        |<span data-ttu-id="b8da7-148">最後に更新`timeOffReason`した id。</span><span class="sxs-lookup"><span data-stu-id="b8da7-148">The identity that last updated this `timeOffReason`.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="b8da7-149">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="b8da7-149">JSON representation</span></span>

<span data-ttu-id="b8da7-150">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="b8da7-150">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.timeOffReason"
}-->

```json
{
  "id": "TOR_891045ca-b5d2-406b-aa06-a3c8921245d7",
  "createdDateTime": "2019-03-12T22:10:38.242Z",
  "lastModifiedDateTime": "2019-03-12T22:10:38.242Z",
  "displayName": "Vacation",
  "iconType": "plane",
  "isActive": true,
  "lastModifiedBy": {
    "application": null,
    "device": null,
    "conversation": null,
    "user": {
      "id": "366c0b19-49b1-41b5-a03f-9f3887bd0ed8",
      "displayName": "John Doe"
    }
  }
}
```


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "timeOffReason resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/timeoffreason.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->