---
title: ユーザーとリソースの空き時間スケジュールを取得する
description: 職場または学校の環境で一般的なシナリオとして、ユーザーが会議に出席できる時間を確認する場合や、ある期間内にチーム、部屋、または備品の空き時間情報を参照する場合があります。
author: angelgolfer-ms
localization_priority: Priority
ms.prod: outlook
ms.openlocfilehash: 8ecf31ec74327d4f5fbd9d585eef24fcaec60709
ms.sourcegitcommit: a17ad12b05fbad86fc21ea4384c36e3b14e543c3
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 03/27/2019
ms.locfileid: "30869198"
---
# <a name="get-freebusy-schedule-of-users-and-resources"></a>ユーザーとリソースの空き時間スケジュールを取得する

職場または学校の環境で一般的なシナリオとして、ユーザーが会議に出席できる時間を確認する場合や、ある期間内にチーム、部屋、または備品の空き時間情報を参照する場合があります。

[getSchedule](/graph/api/calendar-getschedule?view=graph-rest-1.0) アクションを使用すると、特定の期間について 1 つ以上のエンティティ (ユーザー、配布リスト、またはリソース) の空き時間情報を取得できます。 

## <a name="example"></a>例

特定の日の午前 9 時から午後 6 時 (太平洋標準時) までの同僚の Alex の空き時間スケジュールを検索する簡単な例を次に示します。

<!-- {
  "blockType": "ignored",
  "name": "calendar_getSchedule_concept"
}-->
```http
POST https://graph.microsoft.com/v1.0/me/calendar/getschedule 
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

**getSchedule** は、Alex の既定の予定表にある既存のイベントと一致する 2 つのスケジュール項目を返します。これで、各イベントの開始時刻と終了時刻と、その空き時間状態がわかります。 その日付/時刻の範囲内で、残りの時間は Alex が空いていると考えることができます。

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
    "@odata.context":"https://graph.microsoft.com/v1.0/$metadata#Collection(microsoft.graph.scheduleInformation)",
    "value":[
        {
            "scheduleId":"AlexW@contoso.OnMicrosoft.com",
            "availabilityView":"111111002222222200000000000000000000",
            "scheduleItems":[
                {
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

Alex の空き時間スケジュールと勤務時間以外に、**getSchedule** は **availabilityView** も返します。これは、その日の Alex の空き時間情報の結合されたビューです。 結合されたビューは、その日を対象とする時間帯で構成された文字列であり、各時間帯は次の規則を使用して Alex の空き時間情報を示します。 

- `0`= 空き時間
- `1`= 仮の予定
- `2`= ビジー
- `3`= 外出中
- `4`= 別の場所で作業。 

既定では、各時間帯の長さは 30 分です。 この例では、**availabilityViewInterval** プロパティを使用して時間帯を 15 分にカスタマイズしています。

## <a name="how-does-getschedule-compare-with-findmeetingtimes"></a>getSchedule と findMeetingTimes の違い

[findMeetingTimes](/graph/api/user-findmeetingtimes?view=graph-rest-1.0) アクションは、指定されたユーザーとリソースの空き時間情報と稼働時間を両方読み取るという点で **getSchedule** と似ています。 2 つのアクションは、いくつかの主要な点で異なります。

### <a name="application"></a>アプリケーション

**findMeetingTimes** は、特定のビジネス ロジックを適用して、次のような会議の時間と場所を提案します。

- 各エンティティの任意または必須の出席
- その日の時刻について要求されたアクティビティの性質
- 会議のクォーラムに必要な最低限の出席者

[予定の予約の合理化](findmeetingtimes-example.md)に依存するシナリオに適しています。

**getSchedule**では、要求された各予定表の指定された期間の中で、既存のイベントの空き時間情報が単純に返され、その期間の残りの時間は空き時間と見なされます。 シナリオを完了するには、このデータを利用するビジネス ロジックをさらに適用します。

### <a name="app-only-support"></a>アプリ専用のサポート

**findmeetingtimes** は、ユーザーがアプリにサインインしている必要がある委任シナリオのみをサポートしています。 このアプリで読み取ることができるのは、サインインしているユーザーがアクセスできる予定表のイベントのみです。 これには、他のユーザーから委任された予定表や、サインインしたユーザーと共有されている予定表などが含まれている場合があります。

**getSchedule** は、委任シナリオとアプリ専用シナリオの両方をサポートします。 後者の場合、管理者は、サインインしているユーザーがいなくても、すべての予定表にアプリがアクセスすることに同意します。

### <a name="permissions"></a>アクセス許可
**findmeetingtimes**で必要な最低限の権限は Calendars.Read.Shared です。

**getSchedule**で必要な最低限の権限は Calendar.Read です。 

### <a name="version-support"></a>バージョンのサポート

**findmeetingtimes** と **getSchedule** は、両方とも通常運用環境で使用可能で適切です。


## <a name="event-data-returned"></a>返されるイベント データ
アプリケーション用の**getSchedule**で空き時間情報を取得するために必要な最低限の特権のアクセス許可は Calendar.Read です。 アプリのシナリオによっては、サインインしているユーザーまたは管理者が同意することができます。

同意済みのアクセス許可があると、アプリケーションで Outlook を通じて要求されたユーザーのカレンダーに**getSchedule**を使用することができ、要求されたユーザーは**getSchedule**が返すイベント データを制御します。 

たとえば、**getSchedule**は要求されたユーザーの空き時間状況と稼働時間を返すことも、**件名**、**場所**、および提供されたイベントの**isPrivate**プロパティを返すこともできます。

- イベントの秘密度レベルが低く (`normal` または `personal`)、さらに次の条件の 1 つ以上が適用される場合:

   - 要求されたユーザーの予定表の設定は、サインインしているユーザーに件名と場所を表示します。
   - 要求されたユーザーの予定表は、サインインしたユーザーと共有されています

これらの条件は、サインインしているユーザーが組織の管理者かどうかにかかわらず適用されます。 要求されたユーザーは、返されるイベント データを制御します。

## <a name="time-zone-representation"></a>タイム ゾーン表現
既定では、返されるスケジュール項目の開始時刻と終了時刻は UTC で表されます。 `Prefer` ヘッダーを使用して、お使いのアプリに適したタイム ゾーンを指定することができます。 次に例を示します。 
```
Prefer: outlook.timezone="Pacific Standard Time"
```

## <a name="limits-and-error-conditions"></a>制限とエラー条件
次の制限とエラー条件に注意してください。

- **getSchedule** では、一度に最大 20 エンティティの空き時間情報を検索することができます。 この制限は、個別にまたは配布リストのメンバーとして識別されるユーザー数、およびリソース数にも適用されます。
- 検索する期間は 42 日未満である必要があります。
- 指定されたユーザーまたはリソースを **getSchedule** で識別できない場合は、単一のスケジュール項目が返され、エラーが示されます。 


## <a name="see-also"></a>関連項目
- [アクセス許可リファレンス](permissions-reference.md#calendars-permissions)
- [開催可能な会議日時を Outlook カレンダーで検索する](findmeetingtimes-example.md)
