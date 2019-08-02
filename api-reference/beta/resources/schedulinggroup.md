---
title: schedulingGroup リソースの種類
description: スケジュール内のメンバーの論理グループ (通常は役割による)。
author: nkramer
localization_priority: Priority
ms.prod: microsoft-teams
doc_type: resourcePageType_
ms.openlocfilehash: 9f4f494b21a1139ba9a9e0771dcbc41d363bab2b
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "35965300"
---
# <a name="schedulinggroup-resource-type"></a><span data-ttu-id="0f121-103">schedulingGroup リソースの種類</span><span class="sxs-lookup"><span data-stu-id="0f121-103">schedulingGroup resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="0f121-104">[スケジュール](schedule.md)内のメンバーの論理グループ (通常は役割による)。</span><span class="sxs-lookup"><span data-stu-id="0f121-104">A logical grouping of users in a [schedule](schedule.md) (usually by role).</span></span> 

## <a name="methods"></a><span data-ttu-id="0f121-105">メソッド</span><span class="sxs-lookup"><span data-stu-id="0f121-105">Methods</span></span>

| <span data-ttu-id="0f121-106">メソッド</span><span class="sxs-lookup"><span data-stu-id="0f121-106">Method</span></span>       | <span data-ttu-id="0f121-107">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="0f121-107">Return Type</span></span>  |<span data-ttu-id="0f121-108">Description</span><span class="sxs-lookup"><span data-stu-id="0f121-108">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="0f121-109">schedulingGroup を作成する</span><span class="sxs-lookup"><span data-stu-id="0f121-109">Create schedulingGroup</span></span>](../api/schedule-post-schedulinggroups.md) | [<span data-ttu-id="0f121-110">schedulingGroup</span><span class="sxs-lookup"><span data-stu-id="0f121-110">schedulingGroup</span></span>](schedulinggroup.md) | <span data-ttu-id="0f121-111">新しい `schedulingGroup` を作成します。</span><span class="sxs-lookup"><span data-stu-id="0f121-111">Create a new `schedulingGroup`.</span></span>|
|[<span data-ttu-id="0f121-112">List schedulingGroups</span><span class="sxs-lookup"><span data-stu-id="0f121-112">List schedulingGroups</span></span>](../api/schedule-list-schedulinggroups.md) | <span data-ttu-id="0f121-113">[schedulingGroup](schedulinggroup.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="0f121-113">[schedulingGroup](schedulinggroup.md) collection</span></span> | <span data-ttu-id="0f121-114">スケジュール内の `schedulingGroups` のリストを取得します。</span><span class="sxs-lookup"><span data-stu-id="0f121-114">Get the list of `schedulingGroups` in a schedule.</span></span>|
|[<span data-ttu-id="0f121-115">Get schedulingGroup</span><span class="sxs-lookup"><span data-stu-id="0f121-115">Get schedulingGroup</span></span>](../api/schedulinggroup-get.md) | [<span data-ttu-id="0f121-116">schedulingGroup</span><span class="sxs-lookup"><span data-stu-id="0f121-116">schedulingGroup</span></span>](schedulinggroup.md) | <span data-ttu-id="0f121-117">ID で `schedulingGroup` を取得します。</span><span class="sxs-lookup"><span data-stu-id="0f121-117">Get a `schedulingGroup` by ID.</span></span>|
|[<span data-ttu-id="0f121-118">Replace schedulingGroup</span><span class="sxs-lookup"><span data-stu-id="0f121-118">Replace schedulingGroup</span></span>](../api/schedulinggroup-put.md) | [<span data-ttu-id="0f121-119">schedulingGroup</span><span class="sxs-lookup"><span data-stu-id="0f121-119">schedulingGroup</span></span>](schedulinggroup.md) | <span data-ttu-id="0f121-120">`schedulingGroup` を置き換えます。</span><span class="sxs-lookup"><span data-stu-id="0f121-120">Replace a `schedulingGroup`.</span></span>|
|[<span data-ttu-id="0f121-121">Delete schedulingGroup</span><span class="sxs-lookup"><span data-stu-id="0f121-121">Delete schedulingGroup</span></span>](../api/schedulinggroup-delete.md) | <span data-ttu-id="0f121-122">なし</span><span class="sxs-lookup"><span data-stu-id="0f121-122">None</span></span> | <span data-ttu-id="0f121-123">`schedulingGroup` を非アクティブとしてマークします。</span><span class="sxs-lookup"><span data-stu-id="0f121-123">Mark `schedulingGroup` as inactive.</span></span>|

## <a name="properties"></a><span data-ttu-id="0f121-124">プロパティ</span><span class="sxs-lookup"><span data-stu-id="0f121-124">Properties</span></span>
|<span data-ttu-id="0f121-125">名前</span><span class="sxs-lookup"><span data-stu-id="0f121-125">Name</span></span>          |<span data-ttu-id="0f121-126">種類</span><span class="sxs-lookup"><span data-stu-id="0f121-126">Type</span></span>           |<span data-ttu-id="0f121-127">説明</span><span class="sxs-lookup"><span data-stu-id="0f121-127">Description</span></span>                                                                                 |
|--------------|---------------|--------------------------------------------------------------------------------------------|
| <span data-ttu-id="0f121-128">id</span><span class="sxs-lookup"><span data-stu-id="0f121-128">id</span></span>            | `string`      |<span data-ttu-id="0f121-129">`schedulingGroup` の ID。</span><span class="sxs-lookup"><span data-stu-id="0f121-129">ID of the `schedulingGroup`.</span></span>|
| <span data-ttu-id="0f121-130">displayName</span><span class="sxs-lookup"><span data-stu-id="0f121-130">displayName</span></span>   | `string`      | <span data-ttu-id="0f121-131">`schedulingGroup` の表示名。</span><span class="sxs-lookup"><span data-stu-id="0f121-131">The display name for the `schedulingGroup`.</span></span> <span data-ttu-id="0f121-132">必須。</span><span class="sxs-lookup"><span data-stu-id="0f121-132">Required.</span></span> |
| <span data-ttu-id="0f121-133">isActive</span><span class="sxs-lookup"><span data-stu-id="0f121-133">isActive</span></span>          |`bool`      | <span data-ttu-id="0f121-134">新しくエンティティを作成する場合や、既存のエンティティを更新する場合に `schedulingGroup` を使用できるかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="0f121-134">Indicates whether the `schedulingGroup` can be used when creating new entities or updating existing ones.</span></span> <span data-ttu-id="0f121-135">必須。</span><span class="sxs-lookup"><span data-stu-id="0f121-135">Required.</span></span> |
| <span data-ttu-id="0f121-136">UserIds</span><span class="sxs-lookup"><span data-stu-id="0f121-136">userIds</span></span>       | `collection(string)`    |  <span data-ttu-id="0f121-137">`schedulingGroup` のメンバーであるユーザー ID のリスト。</span><span class="sxs-lookup"><span data-stu-id="0f121-137">The list of user IDs that are a member of the `schedulingGroup`.</span></span> <span data-ttu-id="0f121-138">必須。</span><span class="sxs-lookup"><span data-stu-id="0f121-138">Required.</span></span> |
| <span data-ttu-id="0f121-139">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="0f121-139">createdDateTime</span></span>       |`DateTimeOffset`        |<span data-ttu-id="0f121-140">この `schedulingGroup` が最初に作成されたときのタイムスタンプ。</span><span class="sxs-lookup"><span data-stu-id="0f121-140">The time stamp in which this `schedulingGroup` was first created.</span></span> <span data-ttu-id="0f121-141">Timestamp 型は、ISO 8601 形式を使用して日付と時刻の情報を表します。これは常に UTC 時間です。</span><span class="sxs-lookup"><span data-stu-id="0f121-141">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="0f121-142">たとえば、2014 年 1 月 1 日午前 0 時 (UTC) は、'2014-01-01T00:00:00Z'.のようになります。</span><span class="sxs-lookup"><span data-stu-id="0f121-142">For example, midnight UTC on Jan 1, 2014 would look like this: '2014-01-01T00:00:00Z'.</span></span> |
| <span data-ttu-id="0f121-143">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="0f121-143">lastModifiedDateTime</span></span>      |`DateTimeOffset`        |<span data-ttu-id="0f121-144">この `schedulingGroup` の最終更新日のタイムスタンプ。</span><span class="sxs-lookup"><span data-stu-id="0f121-144">The time stamp in which this `schedulingGroup` was last updated.</span></span> <span data-ttu-id="0f121-145">Timestamp 型は、ISO 8601 形式を使用して日付と時刻の情報を表します。これは常に UTC 時間です。</span><span class="sxs-lookup"><span data-stu-id="0f121-145">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="0f121-146">たとえば、2014 年 1 月 1 日午前 0 時 (UTC) は、'2014-01-01T00:00:00Z'.のようになります。</span><span class="sxs-lookup"><span data-stu-id="0f121-146">For example, midnight UTC on Jan 1, 2014 would look like this: '2014-01-01T00:00:00Z'.</span></span> |
| <span data-ttu-id="0f121-147">lastModifiedBy</span><span class="sxs-lookup"><span data-stu-id="0f121-147">lastModifiedBy</span></span>        | [<span data-ttu-id="0f121-148">identitySet</span><span class="sxs-lookup"><span data-stu-id="0f121-148">identitySet</span></span>](identityset.md) |<span data-ttu-id="0f121-149">この `schedulingGroup` を最後に更新した ID。</span><span class="sxs-lookup"><span data-stu-id="0f121-149">The identity that last updated this `schedulingGroup`.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="0f121-150">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="0f121-150">JSON representation</span></span>

<span data-ttu-id="0f121-151">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="0f121-151">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.schedulingGroup",
  "baseType": "microsoft.graph.changeTrackedEntity"
}-->

```json
{
  "id": "string (identifier)",
  "createdDateTime": "String (timestamp)",
  "lastModifiedDateTime": "String (timestamp)",
  "displayName": "String",
  "isActive": true,
  "userIds": ["String (identifier)"],
  "lastModifiedBy":{"@odata.type":"microsoft.graph.identitySet"}
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
  "suppressions": []
}
-->
