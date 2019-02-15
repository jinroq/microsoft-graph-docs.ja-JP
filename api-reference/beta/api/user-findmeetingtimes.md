---
title: 'user: findMeetingTimes'
description: 開催者と出席者の空き時間と、パラメーターとして指定された時間または場所の制限に基づいて、会議の時間と場所を提案します。
localization_priority: Normal
author: angelgolfer-ms
ms.prod: outlook
ms.openlocfilehash: 345b42690644fb94a2b6b2bdf6b3cfcc9ead6333
ms.sourcegitcommit: 539ed08adf3b7ad3253c98636d4ab303ce00176e
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 02/15/2019
ms.locfileid: "30057058"
---
# <a name="user-findmeetingtimes"></a>user: findMeetingTimes

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

開催者と出席者の空き時間と、パラメーターとして指定された時間または場所の制限に基づいて、会議の時間と場所を提案します。

**findMeetingTimes** が会議提案を返すことができない場合は、応答で、**emptySuggestionsReason** プロパティに理由が示されます。この値に基づいて、パラメーターをさらに調整して、**findMeetingTimes** を再度呼び出すことができます。


## <a name="permissions"></a>アクセス許可
この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。

|アクセス許可の種類      | アクセス許可 (特権の小さいものから大きいものへ)              |
|:--------------------|:---------------------------------------------------------|
|委任 (職場または学校のアカウント) | Calendars.Read.Shared、Calendars.ReadWrite.Shared    |
|委任 (個人用 Microsoft アカウント) | サポートされていません。    |
|アプリケーション | サポートされていません。 |

## <a name="http-request"></a>HTTP 要求
<!-- { "blockType": "ignored" } -->
```http
POST /me/findMeetingTimes
POST /users/{id|userPrincipalName}/findMeetingTimes
```
## <a name="request-headers"></a>要求ヘッダー
| 名前       | 値|
|:---------------|:----------|
| Authorization  | ベアラー {トークン}。必須。 |
| 優先: outlook.timezone | 応答として "太平洋標準時" などの特定のタイム ゾーンを表す文字列です。省略可能。このヘッダーが指定されていない場合は、UTC が使用されます。 |

## <a name="request-body"></a>要求本文
サポートされているすべてのパラメーターは以下のとおりです。シナリオに応じて、要求本文で必要な各パラメーターの JSON オブジェクトを指定します。 


| パラメーター    | 種類   |説明|
|:---------------|:--------|:----------|
|attendees|[attendeeDataModel](../resources/attendeedatamodel.md)コレクション|会議の出席者またはリソースのコレクションです。 対応する**type**プロパティで、また`required`は`optional`会議室などの`resource`リソースに対してまたはを指定します。 このプロパティが指定されてい`required`ない場合、findの**会議時間**は**type**プロパティを前提としています。 空のコレクションを使用すると、 **find会議の時間**は開催者のみの空き時間帯を検索します。 省略可能。|
|isOrganizerOptional|Edm.Boolean|開催者が必ずしも出席する必要がない場合は、`True` を指定します。既定値は `false` です。省略可能。|
|locationConstraint|[locationconstraints](../resources/locationconstraints.md)|会議の場所の提案が必要かどうか、または会議のみが開催できる特定の場所があるか、など、会議の場所に関する開催者の要件。省略可能。|
|maxCandidates|Edm.Int32|返される会議時間の提案の最大数です。省略可能。|
|meetingDuration|Edm.Duration|ミーティングの長さ。 [ISO 8601](https://www.iso.org/iso/iso8601)形式で示されます。 たとえば、1時間が ' PT1H ' として示されています。ここで、' P ' は duration 指定子で、t ' は時刻指定子で、' H ' は時間指定子です。 期間の分を示すには、M を使用します。たとえば、2時間30分は ' PT2H30M ' となります。 会議の期間が指定されていない場合、findmeeting の**時間**は既定の30分になります。 省略可能。|
|minimumAttendeePercentage|Edm.Double| 応答で返される時間帯に最低限要求される[確度](#the-confidence-of-a-meeting-suggestion)です。割合 ( %) の値 (0 から 100 まで)。省略可能。|
|returnSuggestionReasons|Edm.Boolean|**SuggestionReason** プロパティで各会議提案の理由を返すには、`True` を指定します。既定値は `false` であり、そのプロパティを返しません。省略可能。|
|timeConstraint|[findMeetingTimesTimeConstraints](../resources/findmeetingtimestimeconstraints.md)|会議の性質 (**activityDomain** プロパティ) と可能な会議の時間帯 (**timeSlots** property) を含めることのできる時間制限。このパラメーターを指定しない場合、**findMeetingTimes** が **activityDomain** を `work` と仮定します。省略可能。|

**timeConstraint** パラメーターに指定できるその他の制限について、次の表で説明します。

|TimeConstraint の activityDomain 値|会議の時間の候補|
|:-----|:-----|
|作業| ユーザーの予定表の構成で定義された稼働時間 (ユーザーまたは管理者がカスタマイズできる) の範囲内で候補が提案されます。既定の稼働時間は、月曜日から金曜日の午前 8 時から午後 5 時 (メールボックスに設定されたタイム ゾーンでの時刻) です。**activityDomain** を指定しない場合、これが既定値です。 |
|personal| ユーザーの稼働時間の範囲内と、土曜日と日曜日の範囲内で候補が提案されます。既定では、月曜日から日曜日の午前 8 時から午後 5 時 (メールボックスに設定されたタイム ゾーンでの時刻) です。|
|Unrestricted | 任意の曜日の任意の時刻から候補が提案されます。|
|不明 | 将来的に使われなくなりますので、この値は使わないでください。現在の動作は、`work` と同じです。`work`、`personal` または `unrestricted` を使用するように、既存のコードを適宜変更します。|


指定したパラメーターに基づいて、**findMeetingTimes** は開催者と出席者の標準として設定されている予定表で空き時間状態を確認します。アクションは、開催できる可能性が最も高い会議の日時を計算し、会議の提案を返します。

## <a name="response"></a>応答

成功した場合、この`200 OK`メソッドは応答コードと、応答本文で[findmeetingtimesresponse](../resources/findmeetingtimesresponse.md)を返します。 

**findmeetingtimesresponse**には、会議提案と**emptySuggestionsReason**プロパティのコレクションが含まれています。 各提案は、 [meetingTimeSuggestion](../resources/meetingtimesuggestion.md)として定義されており、参加者が参加するには 50% の信頼度が必要です。または、 **minimumAttendeePercentage**パラメーターで指定した特定の% である必要があります。 

既定では、会議の日時についての各提案は UTC で返されます。 

**findMeetingTimes** が会議提案を返すことができない場合は、応答で、**emptySuggestionsReason** プロパティに理由が示されます。この値に基づいて、パラメーターをさらに調整して、**findMeetingTimes** を再度呼び出すことができます。

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
|Samantha | 多忙 | 0% |

この場合、出席の平均見込みである会議時間の提案の信頼度は、(100% + 49% + 0%)/3 = 49.66% です。

**findMeetingTimes** で 80% の **minimumAttendeePercentage** を指定すると、49.66% < 80% のため、操作では応答でこの時間の提案は返されません。

## <a name="example"></a>例

次の例は、要求本文で次のパラメーターを指定して、あらかじめ決められた会議を開催する時間を検索し、各提案の理由を要求する方法を示しています。

- **attendees**
- **locationConstraint**
- **timeConstraint**
- **isOrganizerOptional**
- **meetingDuration**
- **returnSuggestionReasons**
- **minimumAttendeePercentage**

**findMeetingTimes** が任意の提案を返す場合は、**returnSuggestionReasons** パラメーターを設定することで、各提案の **SuggestionReason** プロパティの説明も取得できます。

要求では、PST タイムゾーンの時刻が指定されていることに注意してください。 既定では、応答は会議時間の提案を UTC で返します。 `Prefer: outlook.timezone`要求ヘッダーを使用して、応答の時間の値に加えて PST を指定することができます。

##### <a name="request"></a>要求
要求の例を次に示します。
<!-- {
  "blockType": "request",
  "name": "user_findmeetingtimes"
}-->
```http
POST https://graph.microsoft.com/beta/me/findMeetingTimes
Prefer: outlook.timezone="Pacific Standard Time"
Content-Type: application/json

{ 
  "attendees": [ 
    { 
      "type": "required",  
      "emailAddress": { 
        "name": "Alex Wilbur",
        "address": "alexw@contoso.onmicrosoft.com" 
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
    "activityDomain":"work", 
    "timeslots": [ 
      { 
        "start": { 
          "dateTime": "2019-04-16T09:00:00",  
          "timeZone": "Pacific Standard Time" 
        },  
        "end": { 
          "dateTime": "2019-04-18T17:00:00",  
          "timeZone": "Pacific Standard Time" 
        } 
      } 
    ] 
  },  
  "isOrganizerOptional": "false",
  "meetingDuration": "PT1H",
  "returnSuggestionReasons": "true",
  "minimumAttendeePercentage": "100"
}
```

##### <a name="response"></a>応答
応答の例を次に示します。メモ:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。実際の呼び出しではすべてのプロパティが返されます。
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.findMeetingTimesResponse",
  "isCollection": false
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Preference-Applied: outlook.timezone="Pacific Standard Time"

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#microsoft.graph.findMeetingTimesResponse",
    "emptySuggestionsReason": "",
    "meetingTimeSuggestions": [
        {
            "confidence": 100,
            "organizerAvailability": "free",
            "suggestionReason": "Suggested because it is one of the nearest times when all attendees are available.",
            "attendeeAvailability": [
                {
                    "availability": "free",
                    "attendee": {
                        "emailAddress": {
                            "address": "alexw@contoso.onmicrosoft.com"
                        }
                    }
                }
            ],
            "locations": [
                {
                    "displayName": "Conf room Hood"
                }
            ],
            "meetingTimeSlot": {
                "start": {
                    "dateTime": "2019-04-18T08:00:00.0000000",
                    "timeZone": "Pacific Standard Time"
                },
                "end": {
                    "dateTime": "2019-04-18T09:00:00.0000000",
                    "timeZone": "Pacific Standard Time"
                }
            }
        },
        {
            "confidence": 100,
            "organizerAvailability": "free",
            "suggestionReason": "Suggested because it is one of the nearest times when all attendees are available.",
            "attendeeAvailability": [
                {
                    "availability": "free",
                    "attendee": {
                        "emailAddress": {
                            "address": "alexw@contoso.onmicrosoft.com"
                        }
                    }
                }
            ],
            "locations": [
                {
                    "displayName": "Conf room Hood"
                }
            ],
            "meetingTimeSlot": {
                "start": {
                    "dateTime": "2019-04-18T12:00:00.0000000",
                    "timeZone": "Pacific Standard Time"
                },
                "end": {
                    "dateTime": "2019-04-18T13:00:00.0000000",
                    "timeZone": "Pacific Standard Time"
                }
            }
        },
        {
            "confidence": 100,
            "organizerAvailability": "free",
            "suggestionReason": "Suggested because it is one of the nearest times when all attendees are available.",
            "attendeeAvailability": [
                {
                    "availability": "free",
                    "attendee": {
                        "emailAddress": {
                            "address": "alexw@contoso.onmicrosoft.com"
                        }
                    }
                }
            ],
            "locations": [
                {
                    "displayName": "Conf room Hood"
                }
            ],
            "meetingTimeSlot": {
                "start": {
                    "dateTime": "2019-04-18T16:00:00.0000000",
                    "timeZone": "Pacific Standard Time"
                },
                "end": {
                    "dateTime": "2019-04-18T17:00:00.0000000",
                    "timeZone": "Pacific Standard Time"
                }
            }
        }
    ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "user: findMeetingTimes",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Warning: /api-reference/beta/api/user_findmeetingtimes.md:\r\n      Failed to parse any rows out of table with headers: |activityDomain value|Suggestions for meeting times|",
    "Error: /api-reference/beta/api/user-findmeetingtimes.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
