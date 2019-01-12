---
title: calendarGroup リソースの種類
description: ユーザーの予定表のグループです。
author: angelgolfer-ms
localization_priority: Normal
ms.prod: outlook
ms.openlocfilehash: 5b75ebf253276876129859be7d37ecb6748fc0d9
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/12/2019
ms.locfileid: "27949627"
---
# <a name="calendargroup-resource-type"></a><span data-ttu-id="67579-103">calendarGroup リソースの種類</span><span class="sxs-lookup"><span data-stu-id="67579-103">calendarGroup resource type</span></span>

<span data-ttu-id="67579-104">ユーザーの予定表のグループです。</span><span class="sxs-lookup"><span data-stu-id="67579-104">A group of user calendars.</span></span>

## <a name="methods"></a><span data-ttu-id="67579-105">メソッド</span><span class="sxs-lookup"><span data-stu-id="67579-105">Methods</span></span>

| <span data-ttu-id="67579-106">メソッド</span><span class="sxs-lookup"><span data-stu-id="67579-106">Method</span></span>                                                      | <span data-ttu-id="67579-107">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="67579-107">Return Type</span></span>                        | <span data-ttu-id="67579-108">説明</span><span class="sxs-lookup"><span data-stu-id="67579-108">Description</span></span>                                                   |
| :---------------------------------------------------------- | :--------------------------------- | :------------------------------------------------------------ |
| [<span data-ttu-id="67579-109">予定表グループを一覧表示する</span><span class="sxs-lookup"><span data-stu-id="67579-109">List calendar groups</span></span>](../api/user-list-calendargroups.md)  | <span data-ttu-id="67579-110">[Calendar](calendar.md) collection</span><span class="sxs-lookup"><span data-stu-id="67579-110">[Calendar](calendar.md) collection</span></span> | <span data-ttu-id="67579-111">ユーザーの予定表グループを取得します。</span><span class="sxs-lookup"><span data-stu-id="67579-111">Get the user's calendar groups.</span></span>                               |
| [<span data-ttu-id="67579-112">予定表グループを作成する</span><span class="sxs-lookup"><span data-stu-id="67579-112">Create calendar group</span></span>](../api/user-post-calendargroups.md) | [<span data-ttu-id="67579-113">Calendar</span><span class="sxs-lookup"><span data-stu-id="67579-113">Calendar</span></span>](calendar.md)            | <span data-ttu-id="67579-114">新しい予定表グループを作成します。</span><span class="sxs-lookup"><span data-stu-id="67579-114">Create a new calendar group.</span></span>                                  |
| [<span data-ttu-id="67579-115">予定表グループを取得する</span><span class="sxs-lookup"><span data-stu-id="67579-115">Get calendar group</span></span>](../api/calendargroup-get.md)           | [<span data-ttu-id="67579-116">calendarGroup</span><span class="sxs-lookup"><span data-stu-id="67579-116">calendarGroup</span></span>](calendargroup.md)  | <span data-ttu-id="67579-117">予定表グループ オブジェクトのプロパティと関係を読み取ります。</span><span class="sxs-lookup"><span data-stu-id="67579-117">Read properties and relationships of a calendar group object.</span></span> |
| [<span data-ttu-id="67579-118">Update</span><span class="sxs-lookup"><span data-stu-id="67579-118">Update</span></span>](../api/calendargroup-update.md)                    | [<span data-ttu-id="67579-119">calendarGroup</span><span class="sxs-lookup"><span data-stu-id="67579-119">calendarGroup</span></span>](calendargroup.md)  | <span data-ttu-id="67579-120">calendarGroup オブジェクトを更新します。</span><span class="sxs-lookup"><span data-stu-id="67579-120">Update calendarGroup object.</span></span>                                  |
| [<span data-ttu-id="67579-121">Delete</span><span class="sxs-lookup"><span data-stu-id="67579-121">Delete</span></span>](../api/calendargroup-delete.md)                    | <span data-ttu-id="67579-122">なし</span><span class="sxs-lookup"><span data-stu-id="67579-122">None</span></span>                               | <span data-ttu-id="67579-123">calendarGroup オブジェクトを削除します。</span><span class="sxs-lookup"><span data-stu-id="67579-123">Delete calendarGroup object.</span></span>                                  |
| [<span data-ttu-id="67579-124">予定表を一覧表示する</span><span class="sxs-lookup"><span data-stu-id="67579-124">List calendars</span></span>](../api/calendargroup-list-calendars.md)    | <span data-ttu-id="67579-125">[Calendar](calendar.md) collection</span><span class="sxs-lookup"><span data-stu-id="67579-125">[Calendar](calendar.md) collection</span></span> | <span data-ttu-id="67579-126">予定表グループ内の予定表を一覧表示する</span><span class="sxs-lookup"><span data-stu-id="67579-126">List calendars in a calendar group.</span></span>                           |
| [<span data-ttu-id="67579-127">予定表を作成する</span><span class="sxs-lookup"><span data-stu-id="67579-127">Create Calendar</span></span>](../api/calendargroup-post-calendars.md)   | [<span data-ttu-id="67579-128">Calendar</span><span class="sxs-lookup"><span data-stu-id="67579-128">Calendar</span></span>](calendar.md)            | <span data-ttu-id="67579-129">予定表グループに新しい予定表を作成します。</span><span class="sxs-lookup"><span data-stu-id="67579-129">Create a new Calendar in a calendar group.</span></span>                    |

## <a name="properties"></a><span data-ttu-id="67579-130">プロパティ</span><span class="sxs-lookup"><span data-stu-id="67579-130">Properties</span></span>

| <span data-ttu-id="67579-131">プロパティ</span><span class="sxs-lookup"><span data-stu-id="67579-131">Property</span></span>  | <span data-ttu-id="67579-132">種類</span><span class="sxs-lookup"><span data-stu-id="67579-132">Type</span></span>   | <span data-ttu-id="67579-133">説明</span><span class="sxs-lookup"><span data-stu-id="67579-133">Description</span></span>                                                                                                                                                                                               |
| :-------- | :----- | :-------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| <span data-ttu-id="67579-134">名前</span><span class="sxs-lookup"><span data-stu-id="67579-134">name</span></span>      | <span data-ttu-id="67579-135">String</span><span class="sxs-lookup"><span data-stu-id="67579-135">String</span></span> | <span data-ttu-id="67579-136">グループの名前。</span><span class="sxs-lookup"><span data-stu-id="67579-136">The group name.</span></span>                                                                                                                                                                                           |
| <span data-ttu-id="67579-137">changeKey</span><span class="sxs-lookup"><span data-stu-id="67579-137">changeKey</span></span> | <span data-ttu-id="67579-138">String</span><span class="sxs-lookup"><span data-stu-id="67579-138">String</span></span> | <span data-ttu-id="67579-p101">予定表グループのバージョンを識別します。予定表グループを変更するたびに ChangeKey も変更されます。これにより、Exchange は正しいバージョンのオブジェクトに変更を適用できます。読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="67579-p101">Identifies the version of the calendar group. Every time the calendar group is changed, ChangeKey changes as well. This allows Exchange to apply changes to the correct version of the object. Read-only.</span></span> |
| <span data-ttu-id="67579-143">classId</span><span class="sxs-lookup"><span data-stu-id="67579-143">classId</span></span>   | <span data-ttu-id="67579-144">Guid</span><span class="sxs-lookup"><span data-stu-id="67579-144">Guid</span></span>   | <span data-ttu-id="67579-p102">クラス識別子。読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="67579-p102">The class identifier. Read-only.</span></span>                                                                                                                                                                          |
| <span data-ttu-id="67579-147">id</span><span class="sxs-lookup"><span data-stu-id="67579-147">id</span></span>        | <span data-ttu-id="67579-148">String</span><span class="sxs-lookup"><span data-stu-id="67579-148">String</span></span> | <span data-ttu-id="67579-p103">グループの一意識別子。読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="67579-p103">The group's unique identifier. Read-only.</span></span>                                                                                                                                                                 |

## <a name="relationships"></a><span data-ttu-id="67579-151">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="67579-151">Relationships</span></span>

| <span data-ttu-id="67579-152">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="67579-152">Relationship</span></span> | <span data-ttu-id="67579-153">型</span><span class="sxs-lookup"><span data-stu-id="67579-153">Type</span></span>                               | <span data-ttu-id="67579-154">説明</span><span class="sxs-lookup"><span data-stu-id="67579-154">Description</span></span>                                                                    |
| :----------- | :--------------------------------- | :----------------------------------------------------------------------------- |
| <span data-ttu-id="67579-155">予定表</span><span class="sxs-lookup"><span data-stu-id="67579-155">calendars</span></span>    | <span data-ttu-id="67579-156">[Calendar](calendar.md) collection</span><span class="sxs-lookup"><span data-stu-id="67579-156">[Calendar](calendar.md) collection</span></span> | <span data-ttu-id="67579-p104">予定表グループ内の予定表。ナビゲーション プロパティ。読み取り専用です。Null 許容型。</span><span class="sxs-lookup"><span data-stu-id="67579-p104">The calendars in the calendar group. Navigation property. Read-only. Nullable.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="67579-161">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="67579-161">JSON representation</span></span>

<span data-ttu-id="67579-162">以下は、リソースの JSON 表記です</span><span class="sxs-lookup"><span data-stu-id="67579-162">Here is a JSON representation of the resource</span></span>

<!--{
  "blockType": "resource",
  "optionalProperties": [
    "calendars"
  ],
  "keyProperty": "id",
  "baseType": "microsoft.graph.entity",
  "@odata.type": "microsoft.graph.calendarGroup",
  "@odata.annotations": [
    {
      "property": "calendars",
      "capabilities": {
        "changeTracking": false,
        "expandable": false,
        "navigability": "single",
        "searchable": false
      }
    }
  ]
}-->

```json
{
  "changeKey": "string",
  "classId": "guid",
  "id": "string (identifier)",
  "name": "string"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->

<!-- {
  "type": "#page.annotation",
  "description": "calendarGroup resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
