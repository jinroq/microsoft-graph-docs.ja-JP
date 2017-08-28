# <a name="calendargroup-resource-type"></a><span data-ttu-id="2d464-101">calendarGroup リソースの種類</span><span class="sxs-lookup"><span data-stu-id="2d464-101">calendarGroup resource type</span></span>

<span data-ttu-id="2d464-102">予定表のグループです。</span><span class="sxs-lookup"><span data-stu-id="2d464-102">A group of calendars.</span></span>

<span data-ttu-id="2d464-p101">**注**： Outlook.com によってサポートされるのは、../me/calendars ショートカットでアクセス可能な既定の予定表グループのみです。その予定表グループを削除することはできません。</span><span class="sxs-lookup"><span data-stu-id="2d464-p101">**Note** Outlook.com supports only the default calendar group which is accessible by the ../me/calendars shortcut. You cannot delete that calendar group.</span></span>

## <a name="methods"></a><span data-ttu-id="2d464-105">メソッド</span><span class="sxs-lookup"><span data-stu-id="2d464-105">Methods</span></span>

| <span data-ttu-id="2d464-106">メソッド</span><span class="sxs-lookup"><span data-stu-id="2d464-106">Method</span></span>       | <span data-ttu-id="2d464-107">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="2d464-107">Return Type</span></span>  |<span data-ttu-id="2d464-108">説明</span><span class="sxs-lookup"><span data-stu-id="2d464-108">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="2d464-109">予定表グループを一覧表示する</span><span class="sxs-lookup"><span data-stu-id="2d464-109">List calendar groups</span></span>](../api/user_list_calendargroups.md) |<span data-ttu-id="2d464-110">[Calendar](calendar.md) collection</span><span class="sxs-lookup"><span data-stu-id="2d464-110">[Calendar](calendar.md) collection</span></span>| <span data-ttu-id="2d464-111">ユーザーの予定表グループを取得します。</span><span class="sxs-lookup"><span data-stu-id="2d464-111">Get the user's calendar groups.</span></span>|
|[<span data-ttu-id="2d464-112">予定表グループを作成する</span><span class="sxs-lookup"><span data-stu-id="2d464-112">Create calendar group</span></span>](../api/user_post_calendargroups.md) |[<span data-ttu-id="2d464-113">Calendar</span><span class="sxs-lookup"><span data-stu-id="2d464-113">Calendar</span></span>](calendar.md)| <span data-ttu-id="2d464-114">新しい予定表グループを作成します。</span><span class="sxs-lookup"><span data-stu-id="2d464-114">Create a new calendar group.</span></span>|
|[<span data-ttu-id="2d464-115">予定表グループを取得する</span><span class="sxs-lookup"><span data-stu-id="2d464-115">Get calendar group</span></span>](../api/calendargroup_get.md) | [<span data-ttu-id="2d464-116">calendarGroup</span><span class="sxs-lookup"><span data-stu-id="2d464-116">calendarGroup</span></span>](calendargroup.md) |<span data-ttu-id="2d464-117">予定表グループ オブジェクトのプロパティと関係を読み取ります。</span><span class="sxs-lookup"><span data-stu-id="2d464-117">Read properties and relationships of a calendar group object.</span></span>|
|[<span data-ttu-id="2d464-118">Update</span><span class="sxs-lookup"><span data-stu-id="2d464-118">Update</span></span>](../api/calendargroup_update.md) | [<span data-ttu-id="2d464-119">calendarGroup</span><span class="sxs-lookup"><span data-stu-id="2d464-119">calendarGroup</span></span>](calendargroup.md) |<span data-ttu-id="2d464-120">calendarGroup オブジェクトを更新します。</span><span class="sxs-lookup"><span data-stu-id="2d464-120">Update calendarGroup object.</span></span> |
|[<span data-ttu-id="2d464-121">Delete</span><span class="sxs-lookup"><span data-stu-id="2d464-121">Delete</span></span>](../api/calendargroup_delete.md) | <span data-ttu-id="2d464-122">なし</span><span class="sxs-lookup"><span data-stu-id="2d464-122">None</span></span> |<span data-ttu-id="2d464-123">calendarGroup オブジェクトを削除します。</span><span class="sxs-lookup"><span data-stu-id="2d464-123">Delete calendarGroup object.</span></span> |
|[<span data-ttu-id="2d464-124">予定表を一覧表示する</span><span class="sxs-lookup"><span data-stu-id="2d464-124">List calendars</span></span>](../api/calendargroup_list_calendars.md) |<span data-ttu-id="2d464-125">[Calendar](calendar.md) collection</span><span class="sxs-lookup"><span data-stu-id="2d464-125">[Calendar](calendar.md) collection</span></span>| <span data-ttu-id="2d464-126">予定表グループ内の予定表を一覧表示する</span><span class="sxs-lookup"><span data-stu-id="2d464-126">List calendars in a calendar group.</span></span>|
|[<span data-ttu-id="2d464-127">予定表を作成する</span><span class="sxs-lookup"><span data-stu-id="2d464-127">Create Calendar</span></span>](../api/calendargroup_post_calendars.md) |[<span data-ttu-id="2d464-128">Calendar</span><span class="sxs-lookup"><span data-stu-id="2d464-128">Calendar</span></span>](calendar.md)| <span data-ttu-id="2d464-129">予定表グループに新しい予定表を作成します。</span><span class="sxs-lookup"><span data-stu-id="2d464-129">Create a new Calendar in a calendar group.</span></span>|

## <a name="properties"></a><span data-ttu-id="2d464-130">プロパティ</span><span class="sxs-lookup"><span data-stu-id="2d464-130">Properties</span></span>
| <span data-ttu-id="2d464-131">プロパティ</span><span class="sxs-lookup"><span data-stu-id="2d464-131">Property</span></span>     | <span data-ttu-id="2d464-132">型</span><span class="sxs-lookup"><span data-stu-id="2d464-132">Type</span></span>   |<span data-ttu-id="2d464-133">説明</span><span class="sxs-lookup"><span data-stu-id="2d464-133">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="2d464-134">name</span><span class="sxs-lookup"><span data-stu-id="2d464-134">name</span></span>|<span data-ttu-id="2d464-135">String</span><span class="sxs-lookup"><span data-stu-id="2d464-135">String</span></span>|<span data-ttu-id="2d464-136">グループの名前。</span><span class="sxs-lookup"><span data-stu-id="2d464-136">The group name.</span></span>|
|<span data-ttu-id="2d464-137">changeKey</span><span class="sxs-lookup"><span data-stu-id="2d464-137">changeKey</span></span>|<span data-ttu-id="2d464-138">String</span><span class="sxs-lookup"><span data-stu-id="2d464-138">String</span></span>|<span data-ttu-id="2d464-p102">予定表グループのバージョンを識別します。予定表グループを変更するたびに ChangeKey も変更されます。これにより、Exchange は正しいバージョンのオブジェクトに変更を適用できます。読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="2d464-p102">Identifies the version of the calendar group. Every time the calendar group is changed, ChangeKey changes as well. This allows Exchange to apply changes to the correct version of the object. Read-only.</span></span>|
|<span data-ttu-id="2d464-143">classId</span><span class="sxs-lookup"><span data-stu-id="2d464-143">classId</span></span>|<span data-ttu-id="2d464-144">Guid</span><span class="sxs-lookup"><span data-stu-id="2d464-144">Guid</span></span>|<span data-ttu-id="2d464-p103">クラス識別子。読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="2d464-p103">The class identifier. Read-only.</span></span>|
|<span data-ttu-id="2d464-147">id</span><span class="sxs-lookup"><span data-stu-id="2d464-147">id</span></span>|<span data-ttu-id="2d464-148">String</span><span class="sxs-lookup"><span data-stu-id="2d464-148">String</span></span>|<span data-ttu-id="2d464-p104">グループの一意識別子。読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="2d464-p104">The group's unique identifier. Read-only.</span></span>|

## <a name="relationships"></a><span data-ttu-id="2d464-151">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="2d464-151">Relationships</span></span>
| <span data-ttu-id="2d464-152">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="2d464-152">Relationship</span></span> | <span data-ttu-id="2d464-153">型</span><span class="sxs-lookup"><span data-stu-id="2d464-153">Type</span></span>   |<span data-ttu-id="2d464-154">説明</span><span class="sxs-lookup"><span data-stu-id="2d464-154">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="2d464-155">予定表</span><span class="sxs-lookup"><span data-stu-id="2d464-155">calendars</span></span>|<span data-ttu-id="2d464-156">[Calendar](calendar.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="2d464-156">[Calendar](calendar.md) collection</span></span>|<span data-ttu-id="2d464-p105">予定表グループ内の予定表。ナビゲーション プロパティ。読み取り専用。Null 許容型。</span><span class="sxs-lookup"><span data-stu-id="2d464-p105">The calendars in the calendar group. Navigation property. Read-only. Nullable.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="2d464-161">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="2d464-161">JSON representation</span></span>

<span data-ttu-id="2d464-162">以下は、リソースの JSON 表記です</span><span class="sxs-lookup"><span data-stu-id="2d464-162">Here is a JSON representation of the resource</span></span>

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
