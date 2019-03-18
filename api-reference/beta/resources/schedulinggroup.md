---
title: schedulingGroup リソースの種類
description: スケジュール内のメンバーの論理グループ (通常は役割による)。
author: nkramer
localization_priority: Priority
ms.prod: microsoft-teams
ms.openlocfilehash: 644a9492e47979241ccab3f0e69eb90407eb2647
ms.sourcegitcommit: 081cacecb4960aabc9e1011d12f06fe9ecf7d188
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 03/16/2019
ms.locfileid: "30657869"
---
# <a name="schedulinggroup-resource-type"></a><span data-ttu-id="2cb64-103">schedulingGroup リソースの種類</span><span class="sxs-lookup"><span data-stu-id="2cb64-103">schedulingGroup resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="2cb64-104">[スケジュール](schedule.md)内のメンバーの論理グループ (通常は役割による)。</span><span class="sxs-lookup"><span data-stu-id="2cb64-104">A logical grouping of users in a [schedule](schedule.md) (usually by role).</span></span> 

## <a name="methods"></a><span data-ttu-id="2cb64-105">メソッド</span><span class="sxs-lookup"><span data-stu-id="2cb64-105">Methods</span></span>

| <span data-ttu-id="2cb64-106">メソッド</span><span class="sxs-lookup"><span data-stu-id="2cb64-106">Method</span></span>       | <span data-ttu-id="2cb64-107">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="2cb64-107">Return Type</span></span>  |<span data-ttu-id="2cb64-108">Description</span><span class="sxs-lookup"><span data-stu-id="2cb64-108">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="2cb64-109">schedulingGroup を作成する</span><span class="sxs-lookup"><span data-stu-id="2cb64-109">Create schedulingGroup</span></span>](../api/schedule-post-schedulinggroups.md) | [<span data-ttu-id="2cb64-110">schedulingGroup</span><span class="sxs-lookup"><span data-stu-id="2cb64-110">schedulingGroup</span></span>](schedulinggroup.md) | <span data-ttu-id="2cb64-111">新しい `schedulingGroup` を作成します。</span><span class="sxs-lookup"><span data-stu-id="2cb64-111">`schedulingGroup`</span></span>|
|[<span data-ttu-id="2cb64-112">List schedulingGroups</span><span class="sxs-lookup"><span data-stu-id="2cb64-112">List schedulingGroups</span></span>](../api/schedule-list-schedulinggroups.md) | <span data-ttu-id="2cb64-113">[schedulingGroup](schedulinggroup.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="2cb64-113">[schedulingGroup](schedulinggroup.md) collection</span></span> | <span data-ttu-id="2cb64-114">スケジュール内の `schedulingGroups` のリストを取得します。</span><span class="sxs-lookup"><span data-stu-id="2cb64-114">Get the list of all root messages in a channel.</span></span>|
|[<span data-ttu-id="2cb64-115">Get schedulingGroup</span><span class="sxs-lookup"><span data-stu-id="2cb64-115">Get schedulingGroup</span></span>](../api/schedulinggroup-get.md) | [<span data-ttu-id="2cb64-116">schedulingGroup</span><span class="sxs-lookup"><span data-stu-id="2cb64-116">schedulingGroup</span></span>](schedulinggroup.md) | <span data-ttu-id="2cb64-117">ID で `schedulingGroup` を取得します。</span><span class="sxs-lookup"><span data-stu-id="2cb64-117">Get a drive by ID</span></span>|
|[<span data-ttu-id="2cb64-118">Replace schedulingGroup</span><span class="sxs-lookup"><span data-stu-id="2cb64-118">Replace schedulingGroup</span></span>](../api/schedulinggroup-put.md) | [<span data-ttu-id="2cb64-119">schedulingGroup</span><span class="sxs-lookup"><span data-stu-id="2cb64-119">schedulingGroup</span></span>](schedulinggroup.md) | <span data-ttu-id="2cb64-120">`schedulingGroup` を置き換えます。</span><span class="sxs-lookup"><span data-stu-id="2cb64-120">Replace a `schedulingGroup`.</span></span>|
|[<span data-ttu-id="2cb64-121">Delete schedulingGroup</span><span class="sxs-lookup"><span data-stu-id="2cb64-121">Delete schedulingGroup</span></span>](../api/schedulinggroup-delete.md) | <span data-ttu-id="2cb64-122">なし</span><span class="sxs-lookup"><span data-stu-id="2cb64-122">None</span></span> | <span data-ttu-id="2cb64-123">`schedulingGroup` を非アクティブとしてマークします。</span><span class="sxs-lookup"><span data-stu-id="2cb64-123">Mark an Account as inactive</span></span>|

## <a name="properties"></a><span data-ttu-id="2cb64-124">プロパティ</span><span class="sxs-lookup"><span data-stu-id="2cb64-124">Properties</span></span>
|<span data-ttu-id="2cb64-125">名前</span><span class="sxs-lookup"><span data-stu-id="2cb64-125">Name</span></span>          |<span data-ttu-id="2cb64-126">型</span><span class="sxs-lookup"><span data-stu-id="2cb64-126">Type</span></span>           |<span data-ttu-id="2cb64-127">説明</span><span class="sxs-lookup"><span data-stu-id="2cb64-127">Description</span></span>                                                                                 |
|--------------|---------------|--------------------------------------------------------------------------------------------|
| <span data-ttu-id="2cb64-128">id</span><span class="sxs-lookup"><span data-stu-id="2cb64-128">id</span></span>            | `string`      |<span data-ttu-id="2cb64-129">`schedulingGroup` の ID。</span><span class="sxs-lookup"><span data-stu-id="2cb64-129">`schedulingGroup` - ID of the Teacher</span></span>|
| <span data-ttu-id="2cb64-130">displayName</span><span class="sxs-lookup"><span data-stu-id="2cb64-130">displayName</span></span>   | `string`      | <span data-ttu-id="2cb64-131">`schedulingGroup` の表示名。</span><span class="sxs-lookup"><span data-stu-id="2cb64-131">The display name for the `schedulingGroup`.</span></span> <span data-ttu-id="2cb64-132">必須。</span><span class="sxs-lookup"><span data-stu-id="2cb64-132">Required.</span></span> |
| <span data-ttu-id="2cb64-133">isActive</span><span class="sxs-lookup"><span data-stu-id="2cb64-133">isActive</span></span>          |`bool`      | <span data-ttu-id="2cb64-134">新しくエンティティを作成する場合や、既存のエンティティを更新する場合に `schedulingGroup` を使用できるかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="2cb64-134">Indicates whether the `schedulingGroup` can be used when creating new entities or updating existing ones.</span></span> <span data-ttu-id="2cb64-135">必須。</span><span class="sxs-lookup"><span data-stu-id="2cb64-135">Required.</span></span> |
| <span data-ttu-id="2cb64-136">UserIds</span><span class="sxs-lookup"><span data-stu-id="2cb64-136">userIds</span></span>       | `collection(string)`    |  <span data-ttu-id="2cb64-137">`schedulingGroup` のメンバーであるユーザー ID のリスト。</span><span class="sxs-lookup"><span data-stu-id="2cb64-137">The list of user IDs that are a member of the `schedulingGroup`.</span></span> <span data-ttu-id="2cb64-138">必須。</span><span class="sxs-lookup"><span data-stu-id="2cb64-138">Required.</span></span> |
| <span data-ttu-id="2cb64-139">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="2cb64-139">createdDateTime</span></span>       |`DateTimeOffset`        |<span data-ttu-id="2cb64-140">この `schedulingGroup` が最初に作成されたときのタイムスタンプ。</span><span class="sxs-lookup"><span data-stu-id="2cb64-140">The time stamp in which this `schedulingGroup` was first created.</span></span> <span data-ttu-id="2cb64-141">Timestamp 型は、ISO 8601 形式を使用して日付と時刻の情報を表します。これは常に UTC 時間です。</span><span class="sxs-lookup"><span data-stu-id="2cb64-141">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="2cb64-142">たとえば、2014 年 1 月 1 日午前 0 時 (UTC) は、'2014-01-01T00:00:00Z'.のようになります。</span><span class="sxs-lookup"><span data-stu-id="2cb64-142">For example, midnight UTC on Jan 1, 2014 would look like this: '2014-01-01T00:00:00Z'.</span></span> |
| <span data-ttu-id="2cb64-143">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="2cb64-143">lastModifiedDateTime</span></span>      |`DateTimeOffset`        |<span data-ttu-id="2cb64-144">この `schedulingGroup` の最終更新日のタイムスタンプ。</span><span class="sxs-lookup"><span data-stu-id="2cb64-144">The time stamp in which this `schedulingGroup` was last updated.</span></span> <span data-ttu-id="2cb64-145">Timestamp 型は、ISO 8601 形式を使用して日付と時刻の情報を表します。これは常に UTC 時間です。</span><span class="sxs-lookup"><span data-stu-id="2cb64-145">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="2cb64-146">たとえば、2014 年 1 月 1 日午前 0 時 (UTC) は、'2014-01-01T00:00:00Z'.のようになります。</span><span class="sxs-lookup"><span data-stu-id="2cb64-146">For example, midnight UTC on Jan 1, 2014 would look like this: '2014-01-01T00:00:00Z'.</span></span> |
| <span data-ttu-id="2cb64-147">lastModifiedBy</span><span class="sxs-lookup"><span data-stu-id="2cb64-147">lastModifiedBy</span></span>        |`microsoft.graph.identitySet`        |<span data-ttu-id="2cb64-148">この `schedulingGroup` を最後に更新した ID。</span><span class="sxs-lookup"><span data-stu-id="2cb64-148">The identity that last updated this `schedulingGroup`.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="2cb64-149">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="2cb64-149">JSON representation</span></span>

<span data-ttu-id="2cb64-150">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="2cb64-150">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.schedulingGroup"
}-->

```json
{
  "id": "TAG_f914d037-00a3-4ba4-b712-ef178cbea263",
  "createdDateTime": "2019-03-12T22:10:38.242Z",
  "lastModifiedDateTime": "2019-03-12T22:10:38.242Z",
  "displayName": "Cashiers",
  "isActive": true,
  "userIds": [
    "c5d0c76b-80c4-481c-be50-923cd8d680a1",
    "2a4296b3-a28a-44ba-bc66-0274b9b95851"
  ],
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
  "description": "schedulingGroup resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/schedulinggroup.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
