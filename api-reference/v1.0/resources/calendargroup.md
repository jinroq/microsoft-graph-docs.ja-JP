---
title: calendarGroup リソースの種類
description: ユーザーカレンダーのグループ。
author: angelgolfer-ms
localization_priority: Normal
ms.prod: outlook
doc_type: resourcePageType
ms.openlocfilehash: 3931359b3b7eec65e2c675fbc5b6ef40176b13fb
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "36033055"
---
# <a name="calendargroup-resource-type"></a><span data-ttu-id="2e1cf-103">calendarGroup リソースの種類</span><span class="sxs-lookup"><span data-stu-id="2e1cf-103">calendarGroup resource type</span></span>

<span data-ttu-id="2e1cf-104">ユーザーカレンダーのグループ。</span><span class="sxs-lookup"><span data-stu-id="2e1cf-104">A group of user calendars.</span></span>

## <a name="methods"></a><span data-ttu-id="2e1cf-105">メソッド</span><span class="sxs-lookup"><span data-stu-id="2e1cf-105">Methods</span></span>

| <span data-ttu-id="2e1cf-106">メソッド</span><span class="sxs-lookup"><span data-stu-id="2e1cf-106">Method</span></span>                                                      | <span data-ttu-id="2e1cf-107">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="2e1cf-107">Return Type</span></span>                        | <span data-ttu-id="2e1cf-108">説明</span><span class="sxs-lookup"><span data-stu-id="2e1cf-108">Description</span></span>                                                   |
| :---------------------------------------------------------- | :--------------------------------- | :------------------------------------------------------------ |
| [<span data-ttu-id="2e1cf-109">予定表グループを一覧表示する</span><span class="sxs-lookup"><span data-stu-id="2e1cf-109">List calendar groups</span></span>](../api/user-list-calendargroups.md)  | <span data-ttu-id="2e1cf-110">[Calendar](calendar.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="2e1cf-110">[Calendar](calendar.md) collection</span></span> | <span data-ttu-id="2e1cf-111">ユーザーの予定表グループを取得します。</span><span class="sxs-lookup"><span data-stu-id="2e1cf-111">Get the user's calendar groups.</span></span>                               |
| [<span data-ttu-id="2e1cf-112">予定表グループを作成する</span><span class="sxs-lookup"><span data-stu-id="2e1cf-112">Create calendar group</span></span>](../api/user-post-calendargroups.md) | [<span data-ttu-id="2e1cf-113">Calendar</span><span class="sxs-lookup"><span data-stu-id="2e1cf-113">Calendar</span></span>](calendar.md)            | <span data-ttu-id="2e1cf-114">新しい予定表グループを作成します。</span><span class="sxs-lookup"><span data-stu-id="2e1cf-114">Create a new calendar group.</span></span>                                  |
| [<span data-ttu-id="2e1cf-115">予定表グループを取得する</span><span class="sxs-lookup"><span data-stu-id="2e1cf-115">Get calendar group</span></span>](../api/calendargroup-get.md)           | [<span data-ttu-id="2e1cf-116">calendarGroup</span><span class="sxs-lookup"><span data-stu-id="2e1cf-116">calendarGroup</span></span>](calendargroup.md)  | <span data-ttu-id="2e1cf-117">予定表グループ オブジェクトのプロパティと関係を読み取ります。</span><span class="sxs-lookup"><span data-stu-id="2e1cf-117">Read properties and relationships of a calendar group object.</span></span> |
| [<span data-ttu-id="2e1cf-118">Update</span><span class="sxs-lookup"><span data-stu-id="2e1cf-118">Update</span></span>](../api/calendargroup-update.md)                    | [<span data-ttu-id="2e1cf-119">calendarGroup</span><span class="sxs-lookup"><span data-stu-id="2e1cf-119">calendarGroup</span></span>](calendargroup.md)  | <span data-ttu-id="2e1cf-120">calendarGroup オブジェクトを更新します。</span><span class="sxs-lookup"><span data-stu-id="2e1cf-120">Update calendarGroup object.</span></span>                                  |
| [<span data-ttu-id="2e1cf-121">Delete</span><span class="sxs-lookup"><span data-stu-id="2e1cf-121">Delete</span></span>](../api/calendargroup-delete.md)                    | <span data-ttu-id="2e1cf-122">None</span><span class="sxs-lookup"><span data-stu-id="2e1cf-122">None</span></span>                               | <span data-ttu-id="2e1cf-123">calendarGroup オブジェクトを削除します。</span><span class="sxs-lookup"><span data-stu-id="2e1cf-123">Delete calendarGroup object.</span></span>                                  |
| [<span data-ttu-id="2e1cf-124">List calendars</span><span class="sxs-lookup"><span data-stu-id="2e1cf-124">List calendars</span></span>](../api/calendargroup-list-calendars.md)    | <span data-ttu-id="2e1cf-125">[Calendar](calendar.md) collection</span><span class="sxs-lookup"><span data-stu-id="2e1cf-125">[Calendar](calendar.md) collection</span></span> | <span data-ttu-id="2e1cf-126">予定表グループ内の予定表を一覧表示する</span><span class="sxs-lookup"><span data-stu-id="2e1cf-126">List calendars in a calendar group.</span></span>                           |
| [<span data-ttu-id="2e1cf-127">予定表を作成する</span><span class="sxs-lookup"><span data-stu-id="2e1cf-127">Create Calendar</span></span>](../api/calendargroup-post-calendars.md)   | [<span data-ttu-id="2e1cf-128">Calendar</span><span class="sxs-lookup"><span data-stu-id="2e1cf-128">Calendar</span></span>](calendar.md)            | <span data-ttu-id="2e1cf-129">予定表グループに新しい予定表を作成します。</span><span class="sxs-lookup"><span data-stu-id="2e1cf-129">Create a new Calendar in a calendar group.</span></span>                    |

## <a name="properties"></a><span data-ttu-id="2e1cf-130">プロパティ</span><span class="sxs-lookup"><span data-stu-id="2e1cf-130">Properties</span></span>

| <span data-ttu-id="2e1cf-131">プロパティ</span><span class="sxs-lookup"><span data-stu-id="2e1cf-131">Property</span></span>  | <span data-ttu-id="2e1cf-132">型</span><span class="sxs-lookup"><span data-stu-id="2e1cf-132">Type</span></span>   | <span data-ttu-id="2e1cf-133">説明</span><span class="sxs-lookup"><span data-stu-id="2e1cf-133">Description</span></span>                                                                                                                                                                                               |
| :-------- | :----- | :-------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| <span data-ttu-id="2e1cf-134">name</span><span class="sxs-lookup"><span data-stu-id="2e1cf-134">name</span></span>      | <span data-ttu-id="2e1cf-135">String</span><span class="sxs-lookup"><span data-stu-id="2e1cf-135">String</span></span> | <span data-ttu-id="2e1cf-136">グループの名前。</span><span class="sxs-lookup"><span data-stu-id="2e1cf-136">The group name.</span></span>                                                                                                                                                                                           |
| <span data-ttu-id="2e1cf-137">changeKey</span><span class="sxs-lookup"><span data-stu-id="2e1cf-137">changeKey</span></span> | <span data-ttu-id="2e1cf-138">String</span><span class="sxs-lookup"><span data-stu-id="2e1cf-138">String</span></span> | <span data-ttu-id="2e1cf-p101">予定表グループのバージョンを識別します。予定表グループを変更するたびに ChangeKey も変更されます。これにより、Exchange は正しいバージョンのオブジェクトに変更を適用できます。読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="2e1cf-p101">Identifies the version of the calendar group. Every time the calendar group is changed, ChangeKey changes as well. This allows Exchange to apply changes to the correct version of the object. Read-only.</span></span> |
| <span data-ttu-id="2e1cf-143">classId</span><span class="sxs-lookup"><span data-stu-id="2e1cf-143">classId</span></span>   | <span data-ttu-id="2e1cf-144">Guid</span><span class="sxs-lookup"><span data-stu-id="2e1cf-144">Guid</span></span>   | <span data-ttu-id="2e1cf-p102">クラス識別子。読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="2e1cf-p102">The class identifier. Read-only.</span></span>                                                                                                                                                                          |
| <span data-ttu-id="2e1cf-147">id</span><span class="sxs-lookup"><span data-stu-id="2e1cf-147">id</span></span>        | <span data-ttu-id="2e1cf-148">String</span><span class="sxs-lookup"><span data-stu-id="2e1cf-148">String</span></span> | <span data-ttu-id="2e1cf-p103">グループの一意識別子。読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="2e1cf-p103">The group's unique identifier. Read-only.</span></span>                                                                                                                                                                 |

## <a name="relationships"></a><span data-ttu-id="2e1cf-151">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="2e1cf-151">Relationships</span></span>

| <span data-ttu-id="2e1cf-152">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="2e1cf-152">Relationship</span></span> | <span data-ttu-id="2e1cf-153">型</span><span class="sxs-lookup"><span data-stu-id="2e1cf-153">Type</span></span>                               | <span data-ttu-id="2e1cf-154">説明</span><span class="sxs-lookup"><span data-stu-id="2e1cf-154">Description</span></span>                                                                    |
| :----------- | :--------------------------------- | :----------------------------------------------------------------------------- |
| <span data-ttu-id="2e1cf-155">calendars</span><span class="sxs-lookup"><span data-stu-id="2e1cf-155">calendars</span></span>    | <span data-ttu-id="2e1cf-156">[Calendar](calendar.md) collection</span><span class="sxs-lookup"><span data-stu-id="2e1cf-156">[Calendar](calendar.md) collection</span></span> | <span data-ttu-id="2e1cf-p104">予定表グループ内の予定表。ナビゲーション プロパティ。読み取り専用です。Null 許容型。</span><span class="sxs-lookup"><span data-stu-id="2e1cf-p104">The calendars in the calendar group. Navigation property. Read-only. Nullable.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="2e1cf-161">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="2e1cf-161">JSON representation</span></span>

<span data-ttu-id="2e1cf-162">以下は、リソースの JSON 表記です</span><span class="sxs-lookup"><span data-stu-id="2e1cf-162">Here is a JSON representation of the resource</span></span>

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
