# <a name="update-event"></a>イベントの更新

 [イベント](../resources/event.md)  オブジェクトのプロパティを更新します。
## <a name="permissions"></a>アクセス許可
この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](../../../concepts/permissions_reference.md)」を参照してください。

|アクセス許可の種類      | アクセス許可 (特権の小さいものから大きいものへ)              |
|:--------------------|:---------------------------------------------------------|
|委任 (職場または学校のアカウント) | Calendars.ReadWrite    |
|委任 (個人用 Microsoft アカウント) | Calendars.ReadWrite    |
|アプリケーション | Calendars.ReadWrite |

## <a name="http-request"></a>HTTP 要求
<!-- { "blockType": "ignored" } -->
```http
PATCH /me/events/{id}
PATCH /users/{id | userPrincipalName}/events/{id}
PATCH /groups/{id}/events/{id}

PATCH /me/calendar/events/{id}
PATCH /users/{id | userPrincipalName}/calendar/events/{id}
PATCH /groups/{id}/calendar/events/{id}

PATCH /me/calendars/{id}/events/{id}
PATCH /users/{id | userPrincipalName}/calendars/{id}/events/{id}

PATCH /me/calendargroup/calendars/{id}/events/{id}
PATCH /users/{id | userPrincipalName}/calendargroup/calendars/{id}/events/{id}

PATCH /me/calendargroups/{id}/calendars/{id}/events/{id}
PATCH /users/{id | userPrincipalName}/calendargroups/{id}/calendars/{id}/events/{id}
```
## <a name="request-headers"></a>要求ヘッダー
| 名前       | 型 | 説明|
|:-----------|:------|:----------|
| 承認  | 文字列  | ベアラー {トークン}。必須。 |

## <a name="request-body"></a>要求本文
要求本文で、更新する関連フィールドの値を指定します。要求本文に含まれない既存のプロパティは、以前の値のままになるか、他のプロパティ値の変化に基づいて再計算されます。最適なパフォーマンスを得るためには、変更されていない既存の値を含めないでください。

| プロパティ     | タイプ   |説明|
|:---------------|:--------|:----------|
|出席者|[出席者](../resources/attendee.md)|イベントの参加者のコレクションです。|
|本文|[ItemBody](../resources/itembody.md)|イベントに関連付けられたメッセージの本文。|
|分類項目|文字列|イベントに関連付けられたカテゴリ。|
|終了|[DateTimeTimeZone](../resources/datetimetimezone.md)|イベントが終了する日時。<br/><br/>既定で、終了時刻は UTC 単位です。EndTimeZone でオプションのタイム ゾーンを指定して、そのタイム ゾーンで終了時刻を表現し、UTC からの時間オフセットを含めることができます。EndTimeZone を使用する場合、StartTimeZone の値も指定する必要があります。<br/><br/>この例では、太平洋標準時で 2015 年 2 月 25 日午後 9:34 を指定します ("2015-02-25T21:34:00-08:00")。 |
|重要性|文字列|イベントの重要性。 可能な値は、  `low`、 `normal`、 `high` です。|
|isAllDay|ブール値|イベントが一日中続く場合に、true に設定します。|
|isReminderOn|ブール値|ユーザーにイベントを通知するアラートを設定する場合は、true に設定します。|
|位置|[位置](../resources/location.md)|イベントの場所。|
|位置|[location](../resources/location.md) コレクション|イベントを開催する場所、または参加者がいる場所。 **location** プロパティと **locations** プロパティは常に互いに一致します。  **location**  のプロパティを更新すると、 **locations**  のコレクションに含まれる既存の位置がすべて削除されて、 **location** の新しい値に置き換えられます。 |
|パターン|[PatternedRecurrence](../resources/patternedrecurrence.md)|イベントの繰り返しパターン。|
|reminderMinutesBeforeStart|Int32|アラーム通知を行う、イベント開始時間前の分数。|
|responseRequested|ブール値|イベントが承諾または辞退されたときに、送信者が応答を要求する場合に、true に設定します。|
|秘密度|文字列| 指定できる値は、 `normal` 、 `personal` 、 `private` 、 `confidential` です。|
|showAs|文字列|状況表示。 指定できる値は、 `free`、 `tentative`、 `busy`、 `oof`、 `workingElsewhere`、 `unknown` です。|
|開始|[DateTimeTimeZone](../resources/datetimetimezone.md)|イベントの開始時刻です。 <br/><br/>既定で、開始時刻は UTC 単位です。EndTimeZone でオプションのタイム ゾーンを指定して、そのタイム ゾーンで開始時刻を表現し、UTC からの時間オフセットを含めることができます。StartTimeZone を使用する場合、EndTimeZone の値も指定する必要があります。<br/><br/>この例では、太平洋標準時で 2015 年 2 月 25 日午後 7:34 を指定します "2015-02-25T19:34:00-08:00".  |
|件名|文字列|イベントの件名のテキスト。|

 **イベント** リソースは [拡張機能](../../../concepts/extensibility_overview.md) をサポートしているため、 `PATCH` 操作を使用して、既存の **イベント** インスタンスで拡張機能のカスタム プロパティにあるアプリ固有のデータを追加、更新、または削除することができます。  
  
更新している **イベント** が定期的な一連のイベントのマスターである場合、複数の出席者が含まれていて、個別に更新されたインスタンスがある場合は、複数の通知の電子メールが送信されます: 一連イベントのマスターに一通と、更新されたインスタンスごとに 一通送信されます。  

## <a name="response"></a>応答

成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で、更新された [event](../resources/event.md) オブジェクトを返します。  

>**注:** このメソッドは、 `ErrorOccurrenceCrossingBoundary` のエラーコードと「修正したイベントは隣のイベントを横ぎるか、もしくは重複しています。」というエラーメッセージと共に、HTTP 400 Bad Request 応答を返すことが出来ます。 これは、パターンの例外に対する次の Outlook 制限をその更新が侵していることを示します。「イベントはその前のイベントのあった日またはその日以前に移動させることはできないし、その次のイベントのある日またはその日以降に移動させることもできない。」

## <a name="example"></a>例

##### <a name="request"></a>要求

以下は、要求の例です。
<!-- {
  "blockType": "request",
  "name": "update_event"
}-->
```http
PATCH https://graph.microsoft.com/v1.0/me/events/{id}
Content-type: application/json
Content-length: 285

{
  "originalStartTimeZone": "originalStartTimeZone-value",
  "originalEndTimeZone": "originalEndTimeZone-value",
  "responseStatus": {
    "response": "",
    "time": "datetime-value"
  },
  "recurrence": null,
  "iCalUId": "iCalUId-value",
  "reminderMinutesBeforeStart": 99,
  "isReminderOn": true
}
```

##### <a name="response"></a>応答

以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.event"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 285

{
  "originalStartTimeZone": "originalStartTimeZone-value",
  "originalEndTimeZone": "originalEndTimeZone-value",
  "responseStatus": {
    "response": "",
    "time": "datetime-value"
  },
  "recurrence": null,  
  "iCalUId": "iCalUId-value",
  "reminderMinutesBeforeStart": 99,
  "isReminderOn": true
}
```

## <a name="see-also"></a>関連項目

- [拡張機能を使用してカスタム データをリソースに追加する](../../../concepts/extensibility_overview.md)
- [オープン拡張機能を使用してカスタム データをユーザーに追加する](../../../concepts/extensibility_open_users.md)
- [スキーマ拡張機能を使用したグループへのカスタム データの追加](../../../concepts/extensibility_schema_groups.md)



<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Update event",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
