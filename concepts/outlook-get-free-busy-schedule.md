# <a name="get-freebusy-schedule-for-users-and-resources-preview"></a>ユーザーおよびリソース (プレビュー) のスケジュールの空き時間情報を取得します。

作業または学校の設定では、一般的なシナリオは、ユーザーが会議の空きを確認したりすると、チーム、部屋、または期間内の機器の可用性を参照します。

 [GetSchedule](../api-reference/beta/api/calendar_getschedule.md) アクションでは、特定の期間の 1 つまたは複数のエンティティのユーザー、配布リスト、またはリソースの可用性情報を取得することができます。 

## <a name="example"></a>例

太平洋標準時午前9から午後 6 時までの特定の日に、同僚アレックスの空き時間のスケジュールを検索する例を示します。

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

**getSchedule** は、アレックスの既存のイベントに一致する項目をスケジュール 2 を返します ' 既定の予定表、各イベントと、空き/予約済みの状態の開始と終了時刻を表示します。 アレックスは、その日付と時刻の範囲内の残りの時間が空いていることを想定できます。

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

アレックスのスケジュールの空き時間情報と作業時間とは別 **getSchedule** も返します **availabilityView**アレックスのマージされたビューには ' その日の可用性です。 マージされたビューは、その日をカバーするタイムスロットで構成された文字列であり、各タイムスロットは次の規則を使用してアレックスの可用性を示します。 

- `0`自由
- `1`仮
- `2`多忙
- `3`外出中
- `4`他の場所で働いています。 

既定では、各タイム スロットの長さは、30 分です。 この例では、15 分に時間帯をカスタマイズするのには **availabilityViewInterval** プロパティを使用します。

## <a name="how-is-getschedule-different-from-findmeetingtimes"></a>getScheduleとfindMeetingTimesの違い

 [FindMeetingTimes](../api-reference/v1.0/api/user_findmeetingtimes.md) アクションは、指定されたユーザーおよびリソースの作業時間と空き時間情報を読み取る両方という点で **getSchedule** に似ています。 2 つのアクションは、いくつかの主要な点で異なります。

### <a name="application"></a>アプリケーション

**findMeetingTimes** には、次のように会議の時刻と場所を提案する特定のビジネス ロジックが適用されます。

- 各エンティティのオプションまたは強制出勤
- 1 日の時間の要求されたアクティビティの性質
- 会議のクォーラムに必要な最低限の参加

 [予約を合理化すること](findmeetingtimes_example.md)に依存するシナリオに適しています。

**getSchedule** は単に空き時間情報のステータスを返します既存のイベントで要求されたカレンダーの特定の期間のと tp がその時間内に残り時間を想定しています。 さらにビジネス ロジックを適用するには、シナリオを完了するのにはこのデータを使用します。

### <a name="app-only-support"></a>アプリ専用のサポート

**findmeetingtimes** は、アプリにサインインしているユーザーを必要とする委任のシナリオのみをサポートします。 アプリでは、サインインしているユーザーがアクセスできるカレンダーのみでイベントを読み取ることができます。 これには、他のユーザーが委任するか、サインイン中のユーザーと共有の予定表が含まれます。

**getSchedule** には、委任とアプリ専用のシナリオがサポートされています。 後者の場合、管理者は、ログインしていないユーザーがいないすべてのカレンダーにアクセスするようにアプリに同意します。


### <a name="version-support"></a>バージョンのサポート

**findmeetingtimes** は、すべてのアプリで一般的に使用できます。 

**getSchedule** は現在利用可能な [プレビューの状態で](versioning_and_support.md#beta-version)、したがって運用アプリで使用するために適切ではありません。


## <a name="permissions"></a>アクセス許可
空き時間情報を取得するために必要な最小特権は、Calendar.Readです。 アプリのシナリオによっては、ログインしているユーザーまたは管理者が同意することができます。
 getSchedule は、要求されたエンティティの空き時間や勤務時間以外にも、イベントの件名と場所を返すことができます。** **

- イベントが [低] 感度のレベルが付いている場合 `normal` または `personal` し、次の条件の 1 つ以上を適用します。

- 要求されたユーザーのカレンダー設定では、組織内のすべてのユーザーがタイトルと場所を表示できます
- 要求されたユーザーの予定表は、サインイン中のユーザーと共有します。
- ログインしているユーザーは、要求されたユーザーと同じ組織の管理者です。

## <a name="time-zone-representation"></a>タイムゾーン表現
既定では、返されたスケジュール項目の開始と終了時刻が UTC で表されます。 `Prefer`ヘッダーを使用して、アプリに適したタイムゾーンを指定することができます。 例: 
```
Prefer: outlook.timezone="Pacific Standard Time"
```

## <a name="limits-and-error-conditions"></a>制限値とエラー条件
次の制限とエラー状態に注意してください。

- **getSchedule** では、空き時間情報を最大 20 個のエンティティを一度に検索をサポートできます。 この制限は、個々にまたは配布リストのメンバーとして識別されたユーザー数、およびリソース数にも適用されます。
- 検索するまでの時間は 42 日未満である必要があります。
-  **GetSchedule** は、指定したユーザーまたはリソースを識別できない場合、1 つのスケジュール項目を返し、エラーを示します。 

## <a name="see-also"></a>関連項目
- [アクセス許可の参照](permissions_reference.md#calendars-permissions)
- [開催可能な会議日時を Outlook カレンダーで検索する](findmeetingtimes_example.md)
