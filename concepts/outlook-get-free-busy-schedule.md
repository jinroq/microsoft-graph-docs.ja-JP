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
# <a name="get-freebusy-schedule-of-users-and-resources-preview"></a>ユーザーおよびリソース (プレビュー) のスケジュールの空き時間情報を取得します。

作業または学校の設定では、一般的なシナリオは、ユーザーが会議の空きを確認したりすると、チーム、部屋、または期間内の機器の可用性を参照します。

[GetSchedule](/graph/api/calendar-getschedule?view=graph-rest-beta)アクションでは、特定の期間の 1 つまたは複数のエンティティのユーザー、配布リスト、またはリソースの可用性情報を取得することができます。 

## <a name="example"></a>例

Pacitfic 標準時午後 6 時までの 9 am からの特定の日に、アレックス、同僚の空き時間のスケジュールを検索する例を示します。

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

**getSchedule**は、Alex の既存のイベントに一致する項目をスケジュール 2 を返します ' 既定の予定表、各イベントと、空き/予約済みの状態の開始と終了時刻を表示します。 Alex は、その日付と時刻の範囲内の残りの時間の空きを想定することができます。

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

スケジュールの空き時間情報、Alex の作業時間とは別**getSchedule**も返します**availabilityView**アレックスのマージされたビューには ' その日の可用性です。 マージされたビューは、Alex を示す各タイム ・ スロットに、その日に対応する時間帯で構成される文字列 ' 次の規則を使用して可用性。 

- `0`無料 =
- `1`仮の予定 =
- `2`= ビジー
- `3`外出 =
- `4`他の場所で作業を = します。 

既定では、各タイム ・ スロットの長さは、30 分です。 この例では、15 分に時間帯をカスタマイズするのには**availabilityViewInterval**プロパティを使用します。

## <a name="how-is-getschedule-different-from-findmeetingtimes"></a>どのように getSchedule とは異なる findMeetingTimes です。

[FindMeetingTimes](/graph/api/user-findmeetingtimes?view=graph-rest-1.0)アクションは、指定されたユーザーおよびリソースの作業時間と空き時間情報を読み取る両方という点で**getSchedule**に似ています。 2 つのアクションは、いくつかの主要な方法が異なります。

### <a name="application"></a>アプリケーション

**findMeetingTimes**には、次のように会議の時刻と場所を提案する特定のビジネス ロジックが適用されます。

- 各エンティティのオプションまたは必須の出勤
- 1 日の時間の要求されたアクティビティの性質
- 会議のクォーラムに必要な最低限の参加

[予約を合理化すること](findmeetingtimes-example.md)に依存するシナリオに適しています。

**getSchedule**は単に空き時間情報のステータスを返します既存のイベントで要求されたカレンダーの特定の期間のと tp がその時間内に残り時間を想定しています。 さらにビジネス ロジックを適用するには、シナリオを完了するのにはこのデータを使用します。

### <a name="app-only-support"></a>アプリケーション専用のサポート

**findmeetingtimes**は、アプリケーションにサインインしているユーザーを必要とする委任のシナリオのみをサポートします。 アプリケーションでは、サインインしているユーザーがアクセスできるカレンダーのみでイベントを読み取ることができます。 これには、他のユーザーが委任するか、サインイン中のユーザーと共有の予定表が含まれます。

**getSchedule**には、委任とアプリ専用のシナリオがサポートされています。 後者の場合、管理者にお客様がサインインしているユーザーがいない状態のすべての予定表にアクセスするアプリケーション同意します。


### <a name="version-support"></a>バージョンのサポート

**findmeetingtimes**は、すべてのアプリケーションで一般的に使用できます。 

**getSchedule**は現在利用可能な[プレビューの状態で](versioning-and-support.md#beta-version)、したがって運用アプリケーションで使用するために適切ではありません。


## <a name="permissions"></a>Permissions
空き時間情報を取得する必要が最低限の特権のアクセス許可は、Calendar.Read です。 アプリケーション シナリオによっては、これはサインインしているユーザーまたは管理者によって同意ことができます。
以外の空き時間情報のステータスと稼働時間の要求のエンティティを**getSchedule**を返すことも、件名と場所を提供する、イベントの。

- イベントが [低] 感度のレベルが付いている場合`normal`または`personal`し、次の条件の 1 つ以上を適用します。

- 要求されたユーザーの予定表の設定は、タイトルや場所を表示するのには組織内のすべてのユーザーを許可します。
- 要求されたユーザーの予定表は、サインイン中のユーザーと共有します。
- サインイン中のユーザーは、要求されたユーザーと同じ組織の管理者です。

## <a name="time-zone-representation"></a>タイム ゾーン表現
既定では、返されたスケジュール項目の開始と終了時刻が UTC で表されます。 使用することができます、 `Prefer` 、アプリの適切なタイム ゾーンを指定するヘッダー。 例:  
```
Prefer: outlook.timezone="Pacific Standard Time"
```

## <a name="limits-and-error-conditions"></a>制限値とエラー条件
次の制限およびエラー条件に注意します。

- **getSchedule**では、空き時間情報を最大 20 個のエンティティを一度に検索をサポートできます。 この制限は、個別に、または配布リストのメンバーとして識別されるユーザーの数にしても、リソースの数に適用されます。
- 検索するまでの時間は 42 日未満である必要があります。
- **GetSchedule**は、指定したユーザーまたはリソースを識別できない場合、1 つのスケジュール項目を返し、エラーを示します。 

## <a name="see-also"></a>関連項目
- [アクセス許可を参照します。](permissions-reference.md#calendars-permissions)
- [開催可能な会議日時を Outlook カレンダーで検索する](findmeetingtimes-example.md)
