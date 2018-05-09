# <a name="workinghours-resource-type"></a><span data-ttu-id="09778-101">workingHours リソースの種類</span><span class="sxs-lookup"><span data-stu-id="09778-101">workingHours resource type</span></span>

<span data-ttu-id="09778-102">ユーザーが働く曜日と、特定のタイムゾーンの時間を表します。</span><span class="sxs-lookup"><span data-stu-id="09778-102">Represents the days of the week and hours in a specific time zone that the user works.</span></span>

<span data-ttu-id="09778-103">アクティビティまたはリソースの計画に対処するシナリオでは、ユーザーの就業時間にアクセスできると便利です。</span><span class="sxs-lookup"><span data-stu-id="09778-103">Having access to a user's working hours is useful in scenarios that handle activity or resource planning.</span></span> <span data-ttu-id="09778-104">ユーザーの就業時間は、ユーザーの[メールボックス設定](mailboxSettings.md)の一部として[取得](../api/user_get_mailboxsettings.md#request-3)、[設定](../api/user_update_mailboxsettings.md#request-2)できます。</span><span class="sxs-lookup"><span data-stu-id="09778-104">You can [get](../api/user_get_mailboxsettings.md#request-3) and [set](../api/user_update_mailboxsettings.md#request-2) the working hours of a user as part of the user's [mailbox settings](mailboxSettings.md).</span></span> 

<span data-ttu-id="09778-105">就業時間には、Outlook クライアントに設定したタイム ゾーンとは異なるタイム ゾーンを設定できます。</span><span class="sxs-lookup"><span data-stu-id="09778-105">You can choose to set a time zone for your working hours differently from the time zone you have set on your Outlook client.</span></span> <span data-ttu-id="09778-106">これは、通常の勤務地とは異なるタイム ゾーンに移動する場合に役立ちます。</span><span class="sxs-lookup"><span data-stu-id="09778-106">This can be useful in cases like when you travel to a different time zone than you usually work in.</span></span> <span data-ttu-id="09778-107">Outlook クライアントを</span><span class="sxs-lookup"><span data-stu-id="09778-107">You can set the Outlook client</span></span>  
<span data-ttu-id="09778-108">移動先のタイム ゾーンに設定すると、現地にいる間、Outlook の時刻の値を現地時間で表示できます。</span><span class="sxs-lookup"><span data-stu-id="09778-108">to the destination time zone so that Outlook time values are displayed in local time while you are there.</span></span>
<span data-ttu-id="09778-109">他のユーザーが通常の勤務地での時間で会議を要求するとしても、該当するタイム ゾーンでの就業時間が考慮されます。</span><span class="sxs-lookup"><span data-stu-id="09778-109">When other people request work meetings with you in your usual place of work, they can still respect your working hours in the appropriate time zone.</span></span>


## <a name="properties"></a><span data-ttu-id="09778-110">プロパティ</span><span class="sxs-lookup"><span data-stu-id="09778-110">Properties</span></span>
| <span data-ttu-id="09778-111">プロパティ</span><span class="sxs-lookup"><span data-stu-id="09778-111">Property</span></span>     | <span data-ttu-id="09778-112">型</span><span class="sxs-lookup"><span data-stu-id="09778-112">Type</span></span>   |<span data-ttu-id="09778-113">説明</span><span class="sxs-lookup"><span data-stu-id="09778-113">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="09778-114">daysOfWeek</span><span class="sxs-lookup"><span data-stu-id="09778-114">daysOfWeek</span></span> | <span data-ttu-id="09778-115">String コレクション</span><span class="sxs-lookup"><span data-stu-id="09778-115">String collection</span></span> | <span data-ttu-id="09778-116">ユーザーが働く曜日。</span><span class="sxs-lookup"><span data-stu-id="09778-116">The days of the week on which the user works.</span></span> |
| <span data-ttu-id="09778-117">startTime</span><span class="sxs-lookup"><span data-stu-id="09778-117">StartTime</span></span> | <span data-ttu-id="09778-118">Edm.TimeOfDay</span><span class="sxs-lookup"><span data-stu-id="09778-118">Edm.TimeOfDay</span></span> | <span data-ttu-id="09778-119">ユーザーの始業時間。</span><span class="sxs-lookup"><span data-stu-id="09778-119">The time of the day that the user starts working.</span></span> |
| <span data-ttu-id="09778-120">endTime</span><span class="sxs-lookup"><span data-stu-id="09778-120">EndTime</span></span> | <span data-ttu-id="09778-121">Edm.TimeOfDay</span><span class="sxs-lookup"><span data-stu-id="09778-121">Edm.TimeOfDay</span></span> | <span data-ttu-id="09778-122">ユーザーの終業時間。</span><span class="sxs-lookup"><span data-stu-id="09778-122">The time of the day that the user stops working.</span></span> |
| <span data-ttu-id="09778-123">timeZone</span><span class="sxs-lookup"><span data-stu-id="09778-123">timeZone</span></span> | [<span data-ttu-id="09778-124">timeZoneBase</span><span class="sxs-lookup"><span data-stu-id="09778-124">timeZoneBase</span></span>](timezonebase.md) | <span data-ttu-id="09778-125">就業時間に適用するタイム ゾーン。</span><span class="sxs-lookup"><span data-stu-id="09778-125">The time zone to which the working hours apply.</span></span> |


## <a name="json-representation"></a><span data-ttu-id="09778-126">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="09778-126">JSON representation</span></span>

<span data-ttu-id="09778-127">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="09778-127">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.workingHours"
}-->

```json
{
  "daysOfWeek": ["string"],
  "startTime": "TimeOfDay",
  "endTime": "TimeOfDay",
  "timeZone": {"@odata.type": "microsoft.graph.timeZoneBase"}
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "workingHours resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->