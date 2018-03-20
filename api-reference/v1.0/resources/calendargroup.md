# <a name="calendargroup-resource-type"></a><span data-ttu-id="f60d5-101">calendarGroup リソースの種類</span><span class="sxs-lookup"><span data-stu-id="f60d5-101">calendarGroup resource type</span></span>

<span data-ttu-id="f60d5-102">予定表のグループです。</span><span class="sxs-lookup"><span data-stu-id="f60d5-102">A group of calendars.</span></span>

## <a name="methods"></a><span data-ttu-id="f60d5-103">メソッド</span><span class="sxs-lookup"><span data-stu-id="f60d5-103">Methods</span></span>

| <span data-ttu-id="f60d5-104">メソッド</span><span class="sxs-lookup"><span data-stu-id="f60d5-104">Method</span></span>                                                      | <span data-ttu-id="f60d5-105">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="f60d5-105">Return Type</span></span>                        | <span data-ttu-id="f60d5-106">説明</span><span class="sxs-lookup"><span data-stu-id="f60d5-106">Description</span></span>                                                   |
| :---------------------------------------------------------- | :--------------------------------- | :------------------------------------------------------------ |
| [<span data-ttu-id="f60d5-107">予定表グループを一覧表示する</span><span class="sxs-lookup"><span data-stu-id="f60d5-107">List calendar groups</span></span>](../api/user_list_calendargroups.md)  | <span data-ttu-id="f60d5-108">[Calendar](calendar.md) collection</span><span class="sxs-lookup"><span data-stu-id="f60d5-108">[Calendar](calendar.md) collection</span></span> | <span data-ttu-id="f60d5-109">ユーザーの予定表グループを取得します。</span><span class="sxs-lookup"><span data-stu-id="f60d5-109">Get the user's calendar groups.</span></span>                               |
| [<span data-ttu-id="f60d5-110">予定表グループを作成する</span><span class="sxs-lookup"><span data-stu-id="f60d5-110">Create calendar group</span></span>](../api/user_post_calendargroups.md) | [<span data-ttu-id="f60d5-111">Calendar</span><span class="sxs-lookup"><span data-stu-id="f60d5-111">Calendar</span></span>](calendar.md)            | <span data-ttu-id="f60d5-112">新しい予定表グループを作成します。</span><span class="sxs-lookup"><span data-stu-id="f60d5-112">Create a new calendar group.</span></span>                                  |
| [<span data-ttu-id="f60d5-113">予定表グループを取得する</span><span class="sxs-lookup"><span data-stu-id="f60d5-113">Get calendar group</span></span>](../api/calendargroup_get.md)           | [<span data-ttu-id="f60d5-114">calendarGroup</span><span class="sxs-lookup"><span data-stu-id="f60d5-114">calendarGroup</span></span>](calendargroup.md)  | <span data-ttu-id="f60d5-115">予定表グループ オブジェクトのプロパティと関係を読み取ります。</span><span class="sxs-lookup"><span data-stu-id="f60d5-115">Read properties and relationships of a calendar group object.</span></span> |
| [<span data-ttu-id="f60d5-116">Update</span><span class="sxs-lookup"><span data-stu-id="f60d5-116">Update</span></span>](../api/calendargroup_update.md)                    | [<span data-ttu-id="f60d5-117">calendarGroup</span><span class="sxs-lookup"><span data-stu-id="f60d5-117">calendarGroup</span></span>](calendargroup.md)  | <span data-ttu-id="f60d5-118">calendarGroup オブジェクトを更新します。</span><span class="sxs-lookup"><span data-stu-id="f60d5-118">Update calendarGroup object.</span></span>                                  |
| [<span data-ttu-id="f60d5-119">Delete</span><span class="sxs-lookup"><span data-stu-id="f60d5-119">Delete</span></span>](../api/calendargroup_delete.md)                    | <span data-ttu-id="f60d5-120">なし</span><span class="sxs-lookup"><span data-stu-id="f60d5-120">None</span></span>                               | <span data-ttu-id="f60d5-121">calendarGroup オブジェクトを削除します。</span><span class="sxs-lookup"><span data-stu-id="f60d5-121">Delete calendarGroup object.</span></span>                                  |
| [<span data-ttu-id="f60d5-122">予定表を一覧表示する</span><span class="sxs-lookup"><span data-stu-id="f60d5-122">List calendars</span></span>](../api/calendargroup_list_calendars.md)    | <span data-ttu-id="f60d5-123">[Calendar](calendar.md) collection</span><span class="sxs-lookup"><span data-stu-id="f60d5-123">[Calendar](calendar.md) collection</span></span> | <span data-ttu-id="f60d5-124">予定表グループ内の予定表を一覧表示する</span><span class="sxs-lookup"><span data-stu-id="f60d5-124">List calendars in a calendar group.</span></span>                           |
| [<span data-ttu-id="f60d5-125">予定表を作成する</span><span class="sxs-lookup"><span data-stu-id="f60d5-125">Create Calendar</span></span>](../api/calendargroup_post_calendars.md)   | [<span data-ttu-id="f60d5-126">Calendar</span><span class="sxs-lookup"><span data-stu-id="f60d5-126">Calendar</span></span>](calendar.md)            | <span data-ttu-id="f60d5-127">予定表グループに新しい予定表を作成します。</span><span class="sxs-lookup"><span data-stu-id="f60d5-127">Create a new Calendar in a calendar group.</span></span>                    |

## <a name="properties"></a><span data-ttu-id="f60d5-128">プロパティ</span><span class="sxs-lookup"><span data-stu-id="f60d5-128">Properties</span></span>

| <span data-ttu-id="f60d5-129">プロパティ</span><span class="sxs-lookup"><span data-stu-id="f60d5-129">Property</span></span>  | <span data-ttu-id="f60d5-130">型</span><span class="sxs-lookup"><span data-stu-id="f60d5-130">Type</span></span>   | <span data-ttu-id="f60d5-131">説明</span><span class="sxs-lookup"><span data-stu-id="f60d5-131">Description</span></span>                                                                                                                                                                                               |
| :-------- | :----- | :-------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| <span data-ttu-id="f60d5-132">name</span><span class="sxs-lookup"><span data-stu-id="f60d5-132">name</span></span>      | <span data-ttu-id="f60d5-133">String</span><span class="sxs-lookup"><span data-stu-id="f60d5-133">String</span></span> | <span data-ttu-id="f60d5-134">グループの名前。</span><span class="sxs-lookup"><span data-stu-id="f60d5-134">The group name.</span></span>                                                                                                                                                                                           |
| <span data-ttu-id="f60d5-135">changeKey</span><span class="sxs-lookup"><span data-stu-id="f60d5-135">changeKey</span></span> | <span data-ttu-id="f60d5-136">String</span><span class="sxs-lookup"><span data-stu-id="f60d5-136">String</span></span> | <span data-ttu-id="f60d5-p101">予定表グループのバージョンを識別します。予定表グループを変更するたびに ChangeKey も変更されます。これにより、Exchange は正しいバージョンのオブジェクトに変更を適用できます。読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="f60d5-p101">Identifies the version of the calendar group. Every time the calendar group is changed, ChangeKey changes as well. This allows Exchange to apply changes to the correct version of the object. Read-only.</span></span> |
| <span data-ttu-id="f60d5-141">classId</span><span class="sxs-lookup"><span data-stu-id="f60d5-141">classId</span></span>   | <span data-ttu-id="f60d5-142">Guid</span><span class="sxs-lookup"><span data-stu-id="f60d5-142">Guid</span></span>   | <span data-ttu-id="f60d5-p102">クラス識別子。読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="f60d5-p102">The class identifier. Read-only.</span></span>                                                                                                                                                                          |
| <span data-ttu-id="f60d5-145">id</span><span class="sxs-lookup"><span data-stu-id="f60d5-145">id</span></span>        | <span data-ttu-id="f60d5-146">String</span><span class="sxs-lookup"><span data-stu-id="f60d5-146">String</span></span> | <span data-ttu-id="f60d5-p103">グループの一意識別子。読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="f60d5-p103">The group's unique identifier. Read-only.</span></span>                                                                                                                                                                 |

## <a name="relationships"></a><span data-ttu-id="f60d5-149">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="f60d5-149">Relationships</span></span>

| <span data-ttu-id="f60d5-150">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="f60d5-150">Relationship</span></span> | <span data-ttu-id="f60d5-151">型</span><span class="sxs-lookup"><span data-stu-id="f60d5-151">Type</span></span>                               | <span data-ttu-id="f60d5-152">説明</span><span class="sxs-lookup"><span data-stu-id="f60d5-152">Description</span></span>                                                                    |
| :----------- | :--------------------------------- | :----------------------------------------------------------------------------- |
| <span data-ttu-id="f60d5-153">予定表</span><span class="sxs-lookup"><span data-stu-id="f60d5-153">calendars</span></span>    | <span data-ttu-id="f60d5-154">[Calendar](calendar.md) collection</span><span class="sxs-lookup"><span data-stu-id="f60d5-154">[Calendar](calendar.md) collection</span></span> | <span data-ttu-id="f60d5-p104">予定表グループ内の予定表。ナビゲーション プロパティ。読み取り専用です。Null 許容型。</span><span class="sxs-lookup"><span data-stu-id="f60d5-p104">The calendars in the calendar group. Navigation property. Read-only. Nullable.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="f60d5-159">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="f60d5-159">JSON representation</span></span>

<span data-ttu-id="f60d5-160">以下は、リソースの JSON 表記です</span><span class="sxs-lookup"><span data-stu-id="f60d5-160">Here is a JSON representation of the resource</span></span>

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
