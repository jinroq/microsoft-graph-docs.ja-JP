---
title: ユーザーおよびリソース (プレビュー) のスケジュールの空き時間情報を取得します。
description: 作業または学校の設定では、一般的なシナリオは、ユーザーが会議の空きを確認したりすると、チーム、部屋、または期間内の機器の可用性を参照します。
ms.openlocfilehash: 8a2dd9318bdd806c99d525ee41f46d78d1963b47
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27092508"
---
# <a name="get-freebusy-schedule-of-users-and-resources-preview"></a><span data-ttu-id="e4bcb-103">ユーザーおよびリソース (プレビュー) のスケジュールの空き時間情報を取得します。</span><span class="sxs-lookup"><span data-stu-id="e4bcb-103">Get free/busy schedule of users and resources (preview)</span></span>

<span data-ttu-id="e4bcb-104">作業または学校の設定では、一般的なシナリオは、ユーザーが会議の空きを確認したりすると、チーム、部屋、または期間内の機器の可用性を参照します。</span><span class="sxs-lookup"><span data-stu-id="e4bcb-104">In a work or school setting, a common scenario is to see when a user is free for meeting, or to browse the availability of a team, room, or equipment for a time period.</span></span>

<span data-ttu-id="e4bcb-105">[GetSchedule](/graph/api/calendar-getschedule?view=graph-rest-beta)アクションでは、特定の期間の 1 つまたは複数のエンティティのユーザー、配布リスト、またはリソースの可用性情報を取得することができます。</span><span class="sxs-lookup"><span data-stu-id="e4bcb-105">The [getSchedule](/graph/api/calendar-getschedule?view=graph-rest-beta) action lets you get the availability information of one or more entities - users, distribution lists, or resources - for a specific period of time.</span></span> 

## <a name="example"></a><span data-ttu-id="e4bcb-106">例</span><span class="sxs-lookup"><span data-stu-id="e4bcb-106">Example</span></span>

<span data-ttu-id="e4bcb-107">Pacitfic 標準時午後 6 時までの 9 am からの特定の日に、アレックス、同僚の空き時間のスケジュールを検索する例を示します。</span><span class="sxs-lookup"><span data-stu-id="e4bcb-107">A simple example is to find the free/busy schedule of a coworker, Alex, on a specific day, from 9am to 6pm, Pacitfic Standard Time:</span></span>

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

<span data-ttu-id="e4bcb-108">**getSchedule**は、Alex の既存のイベントに一致する項目をスケジュール 2 を返します ' 既定の予定表、各イベントと、空き/予約済みの状態の開始と終了時刻を表示します。</span><span class="sxs-lookup"><span data-stu-id="e4bcb-108">**getSchedule** returns two schedule items that match existing events in Alex' default calendar, showing the start and end times of each event and its free/busy status.</span></span> <span data-ttu-id="e4bcb-109">Alex は、その日付と時刻の範囲内の残りの時間の空きを想定することができます。</span><span class="sxs-lookup"><span data-stu-id="e4bcb-109">You can assume Alex is free for the remaining time in that date/time range.</span></span>

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

<span data-ttu-id="e4bcb-110">スケジュールの空き時間情報、Alex の作業時間とは別**getSchedule**も返します**availabilityView**アレックスのマージされたビューには ' その日の可用性です。</span><span class="sxs-lookup"><span data-stu-id="e4bcb-110">Apart from the free/busy schedule and working hours of Alex, **getSchedule** also returns **availabilityView**, which is a merged view of Alex' availability for that day.</span></span> <span data-ttu-id="e4bcb-111">マージされたビューは、Alex を示す各タイム ・ スロットに、その日に対応する時間帯で構成される文字列 ' 次の規則を使用して可用性。</span><span class="sxs-lookup"><span data-stu-id="e4bcb-111">The merged view is a string that consists of time slots covering that day, with each time slot indicating Alex' availability using the following convention:</span></span> 

- <span data-ttu-id="e4bcb-112">`0`無料 =</span><span class="sxs-lookup"><span data-stu-id="e4bcb-112">`0`= free</span></span>
- <span data-ttu-id="e4bcb-113">`1`仮の予定 =</span><span class="sxs-lookup"><span data-stu-id="e4bcb-113">`1`= tentative</span></span>
- <span data-ttu-id="e4bcb-114">`2`= ビジー</span><span class="sxs-lookup"><span data-stu-id="e4bcb-114">`2`= busy</span></span>
- <span data-ttu-id="e4bcb-115">`3`外出 =</span><span class="sxs-lookup"><span data-stu-id="e4bcb-115">`3`= out of office</span></span>
- <span data-ttu-id="e4bcb-116">`4`他の場所で作業を = します。</span><span class="sxs-lookup"><span data-stu-id="e4bcb-116">`4`= working elsewhere.</span></span> 

<span data-ttu-id="e4bcb-117">既定では、各タイム ・ スロットの長さは、30 分です。</span><span class="sxs-lookup"><span data-stu-id="e4bcb-117">By default, the length of each time slot is 30 minutes.</span></span> <span data-ttu-id="e4bcb-118">この例では、15 分に時間帯をカスタマイズするのには**availabilityViewInterval**プロパティを使用します。</span><span class="sxs-lookup"><span data-stu-id="e4bcb-118">This example uses the **availabilityViewInterval** property to customize the time slot to be 15 minutes.</span></span>

## <a name="how-is-getschedule-different-from-findmeetingtimes"></a><span data-ttu-id="e4bcb-119">どのように getSchedule とは異なる findMeetingTimes です。</span><span class="sxs-lookup"><span data-stu-id="e4bcb-119">How is getSchedule different from findMeetingTimes</span></span>

<span data-ttu-id="e4bcb-120">[FindMeetingTimes](/graph/api/user-findmeetingtimes?view=graph-rest-1.0)アクションは、指定されたユーザーおよびリソースの作業時間と空き時間情報を読み取る両方という点で**getSchedule**に似ています。</span><span class="sxs-lookup"><span data-stu-id="e4bcb-120">The [findMeetingTimes](/graph/api/user-findmeetingtimes?view=graph-rest-1.0) action is similar to **getSchedule** in that both read the free/busy status and working hours of specified users and resources.</span></span> <span data-ttu-id="e4bcb-121">2 つのアクションは、いくつかの主要な方法が異なります。</span><span class="sxs-lookup"><span data-stu-id="e4bcb-121">The two actions differ in a few major ways.</span></span>

### <a name="application"></a><span data-ttu-id="e4bcb-122">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="e4bcb-122">Application</span></span>

<span data-ttu-id="e4bcb-123">**findMeetingTimes**には、次のように会議の時刻と場所を提案する特定のビジネス ロジックが適用されます。</span><span class="sxs-lookup"><span data-stu-id="e4bcb-123">**findMeetingTimes** applies certain business logic to suggest meeting times and locations, such as:</span></span>

- <span data-ttu-id="e4bcb-124">各エンティティのオプションまたは必須の出勤</span><span class="sxs-lookup"><span data-stu-id="e4bcb-124">Optional or mandatory attendance of each entity</span></span>
- <span data-ttu-id="e4bcb-125">1 日の時間の要求されたアクティビティの性質</span><span class="sxs-lookup"><span data-stu-id="e4bcb-125">The nature of the requested activity for the time of the day</span></span>
- <span data-ttu-id="e4bcb-126">会議のクォーラムに必要な最低限の参加</span><span class="sxs-lookup"><span data-stu-id="e4bcb-126">The minimum attendance required for a quorum for a meeting</span></span>

<span data-ttu-id="e4bcb-127">[予約を合理化すること](findmeetingtimes-example.md)に依存するシナリオに適しています。</span><span class="sxs-lookup"><span data-stu-id="e4bcb-127">It is appropriate for scenarios that depend on [streamlining appointment booking](findmeetingtimes-example.md).</span></span>

<span data-ttu-id="e4bcb-128">**getSchedule**は単に空き時間情報のステータスを返します既存のイベントで要求されたカレンダーの特定の期間のと tp がその時間内に残り時間を想定しています。</span><span class="sxs-lookup"><span data-stu-id="e4bcb-128">**getSchedule** simply returns the free/busy status of existing events in each of the requested calendars for a given time period, and assumes the remaining time in that time period tp be free.</span></span> <span data-ttu-id="e4bcb-129">さらにビジネス ロジックを適用するには、シナリオを完了するのにはこのデータを使用します。</span><span class="sxs-lookup"><span data-stu-id="e4bcb-129">You would then apply further business logic to make use of this data to complete your scenario.</span></span>

### <a name="app-only-support"></a><span data-ttu-id="e4bcb-130">アプリケーション専用のサポート</span><span class="sxs-lookup"><span data-stu-id="e4bcb-130">App-only support</span></span>

<span data-ttu-id="e4bcb-131">**findmeetingtimes**は、アプリケーションにサインインしているユーザーを必要とする委任のシナリオのみをサポートします。</span><span class="sxs-lookup"><span data-stu-id="e4bcb-131">**findmeetingtimes** supports only delegated scenarios which require a user to have signed in to the app.</span></span> <span data-ttu-id="e4bcb-132">アプリケーションでは、サインインしているユーザーがアクセスできるカレンダーのみでイベントを読み取ることができます。</span><span class="sxs-lookup"><span data-stu-id="e4bcb-132">The app can read events in only the calendars that the signed-in user can access.</span></span> <span data-ttu-id="e4bcb-133">これには、他のユーザーが委任するか、サインイン中のユーザーと共有の予定表が含まれます。</span><span class="sxs-lookup"><span data-stu-id="e4bcb-133">This can include calendars that other users have delegated or shared with the signed-in user.</span></span>

<span data-ttu-id="e4bcb-134">**getSchedule**には、委任とアプリ専用のシナリオがサポートされています。</span><span class="sxs-lookup"><span data-stu-id="e4bcb-134">**getSchedule** supports both delegated and app-only scenarios.</span></span> <span data-ttu-id="e4bcb-135">後者の場合、管理者にお客様がサインインしているユーザーがいない状態のすべての予定表にアクセスするアプリケーション同意します。</span><span class="sxs-lookup"><span data-stu-id="e4bcb-135">In the latter, an administrator consents the app to access all calendars without a signed-in user.</span></span>


### <a name="version-support"></a><span data-ttu-id="e4bcb-136">バージョンのサポート</span><span class="sxs-lookup"><span data-stu-id="e4bcb-136">Version support</span></span>

<span data-ttu-id="e4bcb-137">**findmeetingtimes**は、すべてのアプリケーションで一般的に使用できます。</span><span class="sxs-lookup"><span data-stu-id="e4bcb-137">**findmeetingtimes** is generally available for all apps.</span></span> 

<span data-ttu-id="e4bcb-138">**getSchedule**は現在利用可能な[プレビューの状態で](versioning-and-support.md#beta-version)、したがって運用アプリケーションで使用するために適切ではありません。</span><span class="sxs-lookup"><span data-stu-id="e4bcb-138">**getSchedule** is currently available [in preview status](versioning-and-support.md#beta-version), and therefore is not appropriate for use in production apps.</span></span>


## <a name="permissions"></a><span data-ttu-id="e4bcb-139">Permissions</span><span class="sxs-lookup"><span data-stu-id="e4bcb-139">Permissions</span></span>
<span data-ttu-id="e4bcb-140">空き時間情報を取得する必要が最低限の特権のアクセス許可は、Calendar.Read です。</span><span class="sxs-lookup"><span data-stu-id="e4bcb-140">The least privileged permission you need to get free/busy information is Calendar.Read.</span></span> <span data-ttu-id="e4bcb-141">アプリケーション シナリオによっては、これはサインインしているユーザーまたは管理者によって同意ことができます。</span><span class="sxs-lookup"><span data-stu-id="e4bcb-141">Depending on your app scenario, this can be consented by the signed-in user or administrator.</span></span>
<span data-ttu-id="e4bcb-142">以外の空き時間情報のステータスと稼働時間の要求のエンティティを**getSchedule**を返すことも、件名と場所を提供する、イベントの。</span><span class="sxs-lookup"><span data-stu-id="e4bcb-142">Other than the free/busy status and working hours of requested entities, **getSchedule** can also return the subject and location of an event, provided that:</span></span>

- <span data-ttu-id="e4bcb-143">イベントが [低] 感度のレベルが付いている場合`normal`または`personal`し、次の条件の 1 つ以上を適用します。</span><span class="sxs-lookup"><span data-stu-id="e4bcb-143">If the event is marked with low sensitivity level - `normal` or `personal` AND one or more of the following conditions applies:</span></span>

- <span data-ttu-id="e4bcb-144">要求されたユーザーの予定表の設定は、タイトルや場所を表示するのには組織内のすべてのユーザーを許可します。</span><span class="sxs-lookup"><span data-stu-id="e4bcb-144">The requested user’s calendar settings allow all the users in the organization to view titles and locations</span></span>
- <span data-ttu-id="e4bcb-145">要求されたユーザーの予定表は、サインイン中のユーザーと共有します。</span><span class="sxs-lookup"><span data-stu-id="e4bcb-145">The requested user’s calendar is shared with the signed-in user</span></span>
- <span data-ttu-id="e4bcb-146">サインイン中のユーザーは、要求されたユーザーと同じ組織の管理者です。</span><span class="sxs-lookup"><span data-stu-id="e4bcb-146">The signed-in user is an administrator of the same organization as the requested user.</span></span>

## <a name="time-zone-representation"></a><span data-ttu-id="e4bcb-147">タイム ゾーン表現</span><span class="sxs-lookup"><span data-stu-id="e4bcb-147">Time zone representation</span></span>
<span data-ttu-id="e4bcb-148">既定では、返されたスケジュール項目の開始と終了時刻が UTC で表されます。</span><span class="sxs-lookup"><span data-stu-id="e4bcb-148">By default, the start and end times of the returned schedule items are represented in UTC.</span></span> <span data-ttu-id="e4bcb-149">使用することができます、 `Prefer` 、アプリの適切なタイム ゾーンを指定するヘッダー。</span><span class="sxs-lookup"><span data-stu-id="e4bcb-149">You can use a `Prefer` header to specify a time zone appropriate for your app.</span></span> <span data-ttu-id="e4bcb-150">例: </span><span class="sxs-lookup"><span data-stu-id="e4bcb-150">As an example:</span></span> 
```
Prefer: outlook.timezone="Pacific Standard Time"
```

## <a name="limits-and-error-conditions"></a><span data-ttu-id="e4bcb-151">制限値とエラー条件</span><span class="sxs-lookup"><span data-stu-id="e4bcb-151">Limits and error conditions</span></span>
<span data-ttu-id="e4bcb-152">次の制限およびエラー条件に注意します。</span><span class="sxs-lookup"><span data-stu-id="e4bcb-152">Be aware of the following limits and error condition:</span></span>

- <span data-ttu-id="e4bcb-153">**getSchedule**では、空き時間情報を最大 20 個のエンティティを一度に検索をサポートできます。</span><span class="sxs-lookup"><span data-stu-id="e4bcb-153">**getSchedule** can support looking up free/busy information for up to 20 entities at once.</span></span> <span data-ttu-id="e4bcb-154">この制限は、個別に、または配布リストのメンバーとして識別されるユーザーの数にしても、リソースの数に適用されます。</span><span class="sxs-lookup"><span data-stu-id="e4bcb-154">This limit applies to the number of users identified individually or as members of a distribution list, and to the number of resources as well.</span></span>
- <span data-ttu-id="e4bcb-155">検索するまでの時間は 42 日未満である必要があります。</span><span class="sxs-lookup"><span data-stu-id="e4bcb-155">The time period to look up must be less than 42 days.</span></span>
- <span data-ttu-id="e4bcb-156">**GetSchedule**は、指定したユーザーまたはリソースを識別できない場合、1 つのスケジュール項目を返し、エラーを示します。</span><span class="sxs-lookup"><span data-stu-id="e4bcb-156">If **getSchedule** cannot identify a specified user or resource, it returns a single schedule item and indicates the error.</span></span> 

## <a name="see-also"></a><span data-ttu-id="e4bcb-157">関連項目</span><span class="sxs-lookup"><span data-stu-id="e4bcb-157">See also</span></span>
- [<span data-ttu-id="e4bcb-158">アクセス許可を参照します。</span><span class="sxs-lookup"><span data-stu-id="e4bcb-158">Permissions reference</span></span>](permissions-reference.md#calendars-permissions)
- [<span data-ttu-id="e4bcb-159">開催可能な会議日時を Outlook カレンダーで検索する</span><span class="sxs-lookup"><span data-stu-id="e4bcb-159">Find possible meeting times on the Outlook calendar</span></span>](findmeetingtimes-example.md)
