# <a name="user-findmeetingtimes"></a>user: findMeetingTimes
パラメーターとして指定された開催者と出席者の空き時間、および時間または場所の制約に基づいて、会議時間の提案を検索します。

**findMeetingTimes** が会議提案を返すことができない場合は、応答で、**emptySuggestionsReason** プロパティに理由が示されます。この値に基づいて、パラメーターをさらに調整して、**findMeetingTimes** を再度呼び出すことができます。

**注**

現時点では、**findMeetingTimes** は以下を前提としています。

- 人である (リソースとは異なる) [attendee](../resources/attendee.md) は、必須の出席者です。そのため、**attendees** コレクション パラメーターの一部として、対応する **type** プロパティで人に `required` を、リソースに `resource` を指定します。
- 会議は、開催者または出席者の勤務時間内のみで提案されます。[timeConstraint](../resources/timeConstraint.md) の **activityDomain** プロパティの指定は無視することができます 


## <a name="prerequisites"></a>前提条件
この API を実行するには、以下のいずれかの**スコープ**が必要です。*Calendars.Read.Shared* または *Calendars.ReadWrite.Shared*
## <a name="http-request"></a>HTTP 要求
<!-- { "blockType": "ignored" } -->
```http
POST /me/findMeetingTimes
POST /users/{id|userPrincipalName}/findMeetingTimes
```
## <a name="request-headers"></a>要求ヘッダー
| 名前       | 値|
|:---------------|:----------|
| 承認  | Bearer <code>|
| Prefer: outlook.timezone | 応答として "太平洋標準時" などの特定のタイム ゾーンを表す文字列です。 |


## <a name="request-body"></a>要求本文
サポートされているすべてのパラメーターは以下のとおりです。シナリオに応じて、要求本文で必要な各パラメーターの JSON オブジェクトを指定します。指定したパラメーターに基づいて、**findMeetingTimes** は開催者と出席者の標準として設定されている予定表で空き時間状態を確認します。アクションは、開催できる可能性が最も高い会議の日時を計算し、会議の提案を返します。


| パラメーター       | 型    |説明|
|:---------------|:--------|:----------|
|attendees|[attendeeBase](../resources/attendeebase.md) コレクション|会議の出席者またはリソースのコレクションです。コレクションを空にすると、**findMeetingTimes** は開催者のみの空き時間帯を検索します。|
|locationConstraint|[locationConstraint](../resources/locationconstraint.md)|会議の場所の提案が必要かどうか、または会議のみが開催できる特定の場所があるか、など、会議の場所に関する開催者の要件。|
|timeConstraint|[timeConstraint](../resources/timeconstraint.md)|会議を開催する開始時刻と終了時刻の範囲。このパラメーターの **start** プロパティと **end** プロパティの一部としてタイム ゾーンを指定することができます。ただし、このタイム ゾーンが影響を与えるのは、**timeConstraint** パラメーターだけで、応答が返されている場合は、時刻の値は既定で UTC になっています。`Prefer: outlook.timezone` 要求ヘッダーを使って、応答の時刻の値に特定のタイム ゾーンを指定することができます。 |
|meetingDuration|Edm.Duration|[ISO8601](http://www.iso.org/iso/iso8601) 形式で示された会議の長さです。たとえば、1 時間は 'PT1H' として示され、このとき 'P' は期間の指定子、'T' は時刻の指定子、'H' は時間の指定子です。会議の期間を指定しない場合、**findMeetingTimes** は既定値の 30 分を使用します。 |
|maxCandidates|Edm.Int32|返される会議時間の提案の最大数です。|
|isOrganizerOptional|Edm.Boolean|開催者の出席が必要ない場合 `True`、それ以外の場合 `false`。　|
|returnSuggestionReasons|Edm.Boolean|**SuggestionReason** プロパティで各会議提案の理由を返すには、`True`。既定値は `false` であり、そのプロパティを返しません。|
|minimumAttendeePercentage|Edm.Double| 応答で返される時間帯に最低限要求される[確度](#the-confidence-of-a-meeting-suggestion)です。割合 (%) の値 (0 から 100 まで)。 |

## <a name="response"></a>応答
成功した場合、このメソッドは `200, OK` 応答コードと、応答本文に入った [meetingTimeSuggestionsResult](../resources/meetingTimeSuggestionsResult.md) を返します。 

**meetingTimeSuggestionsResult** には、会議提案のコレクションと **emptySuggestionsReason** プロパティが含まれます。各提案は、[meetingTimeSuggestion](../resources/meetingTimeSuggestion.md) として定義され、出席者の参加の確度について、平均で 50% または**minimumAttendeePercentage** パラメーターで指定した特定の割合 (%) が付されます。 

既定では、会議の日時についての各提案は UTC で返されます。 

### <a name="the-confidence-of-a-meeting-suggestion"></a>会議の提案の確実性

**meetingTimeSuggestion** の **confidence** プロパティの範囲は 0% から 100% で、各個人の空き時間状態に基づいて会議に出席するすべての出席者の見込みを表します。

- 各出席者に関する、指定の会議期間の空き状態で、確実に出席する場合は 100%、不明な状態は 49%、忙しい場合には 0% です。
- 会議時間の提案の確実性は、指定された対象会議のすべての出席者の出席見込みの平均によって算出されます。
- 会議時間の提案が複数ある場合、**findMeetingTimes** アクションは、算出した確実性が高い方から順番に提案を並べて示します。確実性が同じ提案がある場合には、時系列で提案を並べて示します。
- **findMeetingTimes** の **minimumAttendeePercentage** オプション パラメーターを使用して、少なくとも特定の信頼度の会議の時間帯のみが返されるように指定することができます。たとえば、すべての出席者が出席する見込みが 80% 以上ある提案のみを行う場合は、80% の **minimumAttendeePercentage** を指定できます。**minimumAttendeePercentage** を指定しない場合は、**findMeetingTimes** は 50% の値を前提とします。

たとえば、提案の会議時間に次の空き時間状態の 3 人の出席者がいるとします。

|**出席者**|**空き時間状態**|**出席見込み (%)**|
|:-----|:-----|:-----|
|Dana | 空き | 100% |
|John | 不明 | 49% |
|Fanny | 多忙 | 0% |

この場合、出席の平均見込みである会議時間の提案の信頼度は、(100% + 49% + 0%)/3 = 49.66% です。

**findMeetingTimes** で 80% の **minimumAttendeePercentage** を指定すると、49.66% < 80% のため、操作では応答でこの時間の提案は返されません。

## <a name="example"></a>例

次の例は、要求本文で次のパラメーターを指定して、あらかじめ決められた会議を開催する時間を検索し、各提案の理由を要求する方法を示しています。

- **attendees**
- **locationConstraint**
- **timeConstraint**
- **meetingDuration**
- **returnSuggestionReasons**
- **minimumAttendeePercentage**

**findMeetingTimes** が任意の提案を返す場合は、**returnSuggestionReasons** パラメーターを設定することで、各提案の **SuggestionReason** プロパティの説明も取得できます。

既定では、要求は PST のタイム ゾーンの時間を指定し、応答は UTC で会議時間の提案を返すことに注意してください。PST を指定するのに、また応答の時間の値にも `Prefer: outlook.timezone` 要求ヘッダーを使うことができます。

##### <a name="request"></a>要求
要求の例を次に示します。
<!-- {
  "blockType": "request",
  "name": "user_findmeetingtimes"
}-->
```http
POST https://graph.microsoft.com/v1.0/me/findMeetingTimes
Content-type: application/json

{ 
  "attendees": [ 
    { 
      "type": "required",  
      "emailAddress": { 
        "name": "Fanny Downs",
        "address": "fannyd@a830edad905084922E16072013.onmicrosoft.com" 
      } 
    },
    { 
      "type": "optional",  
      "emailAddress": { 
        "name": "Dana Swope",
        "address": "danas@a830edad905084922E16072013.onmicrosoft.com" 
      } 
    } 
  ],  
  "locationConstraint": { 
    "isRequired": "false",  
    "suggestLocation": "false",  
    "locations": [ 
      { 
        "resolveAvailability": "false",
        "displayName": "Conf room Hood" 
      } 
    ] 
  },  
  "timeConstraint": { 
    "timeslots": [ 
      { 
        "start": { 
          "dateTime": "2016-10-20T07:00:00",  
          "timeZone": "Pacific Standard Time" 
        },  
        "end": { 
          "dateTime": "2016-10-20T17:00:00",  
          "timeZone": "Pacific Standard Time" 
        } 
      } 
    ] 
  },  
  "meetingDuration": "PT2H",
  "returnSuggestionReasons": "true",
  "minimumAttendeePercentage": "60"
}
```

##### <a name="response"></a>応答
応答の例を次に示します。メモ:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。実際の呼び出しではすべてのプロパティが返されます。
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.meetingTimeSuggestionsResult",
  "isCollection": false
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json


{
   "@odata.context":"https://graph.microsoft.com/v1.0/$metadata#microsoft.graph.meetingTimeSuggestionsResult",
   "meetingTimeSuggestions":[
      {
         "meetingTimeSlot":{
            "start":{
               "dateTime":"2016-10-20T15:00:00.0000000",
               "timeZone":"UTC"
            },
            "end":{
               "dateTime":"2016-10-20T17:00:00.0000000",
               "timeZone":"UTC"
            }
         },
         "confidence":100,
         "organizerAvailability":"free",
         "attendeeAvailability":[
            {
               "attendee":{
                  "type":"required",
                  "emailAddress":{
                    "name": "Fanny Downs",
                    "address": "fannyd@a830edad905084922E16072013.onmicrosoft.com" 
                  }
               },
               "availability":"free"
            },
            {
               "attendee":{
                  "type":"required",
                  "emailAddress":{
                    "name": "Dana Swope",
                    "address": "danas@a830edad905084922E16072013.onmicrosoft.com" 
                  }
               },
               "availability":"free"
            }
         ],
         "locations":[
            {
               "displayName":"Conf room Hood"
            }
         ],
         "suggestionReason":"Suggested because it is one of the nearest times when all attendees are available."
      },
      {
         "meetingTimeSlot":{
            "start":{
               "dateTime":"2016-10-20T17:00:00.0000000",
               "timeZone":"UTC"
            },
            "end":{
               "dateTime":"2016-10-20T19:00:00.0000000",
               "timeZone":"UTC"
            }
         },
         "confidence":100,
         "organizerAvailability":"free",
         "attendeeAvailability":[
            {
               "attendee":{
                  "type":"required",
                  "emailAddress":{
                    "name": "Fanny Downs",
                    "address": "fannyd@a830edad905084922E16072013.onmicrosoft.com" 
                  }
               },
               "availability":"free"
            },
            {
               "attendee":{
                  "type":"required",
                  "emailAddress":{
                    "name": "Dana Swope",
                    "address": "danas@a830edad905084922E16072013.onmicrosoft.com" 
                  }
               },
               "availability":"unknown"
            }
         ],
         "locations":[
            {
               "displayName":"Conf room Hood"
            }
         ],
         "suggestionReason":"Suggested because it is one of the nearest times when all attendees are available."
      }
   ],
   "emptySuggestionsReason":""
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "user: findMeetingTimes",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->