# <a name="get-freebusy-schedule-of-users-and-resources-preview"></a><span data-ttu-id="f4633-101">ユーザーおよびリソースのスケジュールの空き時間情報を取得する (プレビュー)</span><span class="sxs-lookup"><span data-stu-id="f4633-101">Get free/busy schedule for users and resources (preview)</span></span>

<span data-ttu-id="f4633-102">作業または学校の設定では、一般的なシナリオは、ユーザーが会議の空きを確認したりすると、チーム、部屋、または期間内の機器の可用性を参照します。</span><span class="sxs-lookup"><span data-stu-id="f4633-102">In a work or school setting, a common scenario is to see when a user is free for meeting, or to browse the availability of a team, room, or equipment for a time period.</span></span>

<span data-ttu-id="f4633-103">[GetSchedule](../api-reference/beta/api/calendar_getschedule.md) アクションでは、特定の期間の 1 つまたは複数のエンティティのユーザー、配布リスト、またはリソースの可用性情報を取得することができます。</span><span class="sxs-lookup"><span data-stu-id="f4633-103">The [getSchedule](../api-reference/beta/api/calendar_getschedule.md) action lets you get the availability information of one or more entities - users, distribution lists, or resources - for a specific period of time.</span></span> 

## <a name="example"></a><span data-ttu-id="f4633-104">例</span><span class="sxs-lookup"><span data-stu-id="f4633-104">Example</span></span>

<span data-ttu-id="f4633-105">太平洋標準時午前9から午後 6 時までの特定の日に、同僚アレックスの空き時間のスケジュールを検索する例を示します。</span><span class="sxs-lookup"><span data-stu-id="f4633-105">A simple example is to find the free/busy schedule of a coworker, Alex, on a specific day, from 9am to 6pm, Pacitfic Standard Time:</span></span>

<!-- {
  "blockType": "ignored",
  "name": "calendar_getSchedule_concept"
}-->
```http
POST https://graph.microsoft.com/beta/me/calendar/getschedule 
Prefer: outlook.timezone="Pacific Standard Time"
Content-Type: application/json

{        
    "Schedules": ["AlexW@contoso.OnMicrosoft.com"],
    "StartTime": {
        "dateTime": "2018-08-06T09:00:00",
        "timeZone": "Pacific Standard Time"
    },
    "EndTime": {
        "dateTime": "2018-08-06T18:00:00",
        "timeZone": "Pacific Standard Time"
    },
    "availabilityViewInterval": "15"
}
```

<span data-ttu-id="f4633-106">**getSchedule** は、アレックスの既存のイベントに一致する項目をスケジュール 2 を返します ' 既定の予定表、各イベントと、空き/予約済みの状態の開始と終了時刻を表示します。</span><span class="sxs-lookup"><span data-stu-id="f4633-106">**getSchedule** returns two schedule items that match existing events in Alex' default calendar, showing the start and end times of each event and its free/busy status.</span></span> <span data-ttu-id="f4633-107">アレックスは、その日付と時刻の範囲内の残りの時間が空いていることを想定できます。</span><span class="sxs-lookup"><span data-stu-id="f4633-107">You can assume Alex is free for the remaining time in that date/time range.</span></span>

<!-- {
  "blockType": "ignored",
  "truncated": true,
  "@odata.type": "microsoft.graph.scheduleInformation",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "@odata.context":"https://graph.microsoft.com/beta/$metadata#Collection(microsoft.graph.scheduleInformation)",
    "value":[
        {
            "scheduleId":"AlexW@contoso.OnMicrosoft.com",
            "availabilityView":"111111002222222200000000000000000000",
            "scheduleItems":[
                {
                    "isPrivate":false,
                    "status":"Tentative",
                    "start":{
                        "dateTime":"2018-08-06T09:00:00.0000000",
                        "timeZone":"Pacific Standard Time"
                    },
                    "end":{
                        "dateTime":"2018-08-06T10:30:00.0000000",
                        "timeZone":"Pacific Standard Time"
                    }
                },
                {
                    "isPrivate":false,
                    "status":"Busy",
                    "start":{
                        "dateTime":"2018-08-06T11:00:00.0000000",
                        "timeZone":"Pacific Standard Time"
                    },
                    "end":{
                        "dateTime":"2018-08-06T13:00:00.0000000",
                        "timeZone":"Pacific Standard Time"
                    }
                }
            ],
            "workingHours":{
                "daysOfWeek":[
                    "monday",
                    "tuesday",
                    "wednesday",
                    "thursday",
                    "friday"
                ],
                "startTime":"08:00:00.0000000",
                "endTime":"17:00:00.0000000",
                "timeZone":{
                    "@odata.type":"#microsoft.graph.customTimeZone",
                    "bias":480,
                    "name":"Customized Time Zone",
                    "standardOffset":{
                        "time":"02:00:00.0000000",
                        "dayOccurrence":1,
                        "dayOfWeek":"sunday",
                        "month":11,
                        "year":0
                    },
                    "daylightOffset":{
                        "daylightBias":-60,
                        "time":"02:00:00.0000000",
                        "dayOccurrence":2,
                        "dayOfWeek":"sunday",
                        "month":3,
                        "year":0
                    }
                }
            }
        }
    ]
}

```

<span data-ttu-id="f4633-108">アレックスのスケジュールの空き時間情報と作業時間とは別 **getSchedule** も返します **availabilityView**アレックスのマージされたビューには ' その日の可用性です。</span><span class="sxs-lookup"><span data-stu-id="f4633-108">Apart from the free/busy schedule and working hours of Alex, **getSchedule** also returns **availabilityView**, which is a merged view of Alex' availability for that day.</span></span> <span data-ttu-id="f4633-109">マージされたビューは、その日をカバーするタイムスロットで構成された文字列であり、各タイムスロットは次の規則を使用してアレックスの可用性を示します。</span><span class="sxs-lookup"><span data-stu-id="f4633-109">The merged view is a string that consists of time slots covering that day, with each time slot indicating Alex' availability using the following convention:</span></span> 

- <span data-ttu-id="f4633-110">`0`自由</span><span class="sxs-lookup"><span data-stu-id="f4633-110">`0`= free</span></span>
- <span data-ttu-id="f4633-111">`1`仮</span><span class="sxs-lookup"><span data-stu-id="f4633-111">`1`= tentative</span></span>
- <span data-ttu-id="f4633-112">`2`多忙</span><span class="sxs-lookup"><span data-stu-id="f4633-112">`2`= busy</span></span>
- <span data-ttu-id="f4633-113">`3`外出中</span><span class="sxs-lookup"><span data-stu-id="f4633-113">`3`= out of office</span></span>
- <span data-ttu-id="f4633-114">`4`他の場所で働いています。</span><span class="sxs-lookup"><span data-stu-id="f4633-114">`4`= working elsewhere.</span></span> 

<span data-ttu-id="f4633-115">既定では、各タイム スロットの長さは 30 分です。</span><span class="sxs-lookup"><span data-stu-id="f4633-115">Specifies the length of each time slot in minutes. Default is 30 minutes.</span></span> <span data-ttu-id="f4633-116">この例では、15 分に時間帯をカスタマイズするのには **availabilityViewInterval** プロパティを使用します。</span><span class="sxs-lookup"><span data-stu-id="f4633-116">This example uses the **availabilityViewInterval** property to customize the time slot to be 15 minutes.</span></span>

## <a name="how-is-getschedule-different-from-findmeetingtimes"></a><span data-ttu-id="f4633-117">getScheduleとfindMeetingTimesの違い</span><span class="sxs-lookup"><span data-stu-id="f4633-117">How is getSchedule different from findMeetingTimes</span></span>

<span data-ttu-id="f4633-118">[FindMeetingTimes](../api-reference/v1.0/api/user_findmeetingtimes.md) アクションは、指定されたユーザーおよびリソースの作業時間と空き時間情報を読み取る両方という点で **getSchedule** に似ています。</span><span class="sxs-lookup"><span data-stu-id="f4633-118">The [findMeetingTimes](../api-reference/v1.0/api/user_findmeetingtimes.md) action is similar to **getSchedule** in that both read the free/busy status and working hours of specified users and resources.</span></span> <span data-ttu-id="f4633-119">2 つのアクションは、いくつかの主要な点で異なります。</span><span class="sxs-lookup"><span data-stu-id="f4633-119">The two actions differ in a few major ways.</span></span>

### <a name="application"></a><span data-ttu-id="f4633-120">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="f4633-120">Application</span></span>

<span data-ttu-id="f4633-121">**findMeetingTimes** には、次のように会議の時刻と場所を提案する特定のビジネス ロジックが適用されます。</span><span class="sxs-lookup"><span data-stu-id="f4633-121">**findMeetingTimes** applies certain business logic to suggest meeting times and locations, such as:</span></span>

- <span data-ttu-id="f4633-122">各エンティティのオプションまたは強制出勤</span><span class="sxs-lookup"><span data-stu-id="f4633-122">Optional or mandatory attendance of each entity</span></span>
- <span data-ttu-id="f4633-123">1 日の時間の要求されたアクティビティの性質</span><span class="sxs-lookup"><span data-stu-id="f4633-123">The nature of the requested activity for the time of the day</span></span>
- <span data-ttu-id="f4633-124">会議のクォーラムに必要な最低限の参加</span><span class="sxs-lookup"><span data-stu-id="f4633-124">The minimum attendance required for a quorum for a meeting</span></span>

<span data-ttu-id="f4633-125">[予約を合理化すること](findmeetingtimes_example.md)に依存するシナリオに適しています。</span><span class="sxs-lookup"><span data-stu-id="f4633-125">It is appropriate for scenarios that depend on [streamlining appointment booking](findmeetingtimes_example.md).</span></span>

<span data-ttu-id="f4633-126">**getSchedule** は単に空き時間情報のステータスを返します既存のイベントで要求されたカレンダーの特定の期間のと tp がその時間内に残り時間を想定しています。</span><span class="sxs-lookup"><span data-stu-id="f4633-126">**getSchedule** simply returns the free/busy status of existing events in each of the requested calendars for a given time period, and assumes the remaining time in that time period tp be free.</span></span> <span data-ttu-id="f4633-127">さらにビジネス ロジックを適用するには、シナリオを完了するのにはこのデータを使用します。</span><span class="sxs-lookup"><span data-stu-id="f4633-127">You would then apply further business logic to make use of this data to complete your scenario.</span></span>

### <a name="app-only-support"></a><span data-ttu-id="f4633-128">アプリ専用のサポート</span><span class="sxs-lookup"><span data-stu-id="f4633-128">App-only support</span></span>

<span data-ttu-id="f4633-129">**findmeetingtimes** は、アプリにサインインしているユーザーを必要とする委任のシナリオのみをサポートします。</span><span class="sxs-lookup"><span data-stu-id="f4633-129">**findmeetingtimes** supports only delegated scenarios which require a user to have signed in to the app.</span></span> <span data-ttu-id="f4633-130">アプリでは、サインインしているユーザーがアクセスできるカレンダーのみでイベントを読み取ることができます。</span><span class="sxs-lookup"><span data-stu-id="f4633-130">The app can read events in only the calendars that the signed-in user can access.</span></span> <span data-ttu-id="f4633-131">これには、他のユーザーが委任するか、サインイン中のユーザーと共有の予定表が含まれます。</span><span class="sxs-lookup"><span data-stu-id="f4633-131">This can include calendars that other users have delegated or shared with the signed-in user.</span></span>

<span data-ttu-id="f4633-132">**getSchedule** には、委任とアプリ専用のシナリオがサポートされています。</span><span class="sxs-lookup"><span data-stu-id="f4633-132">**getSchedule** supports both delegated and app-only scenarios.</span></span> <span data-ttu-id="f4633-133">後者の場合、管理者は、ログインしていないユーザーがいないすべてのカレンダーにアクセスするようにアプリに同意します。</span><span class="sxs-lookup"><span data-stu-id="f4633-133">In the latter, an administrator consents the app to access all calendars without a signed-in user.</span></span>


### <a name="version-support"></a><span data-ttu-id="f4633-134">バージョンのサポート</span><span class="sxs-lookup"><span data-stu-id="f4633-134">Version support</span></span>

<span data-ttu-id="f4633-135">**findmeetingtimes** は、すべてのアプリで一般的に使用できます。</span><span class="sxs-lookup"><span data-stu-id="f4633-135">**findmeetingtimes** is generally available for all apps.</span></span> 

<span data-ttu-id="f4633-136">**getSchedule** は現在利用可能な [プレビューの状態で](versioning_and_support.md#beta-version)、したがって運用アプリで使用するために適切ではありません。</span><span class="sxs-lookup"><span data-stu-id="f4633-136">**getSchedule** is currently available [in preview status](versioning_and_support.md#beta-version), and therefore is not appropriate for use in production apps.</span></span>


## <a name="permissions"></a><span data-ttu-id="f4633-137">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="f4633-137">Permissions</span></span>
<span data-ttu-id="f4633-138">空き時間情報を取得するために必要な最小特権は、Calendar.Readです。</span><span class="sxs-lookup"><span data-stu-id="f4633-138">The least privileged permission you need to get free/busy information is Calendar.Read.</span></span> <span data-ttu-id="f4633-139">アプリのシナリオによっては、ログインしているユーザーまたは管理者が同意することができます。</span><span class="sxs-lookup"><span data-stu-id="f4633-139">Depending on your app scenario, this can be consented by the signed-in user or administrator.</span></span>
<span data-ttu-id="f4633-140">getSchedule は、要求されたエンティティの空き時間や勤務時間以外にも、イベントの件名と場所を返すことができます。\*\*\*\*</span><span class="sxs-lookup"><span data-stu-id="f4633-140">Other than the free/busy status and working hours of requested entities, **getSchedule** can also return the subject and location of an event, provided that:</span></span>

- <span data-ttu-id="f4633-141">イベントが [低] 感度のレベルが付いている場合 `normal` または `personal` し、次の条件の 1 つ以上を適用します。</span><span class="sxs-lookup"><span data-stu-id="f4633-141">If the event is marked with low sensitivity level - `normal` or `personal` AND one or more of the following conditions applies:</span></span>

- <span data-ttu-id="f4633-142">要求されたユーザーのカレンダー設定では、組織内のすべてのユーザーがタイトルと場所を表示できます</span><span class="sxs-lookup"><span data-stu-id="f4633-142">The requested user’s calendar settings allow all the users in the organization to view titles and locations</span></span>
- <span data-ttu-id="f4633-143">要求されたユーザーの予定表は、サインイン中のユーザーと共有します。</span><span class="sxs-lookup"><span data-stu-id="f4633-143">The requested user’s calendar is shared with the signed-in user</span></span>
- <span data-ttu-id="f4633-144">ログインしているユーザーは、要求されたユーザーと同じ組織の管理者です。</span><span class="sxs-lookup"><span data-stu-id="f4633-144">The signed-in user is an administrator of the same organization as the requested user.</span></span>

## <a name="time-zone-representation"></a><span data-ttu-id="f4633-145">タイム ゾーン表現</span><span class="sxs-lookup"><span data-stu-id="f4633-145">Time zone representation</span></span>
<span data-ttu-id="f4633-146">既定では、返されたスケジュール項目の開始と終了時刻が UTC で表されます。</span><span class="sxs-lookup"><span data-stu-id="f4633-146">By default, the start and end times of the returned schedule items are represented in UTC.</span></span> <span data-ttu-id="f4633-147">ヘッダーを使用して、アプリに適したタイムゾーンを指定することができます。`Prefer`</span><span class="sxs-lookup"><span data-stu-id="f4633-147">You can use a `Prefer` header to specify a time zone appropriate for your app.</span></span> <span data-ttu-id="f4633-148">例:</span><span class="sxs-lookup"><span data-stu-id="f4633-148">As an example:</span></span> 
```
Prefer: outlook.timezone="Pacific Standard Time"
```

## <a name="limits-and-error-conditions"></a><span data-ttu-id="f4633-149">制限値とエラー条件</span><span class="sxs-lookup"><span data-stu-id="f4633-149">Limits and error conditions</span></span>
<span data-ttu-id="f4633-150">次の制限とエラー状態に注意してください。</span><span class="sxs-lookup"><span data-stu-id="f4633-150">Be aware of the following limits and error condition:</span></span>

- <span data-ttu-id="f4633-151">**getSchedule** では、空き時間情報を最大 20 個のエンティティを一度に検索をサポートできます。</span><span class="sxs-lookup"><span data-stu-id="f4633-151">**getSchedule** can support looking up free/busy information for up to 20 entities at once.</span></span> <span data-ttu-id="f4633-152">この制限は、個々にまたは配布リストのメンバーとして識別されたユーザー数、およびリソース数にも適用されます。</span><span class="sxs-lookup"><span data-stu-id="f4633-152">This limit applies to the number of users identified individually or as members of a distribution list, and to the number of resources as well.</span></span>
- <span data-ttu-id="f4633-153">検索するまでの時間は 42 日未満である必要があります。</span><span class="sxs-lookup"><span data-stu-id="f4633-153">The time period to look up must be less than 42 days.</span></span>
- <span data-ttu-id="f4633-154">**GetSchedule** は、指定したユーザーまたはリソースを識別できない場合、1 つのスケジュール項目を返し、エラーを示します。</span><span class="sxs-lookup"><span data-stu-id="f4633-154">If **getSchedule** cannot identify a specified user or resource, it returns a single schedule item and indicates the error.</span></span> 

## <a name="see-also"></a><span data-ttu-id="f4633-155">関連項目</span><span class="sxs-lookup"><span data-stu-id="f4633-155">See also</span></span>
- [<span data-ttu-id="f4633-156">アクセス許可の参照</span><span class="sxs-lookup"><span data-stu-id="f4633-156">Permissions reference</span></span>](permissions_reference.md#calendars-permissions)
- [<span data-ttu-id="f4633-157">開催可能な会議日時を Outlook カレンダーで検索する</span><span class="sxs-lookup"><span data-stu-id="f4633-157">Find possible meeting times on the Outlook calendar</span></span>](findmeetingtimes_example.md)
