---
title: calendarGroup リソースの種類
description: ユーザーの予定表のグループです。
author: angelgolfer-ms
localization_priority: Normal
ms.prod: outlook
ms.openlocfilehash: 10a840fd9ae9835eb5ca6a96b88719605f89245b
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/12/2019
ms.locfileid: "27985292"
---
# <a name="calendargroup-resource-type"></a><span data-ttu-id="688e6-103">calendarGroup リソースの種類</span><span class="sxs-lookup"><span data-stu-id="688e6-103">calendarGroup resource type</span></span>

> <span data-ttu-id="688e6-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="688e6-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="688e6-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="688e6-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="688e6-106">ユーザーの予定表のグループです。</span><span class="sxs-lookup"><span data-stu-id="688e6-106">A group of user calendars.</span></span>

## <a name="methods"></a><span data-ttu-id="688e6-107">メソッド</span><span class="sxs-lookup"><span data-stu-id="688e6-107">Methods</span></span>

| <span data-ttu-id="688e6-108">メソッド</span><span class="sxs-lookup"><span data-stu-id="688e6-108">Method</span></span>                                                      | <span data-ttu-id="688e6-109">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="688e6-109">Return Type</span></span>                        | <span data-ttu-id="688e6-110">説明</span><span class="sxs-lookup"><span data-stu-id="688e6-110">Description</span></span>                                                   |
| :---------------------------------------------------------- | :--------------------------------- | :------------------------------------------------------------ |
| [<span data-ttu-id="688e6-111">予定表グループを一覧表示する</span><span class="sxs-lookup"><span data-stu-id="688e6-111">List calendar groups</span></span>](../api/user-list-calendargroups.md)  | <span data-ttu-id="688e6-112">[Calendar](calendar.md) collection</span><span class="sxs-lookup"><span data-stu-id="688e6-112">[Calendar](calendar.md) collection</span></span> | <span data-ttu-id="688e6-113">ユーザーの予定表グループを取得します。</span><span class="sxs-lookup"><span data-stu-id="688e6-113">Get the user's calendar groups.</span></span>                               |
| [<span data-ttu-id="688e6-114">予定表グループを作成する</span><span class="sxs-lookup"><span data-stu-id="688e6-114">Create calendar group</span></span>](../api/user-post-calendargroups.md) | [<span data-ttu-id="688e6-115">Calendar</span><span class="sxs-lookup"><span data-stu-id="688e6-115">Calendar</span></span>](calendar.md)            | <span data-ttu-id="688e6-116">新しい予定表グループを作成します。</span><span class="sxs-lookup"><span data-stu-id="688e6-116">Create a new calendar group.</span></span>                                  |
| [<span data-ttu-id="688e6-117">予定表グループを取得する</span><span class="sxs-lookup"><span data-stu-id="688e6-117">Get calendar group</span></span>](../api/calendargroup-get.md)           | [<span data-ttu-id="688e6-118">calendarGroup</span><span class="sxs-lookup"><span data-stu-id="688e6-118">calendarGroup</span></span>](calendargroup.md)  | <span data-ttu-id="688e6-119">予定表グループ オブジェクトのプロパティと関係を読み取ります。</span><span class="sxs-lookup"><span data-stu-id="688e6-119">Read properties and relationships of a calendar group object.</span></span> |
| [<span data-ttu-id="688e6-120">Update</span><span class="sxs-lookup"><span data-stu-id="688e6-120">Update</span></span>](../api/calendargroup-update.md)                    | [<span data-ttu-id="688e6-121">calendarGroup</span><span class="sxs-lookup"><span data-stu-id="688e6-121">calendarGroup</span></span>](calendargroup.md)  | <span data-ttu-id="688e6-122">calendarGroup オブジェクトを更新します。</span><span class="sxs-lookup"><span data-stu-id="688e6-122">Update calendarGroup object.</span></span>                                  |
| [<span data-ttu-id="688e6-123">Delete</span><span class="sxs-lookup"><span data-stu-id="688e6-123">Delete</span></span>](../api/calendargroup-delete.md)                    | <span data-ttu-id="688e6-124">なし</span><span class="sxs-lookup"><span data-stu-id="688e6-124">None</span></span>                               | <span data-ttu-id="688e6-125">calendarGroup オブジェクトを削除します。</span><span class="sxs-lookup"><span data-stu-id="688e6-125">Delete calendarGroup object.</span></span>                                  |
| [<span data-ttu-id="688e6-126">予定表を一覧表示する</span><span class="sxs-lookup"><span data-stu-id="688e6-126">List calendars</span></span>](../api/calendargroup-list-calendars.md)    | <span data-ttu-id="688e6-127">[Calendar](calendar.md) collection</span><span class="sxs-lookup"><span data-stu-id="688e6-127">[Calendar](calendar.md) collection</span></span> | <span data-ttu-id="688e6-128">予定表グループ内の予定表を一覧表示する</span><span class="sxs-lookup"><span data-stu-id="688e6-128">List calendars in a calendar group.</span></span>                           |
| [<span data-ttu-id="688e6-129">予定表を作成する</span><span class="sxs-lookup"><span data-stu-id="688e6-129">Create Calendar</span></span>](../api/calendargroup-post-calendars.md)   | [<span data-ttu-id="688e6-130">Calendar</span><span class="sxs-lookup"><span data-stu-id="688e6-130">Calendar</span></span>](calendar.md)            | <span data-ttu-id="688e6-131">予定表グループに新しい予定表を作成します。</span><span class="sxs-lookup"><span data-stu-id="688e6-131">Create a new Calendar in a calendar group.</span></span>                    |

## <a name="properties"></a><span data-ttu-id="688e6-132">プロパティ</span><span class="sxs-lookup"><span data-stu-id="688e6-132">Properties</span></span>

| <span data-ttu-id="688e6-133">プロパティ</span><span class="sxs-lookup"><span data-stu-id="688e6-133">Property</span></span>  | <span data-ttu-id="688e6-134">型</span><span class="sxs-lookup"><span data-stu-id="688e6-134">Type</span></span>   | <span data-ttu-id="688e6-135">説明</span><span class="sxs-lookup"><span data-stu-id="688e6-135">Description</span></span>                                                                                                                                                                                               |
| :-------- | :----- | :-------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| <span data-ttu-id="688e6-136">名前</span><span class="sxs-lookup"><span data-stu-id="688e6-136">name</span></span>      | <span data-ttu-id="688e6-137">String</span><span class="sxs-lookup"><span data-stu-id="688e6-137">String</span></span> | <span data-ttu-id="688e6-138">グループの名前。</span><span class="sxs-lookup"><span data-stu-id="688e6-138">The group name.</span></span>                                                                                                                                                                                           |
| <span data-ttu-id="688e6-139">changeKey</span><span class="sxs-lookup"><span data-stu-id="688e6-139">changeKey</span></span> | <span data-ttu-id="688e6-140">String</span><span class="sxs-lookup"><span data-stu-id="688e6-140">String</span></span> | <span data-ttu-id="688e6-p102">予定表グループのバージョンを識別します。予定表グループを変更するたびに ChangeKey も変更されます。これにより、Exchange は正しいバージョンのオブジェクトに変更を適用できます。読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="688e6-p102">Identifies the version of the calendar group. Every time the calendar group is changed, ChangeKey changes as well. This allows Exchange to apply changes to the correct version of the object. Read-only.</span></span> |
| <span data-ttu-id="688e6-145">classId</span><span class="sxs-lookup"><span data-stu-id="688e6-145">classId</span></span>   | <span data-ttu-id="688e6-146">Guid</span><span class="sxs-lookup"><span data-stu-id="688e6-146">Guid</span></span>   | <span data-ttu-id="688e6-p103">クラス識別子。読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="688e6-p103">The class identifier. Read-only.</span></span>                                                                                                                                                                          |
| <span data-ttu-id="688e6-149">id</span><span class="sxs-lookup"><span data-stu-id="688e6-149">id</span></span>        | <span data-ttu-id="688e6-150">String</span><span class="sxs-lookup"><span data-stu-id="688e6-150">String</span></span> | <span data-ttu-id="688e6-p104">グループの一意識別子。読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="688e6-p104">The group's unique identifier. Read-only.</span></span>                                                                                                                                                                 |

## <a name="relationships"></a><span data-ttu-id="688e6-153">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="688e6-153">Relationships</span></span>

| <span data-ttu-id="688e6-154">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="688e6-154">Relationship</span></span> | <span data-ttu-id="688e6-155">型</span><span class="sxs-lookup"><span data-stu-id="688e6-155">Type</span></span>                               | <span data-ttu-id="688e6-156">説明</span><span class="sxs-lookup"><span data-stu-id="688e6-156">Description</span></span>                                                                    |
| :----------- | :--------------------------------- | :----------------------------------------------------------------------------- |
| <span data-ttu-id="688e6-157">予定表</span><span class="sxs-lookup"><span data-stu-id="688e6-157">calendars</span></span>    | <span data-ttu-id="688e6-158">[Calendar](calendar.md) collection</span><span class="sxs-lookup"><span data-stu-id="688e6-158">[Calendar](calendar.md) collection</span></span> | <span data-ttu-id="688e6-p105">予定表グループ内の予定表。ナビゲーション プロパティ。読み取り専用です。Null 許容型。</span><span class="sxs-lookup"><span data-stu-id="688e6-p105">The calendars in the calendar group. Navigation property. Read-only. Nullable.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="688e6-163">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="688e6-163">JSON representation</span></span>

<span data-ttu-id="688e6-164">以下は、リソースの JSON 表記です</span><span class="sxs-lookup"><span data-stu-id="688e6-164">Here is a JSON representation of the resource</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [
    "calendars"
  ],
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.calendarGroup"
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
