# <a name="calendargroup-resource-type"></a><span data-ttu-id="54c0f-101">calendarGroup リソースの種類</span><span class="sxs-lookup"><span data-stu-id="54c0f-101">calendarGroup resource type</span></span>

<span data-ttu-id="54c0f-102">ユーザーの予定表のグループです。</span><span class="sxs-lookup"><span data-stu-id="54c0f-102">A group of calendars.</span></span>

## <a name="methods"></a><span data-ttu-id="54c0f-103">メソッド</span><span class="sxs-lookup"><span data-stu-id="54c0f-103">Methods</span></span>

| <span data-ttu-id="54c0f-104">メソッド</span><span class="sxs-lookup"><span data-stu-id="54c0f-104">Method</span></span>                                                      | <span data-ttu-id="54c0f-105">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="54c0f-105">Return Type</span></span>                        | <span data-ttu-id="54c0f-106">説明</span><span class="sxs-lookup"><span data-stu-id="54c0f-106">Description</span></span>                                                   |
| :---------------------------------------------------------- | :--------------------------------- | :------------------------------------------------------------ |
| [<span data-ttu-id="54c0f-107">予定表グループを一覧表示する</span><span class="sxs-lookup"><span data-stu-id="54c0f-107">List calendar groups</span></span>](../api/user_list_calendargroups.md)  | <span data-ttu-id="54c0f-108">[Calendar](calendar.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="54c0f-108">[Calendar](calendar.md) collection</span></span> | <span data-ttu-id="54c0f-109">ユーザーの予定表グループを取得します。</span><span class="sxs-lookup"><span data-stu-id="54c0f-109">Get the user's calendar groups.</span></span>                               |
| [<span data-ttu-id="54c0f-110">予定表グループを作成する</span><span class="sxs-lookup"><span data-stu-id="54c0f-110">Create calendar group</span></span>](../api/user_post_calendargroups.md) | [<span data-ttu-id="54c0f-111">カレンダー</span><span class="sxs-lookup"><span data-stu-id="54c0f-111">Calendar</span></span>](calendar.md)            | <span data-ttu-id="54c0f-112">新しい予定表グループを作成します。</span><span class="sxs-lookup"><span data-stu-id="54c0f-112">Create a new calendar group.</span></span>                                  |
| [<span data-ttu-id="54c0f-113">予定表グループを取得する</span><span class="sxs-lookup"><span data-stu-id="54c0f-113">Get calendar group</span></span>](../api/calendargroup_get.md)           | [<span data-ttu-id="54c0f-114">calendarGroup</span><span class="sxs-lookup"><span data-stu-id="54c0f-114">calendarGroup</span></span>](calendargroup.md)  | <span data-ttu-id="54c0f-115">予定表グループ オブジェクトのプロパティと関係を読み取ります。</span><span class="sxs-lookup"><span data-stu-id="54c0f-115">Read properties and relationships of a calendar group object.</span></span> |
| [<span data-ttu-id="54c0f-116">更新する</span><span class="sxs-lookup"><span data-stu-id="54c0f-116">Update</span></span>](../api/calendargroup_update.md)                    | [<span data-ttu-id="54c0f-117">calendarGroup</span><span class="sxs-lookup"><span data-stu-id="54c0f-117">calendarGroup</span></span>](calendargroup.md)  | <span data-ttu-id="54c0f-118">calendarGroup オブジェクトを更新します。</span><span class="sxs-lookup"><span data-stu-id="54c0f-118">Update calendarGroup object.</span></span>                                  |
| [<span data-ttu-id="54c0f-119">削除</span><span class="sxs-lookup"><span data-stu-id="54c0f-119">Delete</span></span>](../api/calendargroup_delete.md)                    | <span data-ttu-id="54c0f-120">なし</span><span class="sxs-lookup"><span data-stu-id="54c0f-120">None</span></span>                               | <span data-ttu-id="54c0f-121">calendarGroup オブジェクトを削除します。</span><span class="sxs-lookup"><span data-stu-id="54c0f-121">Delete calendarGroup object.</span></span>                                  |
| [<span data-ttu-id="54c0f-122">予定表を一覧表示する</span><span class="sxs-lookup"><span data-stu-id="54c0f-122">List calendars</span></span>](../api/calendargroup_list_calendars.md)    | <span data-ttu-id="54c0f-123">[Calendar](calendar.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="54c0f-123">[Calendar](calendar.md) collection</span></span> | <span data-ttu-id="54c0f-124">予定表グループ内の予定表を一覧表示する</span><span class="sxs-lookup"><span data-stu-id="54c0f-124">List calendars in a calendar group.</span></span>                           |
| [<span data-ttu-id="54c0f-125">予定表を作成する</span><span class="sxs-lookup"><span data-stu-id="54c0f-125">Create Calendar</span></span>](../api/calendargroup_post_calendars.md)   | [<span data-ttu-id="54c0f-126">カレンダー</span><span class="sxs-lookup"><span data-stu-id="54c0f-126">Calendar</span></span>](calendar.md)            | <span data-ttu-id="54c0f-127">予定表グループに新しい予定表を作成します。</span><span class="sxs-lookup"><span data-stu-id="54c0f-127">Create a new Calendar in a calendar group.</span></span>                    |

## <a name="properties"></a><span data-ttu-id="54c0f-128">プロパティ</span><span class="sxs-lookup"><span data-stu-id="54c0f-128">Properties</span></span>

| <span data-ttu-id="54c0f-129">プロパティ</span><span class="sxs-lookup"><span data-stu-id="54c0f-129">Property</span></span>  | <span data-ttu-id="54c0f-130">タイプ</span><span class="sxs-lookup"><span data-stu-id="54c0f-130">Type</span></span>   | <span data-ttu-id="54c0f-131">説明</span><span class="sxs-lookup"><span data-stu-id="54c0f-131">Description</span></span>                                                                                                                                                                                               |
| :-------- | :----- | :-------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| <span data-ttu-id="54c0f-132">名前</span><span class="sxs-lookup"><span data-stu-id="54c0f-132">name</span></span>      | <span data-ttu-id="54c0f-133">文字列</span><span class="sxs-lookup"><span data-stu-id="54c0f-133">String</span></span> | <span data-ttu-id="54c0f-134">グループの名前。</span><span class="sxs-lookup"><span data-stu-id="54c0f-134">The group name.</span></span>                                                                                                                                                                                           |
| <span data-ttu-id="54c0f-135">変更キー</span><span class="sxs-lookup"><span data-stu-id="54c0f-135">changeKey</span></span> | <span data-ttu-id="54c0f-136">文字列</span><span class="sxs-lookup"><span data-stu-id="54c0f-136">String</span></span> | <span data-ttu-id="54c0f-p101">予定表グループのバージョンを識別します。予定表グループを変更するたびに ChangeKey も変更されます。これにより、Exchange は正しいバージョンのオブジェクトに変更を適用できます。読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="54c0f-p101">Identifies the version of the calendar group. Every time the calendar group is changed, ChangeKey changes as well. This allows Exchange to apply changes to the correct version of the object. Read-only.</span></span> |
| <span data-ttu-id="54c0f-141">classId</span><span class="sxs-lookup"><span data-stu-id="54c0f-141">classId</span></span>   | <span data-ttu-id="54c0f-142">Guid型</span><span class="sxs-lookup"><span data-stu-id="54c0f-142">Guid</span></span>   | <span data-ttu-id="54c0f-p102">クラス識別子。読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="54c0f-p102">The class identifier. Read-only.</span></span>                                                                                                                                                                          |
| <span data-ttu-id="54c0f-145">ID</span><span class="sxs-lookup"><span data-stu-id="54c0f-145">id</span></span>        | <span data-ttu-id="54c0f-146">文字列</span><span class="sxs-lookup"><span data-stu-id="54c0f-146">String</span></span> | <span data-ttu-id="54c0f-p103">グループの一意識別子。読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="54c0f-p103">The group's unique identifier. Read-only.</span></span>                                                                                                                                                                 |

## <a name="relationships"></a><span data-ttu-id="54c0f-149">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="54c0f-149">Relationships</span></span>

| <span data-ttu-id="54c0f-150">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="54c0f-150">Relationship</span></span> | <span data-ttu-id="54c0f-151">型</span><span class="sxs-lookup"><span data-stu-id="54c0f-151">Type</span></span>                               | <span data-ttu-id="54c0f-152">説明</span><span class="sxs-lookup"><span data-stu-id="54c0f-152">Description</span></span>                                                                    |
| :----------- | :--------------------------------- | :----------------------------------------------------------------------------- |
| <span data-ttu-id="54c0f-153">予定表</span><span class="sxs-lookup"><span data-stu-id="54c0f-153">calendars</span></span>    | <span data-ttu-id="54c0f-154">[Calendar](calendar.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="54c0f-154">[Calendar](calendar.md) collection</span></span> | <span data-ttu-id="54c0f-p104">予定表グループ内の予定表。ナビゲーション プロパティ。読み取り専用です。Null 許容型。</span><span class="sxs-lookup"><span data-stu-id="54c0f-p104">The calendars in the calendar group. Navigation property. Read-only. Nullable.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="54c0f-159">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="54c0f-159">JSON representation</span></span>

<span data-ttu-id="54c0f-160">以下は、リソースの JSON 表記です</span><span class="sxs-lookup"><span data-stu-id="54c0f-160">Here is a JSON representation of the resource</span></span>

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
