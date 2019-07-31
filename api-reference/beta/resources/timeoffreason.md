---
title: timeOffReason リソースの種類
description: スケジュールでタイムアウトになる有効な理由。
author: nkramer
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: resourcePageType_
ms.openlocfilehash: 62943670a0c87d34fd849e988ef5bf827aa6d72a
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "35964288"
---
# <a name="timeoffreason-resource-type"></a><span data-ttu-id="c83a5-103">timeOffReason リソースの種類</span><span class="sxs-lookup"><span data-stu-id="c83a5-103">timeOffReason resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="c83a5-104">[スケジュール](schedule.md)内の[timeoff](timeoff.md)インスタンスの有効な理由。</span><span class="sxs-lookup"><span data-stu-id="c83a5-104">A valid reason to for a [timeOff](timeoff.md) instance in a [schedule](schedule.md).</span></span>

## <a name="methods"></a><span data-ttu-id="c83a5-105">メソッド</span><span class="sxs-lookup"><span data-stu-id="c83a5-105">Methods</span></span>

| <span data-ttu-id="c83a5-106">メソッド</span><span class="sxs-lookup"><span data-stu-id="c83a5-106">Method</span></span>       | <span data-ttu-id="c83a5-107">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="c83a5-107">Return Type</span></span>  |<span data-ttu-id="c83a5-108">説明</span><span class="sxs-lookup"><span data-stu-id="c83a5-108">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="c83a5-109">TimeOffReason の作成</span><span class="sxs-lookup"><span data-stu-id="c83a5-109">Create timeOffReason</span></span>](../api/schedule-post-timeoffreasons.md) | [<span data-ttu-id="c83a5-110">timeOffReason</span><span class="sxs-lookup"><span data-stu-id="c83a5-110">timeOffReason</span></span>](timeoffreason.md) | <span data-ttu-id="c83a5-111">新しい `timeOffReason` を作成します。</span><span class="sxs-lookup"><span data-stu-id="c83a5-111">Create a new `timeOffReason`.</span></span>|
|[<span data-ttu-id="c83a5-112">リスト timeOffReason</span><span class="sxs-lookup"><span data-stu-id="c83a5-112">List timeOffReason</span></span>](../api/schedule-list-timeoffreasons.md) | <span data-ttu-id="c83a5-113">[Timeoffreason](timeoffreason.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="c83a5-113">[timeOffReason](timeoffreason.md) collection</span></span> | <span data-ttu-id="c83a5-114">スケジュール内の `timeOffReasons` のリストを取得します。</span><span class="sxs-lookup"><span data-stu-id="c83a5-114">Get the list of `timeOffReasons` in a schedule.</span></span>|
|[<span data-ttu-id="c83a5-115">TimeOffReason を取得する</span><span class="sxs-lookup"><span data-stu-id="c83a5-115">Get timeOffReason</span></span>](../api/timeoffreason-get.md) | [<span data-ttu-id="c83a5-116">timeOffReason</span><span class="sxs-lookup"><span data-stu-id="c83a5-116">timeOffReason</span></span>](timeoffreason.md) | <span data-ttu-id="c83a5-117">ID で `timeOffReason` を取得します。</span><span class="sxs-lookup"><span data-stu-id="c83a5-117">Get a `timeOffReason` by ID.</span></span>|
|[<span data-ttu-id="c83a5-118">TimeOffReason を置換する</span><span class="sxs-lookup"><span data-stu-id="c83a5-118">Replace timeOffReason</span></span>](../api/timeoffreason-put.md) | [<span data-ttu-id="c83a5-119">timeOffReason</span><span class="sxs-lookup"><span data-stu-id="c83a5-119">timeOffReason</span></span>](timeoffreason.md) | <span data-ttu-id="c83a5-120">`timeOffReason` を置き換えます。</span><span class="sxs-lookup"><span data-stu-id="c83a5-120">Replace a `timeOffReason`.</span></span>|
|[<span data-ttu-id="c83a5-121">TimeOffReason の削除</span><span class="sxs-lookup"><span data-stu-id="c83a5-121">Delete timeOffReason</span></span>](../api/timeoffreason-delete.md) | <span data-ttu-id="c83a5-122">なし</span><span class="sxs-lookup"><span data-stu-id="c83a5-122">None</span></span> | <span data-ttu-id="c83a5-123">`timeOffReason` を非アクティブとしてマークします。</span><span class="sxs-lookup"><span data-stu-id="c83a5-123">Mark `timeOffReason` as inactive.</span></span>|

## <a name="properties"></a><span data-ttu-id="c83a5-124">プロパティ</span><span class="sxs-lookup"><span data-stu-id="c83a5-124">Properties</span></span>
|<span data-ttu-id="c83a5-125">名前</span><span class="sxs-lookup"><span data-stu-id="c83a5-125">Name</span></span>          |<span data-ttu-id="c83a5-126">型</span><span class="sxs-lookup"><span data-stu-id="c83a5-126">Type</span></span>           |<span data-ttu-id="c83a5-127">説明</span><span class="sxs-lookup"><span data-stu-id="c83a5-127">Description</span></span>                                                                                 |
|--------------|---------------|--------------------------------------------------------------------------------------------|
| <span data-ttu-id="c83a5-128">id</span><span class="sxs-lookup"><span data-stu-id="c83a5-128">id</span></span>            |`string`      |<span data-ttu-id="c83a5-129">`timeOffReason` の ID。</span><span class="sxs-lookup"><span data-stu-id="c83a5-129">ID of the `timeOffReason`.</span></span>|
| <span data-ttu-id="c83a5-130">displayName</span><span class="sxs-lookup"><span data-stu-id="c83a5-130">displayName</span></span>               | `string`                  | <span data-ttu-id="c83a5-131">の名前`timeOffReason`。</span><span class="sxs-lookup"><span data-stu-id="c83a5-131">The name of the `timeOffReason`.</span></span> <span data-ttu-id="c83a5-132">必須です。</span><span class="sxs-lookup"><span data-stu-id="c83a5-132">Required.</span></span> |
| <span data-ttu-id="c83a5-133">iconType</span><span class="sxs-lookup"><span data-stu-id="c83a5-133">iconType</span></span> | `timeOffReasonIconType`   | <span data-ttu-id="c83a5-134">サポートされているアイコンの種類: なし、故障]起動平面ファイヤな Id;診察notWorking;レコーダーjuryDuty;世界中カップ代わり天気予報付piggyBank;エサケーキtrafficCone;pin晴れ.</span><span class="sxs-lookup"><span data-stu-id="c83a5-134">Supported icon types: none; car; calendar; running; plane; firstAid; doctor; notWorking; clock; juryDuty; globe; cup; phone; weather; umbrella; piggyBank; dog; cake; trafficCone; pin; sunny.</span></span> <span data-ttu-id="c83a5-135">必須です。</span><span class="sxs-lookup"><span data-stu-id="c83a5-135">Required.</span></span> |
| <span data-ttu-id="c83a5-136">isActive</span><span class="sxs-lookup"><span data-stu-id="c83a5-136">isActive</span></span>          |`Boolean`      | <span data-ttu-id="c83a5-137">新しくエンティティを作成する場合や、既存のエンティティを更新する場合に `timeOffReason` を使用できるかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="c83a5-137">Indicates whether the `timeOffReason` can be used when creating new entities or updating existing ones.</span></span> <span data-ttu-id="c83a5-138">必須。</span><span class="sxs-lookup"><span data-stu-id="c83a5-138">Required.</span></span> |
| <span data-ttu-id="c83a5-139">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="c83a5-139">createdDateTime</span></span>       |`DateTimeOffset`        |<span data-ttu-id="c83a5-140">これ`timeOffReason`が最初に作成されたタイムスタンプ。</span><span class="sxs-lookup"><span data-stu-id="c83a5-140">The time stamp on which this `timeOffReason` was first created.</span></span> <span data-ttu-id="c83a5-141">Timestamp 型は、ISO 8601 形式を使用して日付と時刻の情報を表します。これは常に UTC 時間です。</span><span class="sxs-lookup"><span data-stu-id="c83a5-141">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="c83a5-142">たとえば、2014 年 1 月 1 日午前 0 時 (UTC) は、'2014-01-01T00:00:00Z'.のようになります。</span><span class="sxs-lookup"><span data-stu-id="c83a5-142">For example, midnight UTC on Jan 1, 2014 would look like this: '2014-01-01T00:00:00Z'.</span></span> |
| <span data-ttu-id="c83a5-143">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="c83a5-143">lastModifiedDateTime</span></span>      |`DateTimeOffset`         |<span data-ttu-id="c83a5-144">これ`timeOffReason`が最後に更新されたタイムスタンプ。</span><span class="sxs-lookup"><span data-stu-id="c83a5-144">The time stamp on which this `timeOffReason` was last updated.</span></span> <span data-ttu-id="c83a5-145">Timestamp 型は、ISO 8601 形式を使用して日付と時刻の情報を表します。これは常に UTC 時間です。</span><span class="sxs-lookup"><span data-stu-id="c83a5-145">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="c83a5-146">たとえば、2014 年 1 月 1 日午前 0 時 (UTC) は、'2014-01-01T00:00:00Z'.のようになります。</span><span class="sxs-lookup"><span data-stu-id="c83a5-146">For example, midnight UTC on Jan 1, 2014 would look like this: '2014-01-01T00:00:00Z'.</span></span> |
| <span data-ttu-id="c83a5-147">lastModifiedBy</span><span class="sxs-lookup"><span data-stu-id="c83a5-147">lastModifiedBy</span></span>        | [<span data-ttu-id="c83a5-148">identitySet</span><span class="sxs-lookup"><span data-stu-id="c83a5-148">identitySet</span></span>](identityset.md)        |<span data-ttu-id="c83a5-149">この `timeOffReason` を最後に更新した ID。</span><span class="sxs-lookup"><span data-stu-id="c83a5-149">The identity that last updated this `timeOffReason`.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="c83a5-150">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="c83a5-150">JSON representation</span></span>

<span data-ttu-id="c83a5-151">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="c83a5-151">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.timeOffReason",
  "baseType":"microsoft.graph.changeTrackedEntity"
}-->

```json
{
  "id": "String",
  "createdDateTime": "String (timestamp)",
  "lastModifiedDateTime": "String (timestamp)",
  "displayName": "String",
  "iconType": "String",
  "isActive": true,
  "lastModifiedBy": { "@odata.type":"microsoft.graph.identitySet"}
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
  "suppressions": []
}
-->
