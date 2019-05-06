---
title: 'イベント: デルタ'
description: '**calendarView** において追加、削除、更新された一連のイベント (さまざまなイベント) を取得します。 '
localization_priority: Priority
author: angelgolfer-ms
ms.prod: outlook
ms.openlocfilehash: 7eb8a80f8e857edc9aa9ff8781fae01dc1476677
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32562854"
---
# <a name="event-delta"></a>イベント: デルタ

ユーザーの標準として設定されている予定表の**calendarView** において追加、削除、更新された一連のイベント (さまざまなイベント) を取得します。

イベントの**デルタ**関数呼び出しは、ユーザーの標準として設定されている予定表のさまざまな日付に対する `GET /calendarview` 要求に似ていますが、これら 1 つ以上の呼び出しにおいて[状態トークン](/graph/delta-query-overview)を適切に適用することにより、そのカレンダー ビュー内における増分変化に対してクエリを実行できる点が異なります。これにより、標準として設定されている予定表のユーザー イベントのローカル格納の保守と同期を行う際に、サーバーからその予定表のイベントすべてを毎回フェッチする必要がなくなります。

## <a name="permissions"></a>アクセス許可
この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。


|アクセス許可の種類      | アクセス許可 (特権の小さいものから大きいものへ)              |
|:--------------------|:---------------------------------------------------------|
|委任 (職場または学校のアカウント) | Calendars.Read    |
|委任 (個人用 Microsoft アカウント) | Calendars.Read    |
|アプリケーション | Calendars.Read |

## <a name="http-request"></a>HTTP 要求
<!-- { "blockType": "ignored" } -->
```http
GET /me/calendarView/delta?startDateTime={start_datetime}&endDateTime={end_datetime}
GET /users/{id}/calendarView/delta?startDateTime={start_datetime}&endDateTime={end_datetime}

```

## <a name="query-parameters"></a>クエリ パラメーター

イベントの変化を追跡することにより、1 回以上の、一連の**デルタ**関数呼び出しが発生します。任意のクエリ パラメーター (`$deltatoken` と `$skiptoken` 以外) を使用する場合は、最初の**デルタ**要求でこれを指定する必要があります。Microsoft Graph は、応答で提供される `nextLink` または `deltaLink` の URL のトークン部分に指定したパラメーターを自動的にエンコードします。必要なクエリ パラメーターを前もって指定しておくだけで済みます。それ以降の要求では、前の応答で `nextLink` または `deltaLink` の URL に必要なパラメーターが既にエンコードされ、含まれているため、この URL をコピーして適用します。


| クエリ パラメーター      | 種類   |説明|
|:---------------|:--------|:----------|
|startDateTime|String|時間範囲の開始日時は、ISO 8601 形式で表されます。例: "2015-11-08T19:00:00.0000000"。|
|endDateTime|String|時間範囲の終了日時は、ISO 8601 形式で表されます。例: "2015-11-08T20:00:00.0000000"。|
| $deltatoken | string | 同じカレンダー ビュー用の前の**デルタ**関数呼び出しの `deltaLink` URL で返された[状態トークン](/graph/delta-query-overview)で、その一連の変更追跡が完了したことを示します。このトークンを含む `deltaLink` URL 全体を、該当カレンダー ビュー用の次回の一連の変更追跡の最初の要求内に保存し、適用します。|
| $skiptoken | string | 前の**デルタ**関数呼び出しの `nextLink` URL 内で返された[状態トークン](/graph/delta-query-overview)で、同じカレンダー ビュー内に追跡されるべきさらなる変化があることを示しています。 |

カレンダー ビューでデルタ クエリを実行する場合、`GET /calendarview` 要求で通常得られるプロパティのすべてを得られると予期します。この場合、`$select` はサポートされていません。 


## <a name="request-headers"></a>要求ヘッダー
| 名前       | 型 | 説明 |
|:---------------|:----------|:----------|
| Authorization  | string  | ベアラー {トークン}。必須。 |
| Content-Type  | string  | application/json. Required. |
| Prefer | string  | odata.maxpagesize={x}.省略可能。 |
| Prefer | string | {タイム ゾーン}。省略可能。指定しない場合、UTC が使用されます。|

## <a name="response"></a>応答

成功した場合、このメソッドは `200 OK` の応答コードと、応答本文で [イベント](../resources/event.md) コレクション オブジェクトを返します。

## <a name="example"></a>例
##### <a name="request"></a>要求

次の例では、1 回の**デルタ**関数呼び出しを行い、応答本文中のイベントの最大数を 2 に制限する方法を示します。

カレンダー ビュー内の変更を追跡するには、1 回以上の**デルタ**関数呼び出しを作成し、適切な[状態トークン](/graph/delta-query-overview)を使用して、前回のデルタ クエリ以降になされた一連の増分変更を取得します。 

<!-- {
  "blockType": "request",
  "name": "event_delta"
}-->
```http
GET https://graph.microsoft.com/v1.0/me/calendarView/delta?startdatetime={start_datetime}&enddatetime={end_datetime}

Prefer: odata.maxpagesize=2
```

##### <a name="response"></a>応答
要求が成功した場合、応答に含まれる状態トークンは、_スキップ トークン_ (_@odata.nextLink_ 応答ヘッダーに含まれる) か、_デルタ トークン_ (_@odata.deltaLink_ 応答ヘッダーに含まれる) のいずれかになります。前者はその回を続行する必要があることを示し、後者はその回のすべての変更の取得が完了したことを示します。

以下の応答は、_@odata.nextLink_ 応答ヘッダーに含まれる _skipToken_ を示しています。

注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.event",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 359

{
  "@odata.nextLink":"https://graph.microsoft.com/v1.0/me/calendarView/delta?$skiptoken={_skipToken_}",
  "value": [
    {
      "originalStartTimeZone": "originalStartTimeZone-value",
      "originalEndTimeZone": "originalEndTimeZone-value",
      "responseStatus": {
        "response": "response-value",
        "time": "datetime-value"
      },
      "iCalUId": "iCalUId-value",
      "reminderMinutesBeforeStart": 99,
      "isReminderOn": true
    }
  ]
}
```

### <a name="see-also"></a>関連項目

- [デルタ クエリを使用して、Microsoft Graph データの変更を追跡する](/graph/delta-query-overview)
- [カレンダー内のイベントの増分の変更を取得する](/graph/delta-query-events)

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "event: delta",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
