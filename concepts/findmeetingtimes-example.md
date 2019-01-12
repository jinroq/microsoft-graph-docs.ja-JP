---
title: 開催可能な会議日時を Outlook カレンダーで検索する
description: '職場や学校では、集まるための共通の時間と場所を探して頻繁にオーバーヘッドが発生します。 Microsoft Graph アプリケーションで使用可能 '
localization_priority: Priority
ms.openlocfilehash: 94e9cd7455d08741851662cc071e690b3ad0a558
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/11/2019
ms.locfileid: "27819860"
---
# <a name="find-possible-meeting-times-on-the-outlook-calendar"></a>開催可能な会議日時を Outlook カレンダーで検索する

職場や学校では、集まるための共通の時間と場所を探して頻繁にオーバーヘッドが発生します。Microsoft Graph アプリケーションでは、[findMeetingTimes](/graph/api/user-findmeetingtimes?view=graph-rest-1.0) を使用して、時間、場所、他の制約を満たす開催可能な会議日時を特定できます。   

**findMeetingTimes** アクションでは、会議の日付/時刻範囲、期間、任意出席者または必須出席者、アクティビティの性質 (**activityDomain**) などの条件を指定できます。アクションでは、出席者と開催者の通常の勤務スケジュールと空き時間情報が考慮され、参加者とアクティビティの種類に適した時間が提案されます。たとえば、業務関連のアクティビティは常に開催者と出席者の勤務時間中に行われるように提案され、必須出席者が出席可能な提案は候補リストの上位に表示されます。

Office 365 では、勤務時間とタイム ゾーンをメールボックスごとに構成できます。**findMeetingTimes** アクションは、開催者と出席者間のタイム ゾーンの違いを処理します。既定では、**findMeetingTimes** は UTC で提案を返します。次の要求ヘッダーを使用すると、**findMeetingTimes** は特定のタイム ゾーンで表された提案を返すようになります。
```
Prefer: outlook.timezone="{time-zone-string}}"
```

大規模な会議で特に便利な機能として、定足数のパーセンテージ (**minimumAttendeePercentage**) を指定して、最低限の出席者の空き時間を満たす場合にのみ、**findMeetingTimes** が提案を返すようにできます。

**findMeetingTimes** が会議日時をまったく提案できない場合は、開催者や必須出席者が出席できないなどの特定の理由 (**emptySuggestionsReason**) を示します。この値に基づいて、パラメーターをさらに調整して、**findMeetingTimes** をもう一度呼び出すことができます。

>**注** **findMeetingTimes** アクションは、現在 Office 365 の職場または学校のメールボックスで使用できますが、個人用 outlook.com のメールボックスでは使用できません。

## <a name="example"></a>例

次の例は、**findMeetingTimes** を使用して、2 人のユーザーが数時間会合するための可能な時間を返す方法を示しています。これには、ユーザーの空き時間と勤務スケジュール、および時間内に不在である出席者が考慮されています。この会議の出席者は 2 人のユーザーのみであるため、提案には 100% の出席が必要です。ユーザーの空き時間スケジュールを次に示します。

### <a name="organizers-calendar"></a>開催者のカレンダー

![4 月 17 日から 21 日の空き時間が表示されている開催者の勤務カレンダー](./images/findmeetingtimes_organizer_free_busy.jpg "4 月 17 日から 21 日の空き時間が表示されている開催者の勤務カレンダー")

### <a name="attendees-calendar"></a>出席者のカレンダー

![4 月 17 日から 21 日の空き時間が表示されている出席者の勤務カレンダー](./images/findmeetingtimes_attendee_free_busy.jpg "4 月 17 日から 21 日の空き時間が表示されている出席者の勤務カレンダー")

この例では、**findMeetingTimes** の呼び出しを 2 回行います。

1. 最初の呼び出しは、4 月 18 日から 20 日の日付の範囲を検索します。出席者が 4 月 18 日から 19 日は不在であり、4 月 20 日には共通の空き時間がないため、最初の呼び出しは提案を返しません (理由 (**emptySuggestionsReason**): 出席者が参加できない)。
2. 2 番目の呼び出しは、4 月 21 日の空き時間を検索し、午後 2 時から 4 時の提案を返します。

**findMeetingTimes** への 2 回の呼び出しには、次のパラメーターが含まれます。**findMeetingTimes** のすべての[パラメーター](/graph/api/user-findmeetingtimes?view=graph-rest-1.0#request-body)は省略可能です。

- **attendees**: 1 人の出席者、Samantha Booth を **type** プロパティの `required` として設定します
- **locationConstraint**: 場所の提案は必要ありません
- **timeConstraint**: 最初の呼び出しは、4 月 18 日午前 9 時から 4 月 20 日午後 5 時までの日付/時間範囲を検索します。最初の呼び出しが日時を提案することに失敗した後、2 番目の呼び出しは 4 月 21 日の午前 9 時から午後 5 時で検索します。
- **meetingDuration**: 2 時間
- **returnSuggestionReasons**: この例では、各提案に対する理由が必要です
- **minimumAttendeePercentage**:100% (出席者が提案された時間に出席できる必要があるため)

### <a name="first-request"></a>最初の要求

4 月 18 日から 20 日で両方のユーザーが 2 時間空いている時間帯を検索します。

<!-- {
  "blockType": "ignored",
  "name": "findmeetingtimes_example_first"
}-->
```http
POST https://graph.microsoft.com/v1.0/me/findMeetingTimes
Prefer: outlook.timezone="Pacific Standard Time"
Content-type: application/json

{ 
  "attendees": [ 
    { 
      "type": "required",  
      "emailAddress": { 
        "name": "Samantha Booth",
        "address": "samanthab@contoso.onmicrosoft.com" 
      } 
    }
  ],  
  "locationConstraint": { 
    "isRequired": false,  
    "suggestLocation": false,  
    "locations": [ 
      { 
        "resolveAvailability": false,
        "displayName": "Conf room Hood" 
      } 
    ] 
  },  
  "timeConstraint": {
    "activityDomain":"work", 
    "timeslots": [ 
      { 
        "start": { 
          "dateTime": "2017-04-18T09:00:00",  
          "timeZone": "Pacific Standard Time" 
        },  
        "end": { 
          "dateTime": "2017-04-20T17:00:00",  
          "timeZone": "Pacific Standard Time" 
        } 
      } 
    ] 
  },  
  "meetingDuration": "PT2H",
  "returnSuggestionReasons": true,
  "minimumAttendeePercentage": 100
}
```

### <a name="first-response"></a>最初の応答
4 月 18 日から 20 日の勤務時間中に両方のユーザーが出席可能な 2 時間の時間帯はありません。
<!-- {
  "blockType": "ignored",
  "truncated": true,
  "@odata.type": "microsoft.graph.meetingTimeSuggestionsResult",
  "isCollection": false
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Preference-Applied: outlook.timezone="Pacific Standard Time"
Content-Length: 184

{
    "@odata.context":"https://graph.microsoft.com/v1.0/$metadata#microsoft.graph.meetingTimeSuggestionsResult",
    "emptySuggestionsReason":"AttendeesUnavailable",
    "meetingTimeSuggestions":[

    ]
}
```

### <a name="second-request"></a>2 番目の要求
4 月 21 日の 2 時間の時間帯を検索します。
<!-- {
  "blockType": "ignored",
  "name": "findmeetingtimes_example_second"
}-->
```http
POST https://graph.microsoft.com/v1.0/me/findMeetingTimes
Prefer: outlook.timezone="Pacific Standard Time"
Content-type: application/json

{ 
  "attendees": [ 
    { 
      "type": "required",  
      "emailAddress": { 
        "name": "Samantha Booth",
        "address": "samanthab@contoso.onmicrosoft.com" 
      } 
    }
  ],  
  "locationConstraint": { 
    "isRequired": false,  
    "suggestLocation": false,  
    "locations": [ 
      { 
        "resolveAvailability": false,
        "displayName": "Conf room Hood" 
      } 
    ] 
  },  
  "timeConstraint": {
    "activityDomain":"work", 
    "timeslots": [ 
      { 
        "start": { 
          "dateTime": "2017-04-21T09:00:00",  
          "timeZone": "Pacific Standard Time" 
        },  
        "end": { 
          "dateTime": "2017-04-21T17:00:00",  
          "timeZone": "Pacific Standard Time" 
        } 
      } 
    ] 
  },  
  "meetingDuration": "PT2H",
  "returnSuggestionReasons": true,
  "minimumAttendeePercentage": 100
}
```

### <a name="second-response"></a>2 番目の応答のサンプル
2 番目の **findMeetingTimes** 要求は、両方のユーザーが会合するために 4 月 21 日午後 2 時から 4 時を提案します。
<!-- {
  "blockType": "ignored",
  "truncated": true,
  "@odata.type": "microsoft.graph.meetingTimeSuggestionsResult",
  "isCollection": false
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Preference-Applied: outlook.timezone="Pacific Standard Time"
Content-Length: 714

{
    "@odata.context":"https://graph.microsoft.com/v1.0/$metadata#microsoft.graph.meetingTimeSuggestionsResult",
    "emptySuggestionsReason":"",
    "meetingTimeSuggestions":[
        {
            "confidence":100.0,
            "organizerAvailability":"free",
            "suggestionReason":"Suggested because it is one of the nearest times when all attendees are available.",
            "meetingTimeSlot":{
                "start":{
                    "dateTime":"2017-04-21T14:00:00.0000000",
                    "timeZone":"Pacific Standard Time"
                },
                "end":{
                    "dateTime":"2017-04-21T16:00:00.0000000",
                    "timeZone":"Pacific Standard Time"
                }
            },
            "attendeeAvailability":[
                {
                    "availability":"free",
                    "attendee":{
                        "type":"required",
                        "emailAddress":{
                            "address":"samanthab@contoso.onmicrosoft.com"
                        }
                    }
                }
            ],
            "locations":[
                {
                    "displayName":"Conf room Hood"
                }
            ]
        }
    ]
}
```



## <a name="next-steps"></a>次の手順

一部の出席者が会議に出席できない場合があります。**minimumAttendeePercentage** オプション パラメーターを指定することにより、出席の_確実性_が特定のパーセンテージに達すると、**findMeetingTimes** で時間を提案することができます。[会議の提案の確実性](/graph/api/user-findmeetingtimes?view=graph-rest-1.0#the-confidence-of-a-meeting-suggestion)と他の[パラメーター](/graph/api/user-findmeetingtimes?view=graph-rest-1.0#request-body)の詳細を参照し、より大規模な会議に対して必要に応じて適用します。

会議日時の提案を取得した後、次のことを行うことができます。

1. [イベントを作成し、会議出席依頼として送信する](/graph/api/user-post-events?view=graph-rest-1.0)
2. イベントに[添付ファイルを追加する](/graph/api/event-post-attachments?view=graph-rest-1.0)

詳細については、「[Outlook カレンダーとの統合](outlook-calendar-concept-overview.md)」を参照してください。
