---
title: ユーザーとリソースの空き時間スケジュールを取得する (プレビュー)
description: 職場または学校の環境で一般的なシナリオとして、ユーザーが会議に出席できる時間を確認する場合や、ある期間内にチーム、部屋、または備品の空き時間情報を参照する場合があります。
ms.openlocfilehash: 8a2dd9318bdd806c99d525ee41f46d78d1963b47
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27092508"
---
# <a name="get-freebusy-schedule-of-users-and-resources-preview"></a><span data-ttu-id="43bfa-103">ユーザーとリソースの空き時間スケジュールを取得する (プレビュー)</span><span class="sxs-lookup"><span data-stu-id="43bfa-103">Get free/busy schedule of users and resources (preview)</span></span>

<span data-ttu-id="43bfa-104">職場または学校の環境で一般的なシナリオとして、ユーザーが会議に出席できる時間を確認する場合や、ある期間内にチーム、部屋、または備品の空き時間情報を参照する場合があります。</span><span class="sxs-lookup"><span data-stu-id="43bfa-104">In a work or school setting, a common scenario is to see when a user is free for meeting, or to browse the availability of a team, room, or equipment for a time period.</span></span>

<span data-ttu-id="43bfa-105">[getSchedule](/graph/api/calendar-getschedule?view=graph-rest-beta) アクションを使用すると、特定の期間について 1 つ以上のエンティティ (ユーザー、配布リスト、またはリソース) の空き時間情報を取得できます。</span><span class="sxs-lookup"><span data-stu-id="43bfa-105">The [getSchedule](/graph/api/calendar-getschedule?view=graph-rest-beta) action lets you get the availability information of one or more entities - users, distribution lists, or resources - for a specific period of time.</span></span> 

## <a name="example"></a><span data-ttu-id="43bfa-106">例</span><span class="sxs-lookup"><span data-stu-id="43bfa-106">Example</span></span>

<span data-ttu-id="43bfa-107">特定の日の午前 9 時から午後 6 時 (太平洋標準時) までの同僚の Alex の空き時間スケジュールを検索する簡単な例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="43bfa-107">A simple example is to find the free/busy schedule of a coworker, Alex, on a specific day, from 9am to 6pm, Pacitfic Standard Time:</span></span>

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

<span data-ttu-id="43bfa-108">**getSchedule** は、Alex の既定の予定表にある既存のイベントと一致する 2 つのスケジュール項目を返します。これで、各イベントの開始時刻と終了時刻と、その空き時間状態がわかります。</span><span class="sxs-lookup"><span data-stu-id="43bfa-108">**getSchedule** returns two schedule items that match existing events in Alex' default calendar, showing the start and end times of each event and its free/busy status.</span></span> <span data-ttu-id="43bfa-109">その日付/時刻の範囲内で、残りの時間は Alex が空いていると考えることができます。</span><span class="sxs-lookup"><span data-stu-id="43bfa-109">You can assume Alex is free for the remaining time in that date/time range.</span></span>

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

<span data-ttu-id="43bfa-110">Alex の空き時間スケジュールと勤務時間以外に、**getSchedule** は **availabilityView** も返します。これは、その日の Alex の空き時間情報の結合されたビューです。</span><span class="sxs-lookup"><span data-stu-id="43bfa-110">Apart from the free/busy schedule and working hours of Alex, **getSchedule** also returns **availabilityView**, which is a merged view of Alex' availability for that day.</span></span> <span data-ttu-id="43bfa-111">結合されたビューは、その日を対象とする時間帯で構成された文字列であり、各時間帯は次の規則を使用して Alex の空き時間情報を示します。</span><span class="sxs-lookup"><span data-stu-id="43bfa-111">The merged view is a string that consists of time slots covering that day, with each time slot indicating Alex' availability using the following convention:</span></span> 

- <span data-ttu-id="43bfa-112">`0`= 空き時間</span><span class="sxs-lookup"><span data-stu-id="43bfa-112">`0`= free</span></span>
- <span data-ttu-id="43bfa-113">`1`= 仮の予定</span><span class="sxs-lookup"><span data-stu-id="43bfa-113">`1`= tentative</span></span>
- <span data-ttu-id="43bfa-114">`2`= ビジー</span><span class="sxs-lookup"><span data-stu-id="43bfa-114">`2`= busy</span></span>
- <span data-ttu-id="43bfa-115">`3`= 外出中</span><span class="sxs-lookup"><span data-stu-id="43bfa-115">`3`= out of office</span></span>
- <span data-ttu-id="43bfa-116">`4`= 別の場所で作業。</span><span class="sxs-lookup"><span data-stu-id="43bfa-116">`4`= working elsewhere.</span></span> 

<span data-ttu-id="43bfa-117">既定では、各時間帯の長さは 30 分です。</span><span class="sxs-lookup"><span data-stu-id="43bfa-117">Specifies the length of each time slot in minutes. Default is 30 minutes.</span></span> <span data-ttu-id="43bfa-118">この例では、**availabilityViewInterval** プロパティを使用して時間帯を 15 分にカスタマイズしています。</span><span class="sxs-lookup"><span data-stu-id="43bfa-118">This example uses the **availabilityViewInterval** property to customize the time slot to be 15 minutes.</span></span>

## <a name="how-is-getschedule-different-from-findmeetingtimes"></a><span data-ttu-id="43bfa-119">getSchedule と findMeetingTimes の違い</span><span class="sxs-lookup"><span data-stu-id="43bfa-119">How is getSchedule different from findMeetingTimes</span></span>

<span data-ttu-id="43bfa-120">[findMeetingTimes](/graph/api/user-findmeetingtimes?view=graph-rest-1.0) アクションは、指定されたユーザーとリソースの空き時間情報と稼働時間を両方読み取るという点で **getSchedule** と似ています。</span><span class="sxs-lookup"><span data-stu-id="43bfa-120">The [findMeetingTimes](/graph/api/user-findmeetingtimes?view=graph-rest-1.0) action is similar to **getSchedule** in that both read the free/busy status and working hours of specified users and resources.</span></span> <span data-ttu-id="43bfa-121">2 つのアクションは、いくつかの主要な点で異なります。</span><span class="sxs-lookup"><span data-stu-id="43bfa-121">The two actions differ in a few major ways.</span></span>

### <a name="application"></a><span data-ttu-id="43bfa-122">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="43bfa-122">Application</span></span>

<span data-ttu-id="43bfa-123">**findMeetingTimes** は、特定のビジネス ロジックを適用して、次のような会議の時間と場所を提案します。</span><span class="sxs-lookup"><span data-stu-id="43bfa-123">**findMeetingTimes** applies certain business logic to suggest meeting times and locations, such as:</span></span>

- <span data-ttu-id="43bfa-124">各エンティティの任意または必須の出席</span><span class="sxs-lookup"><span data-stu-id="43bfa-124">Optional or mandatory attendance of each entity</span></span>
- <span data-ttu-id="43bfa-125">その日の時刻について要求されたアクティビティの性質</span><span class="sxs-lookup"><span data-stu-id="43bfa-125">The nature of the requested activity for the time of the day</span></span>
- <span data-ttu-id="43bfa-126">会議のクォーラムに必要な最低限の出席者</span><span class="sxs-lookup"><span data-stu-id="43bfa-126">The minimum attendance required for a quorum for a meeting</span></span>

<span data-ttu-id="43bfa-127">[予定の予約の合理化](findmeetingtimes-example.md)に依存するシナリオに適しています。</span><span class="sxs-lookup"><span data-stu-id="43bfa-127">It is appropriate for scenarios that depend on [streamlining appointment booking](findmeetingtimes-example.md).</span></span>

<span data-ttu-id="43bfa-128">**getSchedule** では、要求された各予定表の指定された期間の中で、既存のイベントの空き時間情報が単純に返され、その期間の残りの時間は空き時間と見なされます。</span><span class="sxs-lookup"><span data-stu-id="43bfa-128">**getSchedule** simply returns the free/busy status of existing events in each of the requested calendars for a given time period, and assumes the remaining time in that time period tp be free.</span></span> <span data-ttu-id="43bfa-129">シナリオを完了するには、このデータを利用するビジネス ロジックをさらに適用します。</span><span class="sxs-lookup"><span data-stu-id="43bfa-129">You would then apply further business logic to make use of this data to complete your scenario.</span></span>

### <a name="app-only-support"></a><span data-ttu-id="43bfa-130">アプリ専用のサポート</span><span class="sxs-lookup"><span data-stu-id="43bfa-130">App-only support</span></span>

<span data-ttu-id="43bfa-131">**findmeetingtimes** は、ユーザーがアプリにサインインしている必要がある委任シナリオのみをサポートしています。</span><span class="sxs-lookup"><span data-stu-id="43bfa-131">**findmeetingtimes** supports only delegated scenarios which require a user to have signed in to the app.</span></span> <span data-ttu-id="43bfa-132">このアプリで読み取ることができるのは、サインインしているユーザーがアクセスできる予定表のイベントのみです。</span><span class="sxs-lookup"><span data-stu-id="43bfa-132">The app can read events in only the calendars that the signed-in user can access.</span></span> <span data-ttu-id="43bfa-133">これには、他のユーザーから委任された予定表や、サインインしたユーザーと共有されている予定表などが含まれている場合があります。</span><span class="sxs-lookup"><span data-stu-id="43bfa-133">This can include calendars that other users have delegated or shared with the signed-in user.</span></span>

<span data-ttu-id="43bfa-134">**getSchedule** は、委任シナリオとアプリ専用シナリオの両方をサポートします。</span><span class="sxs-lookup"><span data-stu-id="43bfa-134">**getSchedule** supports both delegated and app-only scenarios.</span></span> <span data-ttu-id="43bfa-135">後者の場合、管理者は、サインインしているユーザーがいなくても、すべての予定表にアプリがアクセスすることに同意します。</span><span class="sxs-lookup"><span data-stu-id="43bfa-135">In the latter, an administrator consents the app to access all calendars without a signed-in user.</span></span>


### <a name="version-support"></a><span data-ttu-id="43bfa-136">バージョンのサポート</span><span class="sxs-lookup"><span data-stu-id="43bfa-136">Version support</span></span>

<span data-ttu-id="43bfa-137">**findmeetingtimes** は、すべてのアプリで一般的に利用できます。</span><span class="sxs-lookup"><span data-stu-id="43bfa-137">**findmeetingtimes** is generally available for all apps.</span></span> 

<span data-ttu-id="43bfa-138">**getSchedule** は、現在は[プレビュー状態](versioning-and-support.md#beta-version)で利用できます。そのため、運用環境アプリでは使用できません。</span><span class="sxs-lookup"><span data-stu-id="43bfa-138">**getSchedule** is currently available [in preview status](versioning-and-support.md#beta-version), and therefore is not appropriate for use in production apps.</span></span>


## <a name="permissions"></a><span data-ttu-id="43bfa-139">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="43bfa-139">Permissions</span></span>
<span data-ttu-id="43bfa-140">空き時間情報を取得するために必要な最低限の特権のアクセス許可は Calendar.Read です。</span><span class="sxs-lookup"><span data-stu-id="43bfa-140">The least privileged permission you need to get free/busy information is Calendar.Read.</span></span> <span data-ttu-id="43bfa-141">アプリのシナリオによっては、サインインしているユーザーまたは管理者が同意することができます。</span><span class="sxs-lookup"><span data-stu-id="43bfa-141">Depending on your app scenario, this can be consented by the signed-in user or administrator.</span></span>
<span data-ttu-id="43bfa-142">**getSchedule** は、要求されたエンティティの空き時間情報と稼働時間以外にも、次の条件を満たす場合に、イベントの件名と場所を返すことができます。</span><span class="sxs-lookup"><span data-stu-id="43bfa-142">Other than the free/busy status and working hours of requested entities, **getSchedule** can also return the subject and location of an event, provided that:</span></span>

- <span data-ttu-id="43bfa-143">イベントの秘密度レベルが低く (`normal` または `personal`)、さらに次の条件の 1 つ以上が適用される場合:</span><span class="sxs-lookup"><span data-stu-id="43bfa-143">If the event is marked with low sensitivity level - `normal` or `personal` AND one or more of the following conditions applies:</span></span>

- <span data-ttu-id="43bfa-144">要求されたユーザーの予定表の設定では、組織内のすべてのユーザーがタイトルと場所を表示できます</span><span class="sxs-lookup"><span data-stu-id="43bfa-144">The requested user’s calendar settings allow all the users in the organization to view titles and locations</span></span>
- <span data-ttu-id="43bfa-145">要求されたユーザーの予定表は、サインインしたユーザーと共有されています</span><span class="sxs-lookup"><span data-stu-id="43bfa-145">The requested user’s calendar is shared with the signed-in user</span></span>
- <span data-ttu-id="43bfa-146">サインインしたユーザーは、要求されたユーザーと同じ組織の管理者です。</span><span class="sxs-lookup"><span data-stu-id="43bfa-146">The signed-in user is an administrator of the same organization as the requested user.</span></span>

## <a name="time-zone-representation"></a><span data-ttu-id="43bfa-147">タイム ゾーン表現</span><span class="sxs-lookup"><span data-stu-id="43bfa-147">Time zone representation</span></span>
<span data-ttu-id="43bfa-148">既定では、返されるスケジュール項目の開始時刻と終了時刻は UTC で表されます。</span><span class="sxs-lookup"><span data-stu-id="43bfa-148">By default, the start and end times of the returned schedule items are represented in UTC.</span></span> <span data-ttu-id="43bfa-149">`Prefer` ヘッダーを使用して、お使いのアプリに適したタイム ゾーンを指定することができます。</span><span class="sxs-lookup"><span data-stu-id="43bfa-149">You can use a `Prefer` header to specify a time zone appropriate for your app.</span></span> <span data-ttu-id="43bfa-150">次に例を示します。</span><span class="sxs-lookup"><span data-stu-id="43bfa-150">As an example:</span></span> 
```
Prefer: outlook.timezone="Pacific Standard Time"
```

## <a name="limits-and-error-conditions"></a><span data-ttu-id="43bfa-151">制限とエラー条件</span><span class="sxs-lookup"><span data-stu-id="43bfa-151">Limits and error conditions</span></span>
<span data-ttu-id="43bfa-152">次の制限とエラー条件に注意してください。</span><span class="sxs-lookup"><span data-stu-id="43bfa-152">Be aware of the following limits and error condition:</span></span>

- <span data-ttu-id="43bfa-153">**getSchedule** では、一度に最大 20 エンティティの空き時間情報を検索することができます。</span><span class="sxs-lookup"><span data-stu-id="43bfa-153">**getSchedule** can support looking up free/busy information for up to 20 entities at once.</span></span> <span data-ttu-id="43bfa-154">この制限は、個別にまたは配布リストのメンバーとして識別されるユーザー数、およびリソース数にも適用されます。</span><span class="sxs-lookup"><span data-stu-id="43bfa-154">This limit applies to the number of users identified individually or as members of a distribution list, and to the number of resources as well.</span></span>
- <span data-ttu-id="43bfa-155">検索する期間は 42 日未満である必要があります。</span><span class="sxs-lookup"><span data-stu-id="43bfa-155">The time period to look up must be less than 42 days.</span></span>
- <span data-ttu-id="43bfa-156">指定されたユーザーまたはリソースを **getSchedule** で識別できない場合は、単一のスケジュール項目が返され、エラーが示されます。</span><span class="sxs-lookup"><span data-stu-id="43bfa-156">If **getSchedule** cannot identify a specified user or resource, it returns a single schedule item and indicates the error.</span></span> 

## <a name="see-also"></a><span data-ttu-id="43bfa-157">関連項目</span><span class="sxs-lookup"><span data-stu-id="43bfa-157">See also</span></span>
- [<span data-ttu-id="43bfa-158">アクセス許可リファレンス</span><span class="sxs-lookup"><span data-stu-id="43bfa-158">Permissions reference</span></span>](permissions-reference.md#calendars-permissions)
- [<span data-ttu-id="43bfa-159">開催可能な会議日時を Outlook カレンダーで検索する</span><span class="sxs-lookup"><span data-stu-id="43bfa-159">Find possible meeting times on the Outlook calendar</span></span>](findmeetingtimes-example.md)
