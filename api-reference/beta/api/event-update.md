---
title: イベントの更新
description: イベント オブジェクトのプロパティを更新します。
author: angelgolfer-ms
localization_priority: Normal
ms.prod: outlook
ms.openlocfilehash: b3f101c14a69c6dc2b3687e9d4a1509e6ac7a531
ms.sourcegitcommit: d95f6d39a0479da6e531f3734c4029dc596b9a3f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/30/2019
ms.locfileid: "29643952"
---
# <a name="update-event"></a>イベントの更新

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

[イベント](../resources/event.md)オブジェクトのプロパティを更新します。
## <a name="permissions"></a>アクセス許可
この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。

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
| Authorization  | string  | ベアラー {トークン}。必須。 |

## <a name="request-body"></a>要求本文
要求本文で、更新する関連フィールドの値を指定します。要求本文に含まれない既存のプロパティは、以前の値のままになるか、他のプロパティ値の変化に基づいて再計算されます。最適なパフォーマンスを得るためには、変更されていない既存の値を含めないでください。

| プロパティ       | 型    | 説明 |
|:---------------|:--------|:------------|
| attendees|Attendee|イベントの出席者のコレクション。|
| body|ItemBody|イベントに関連付けられたメッセージの本文。|
| categories|String|イベントに関連付けられたカテゴリ。|
| end|DateTimeTimeZone|イベントが終了する日時。<br/><br/>既定で、終了時刻は UTC 単位です。EndTimeZone でオプションのタイム ゾーンを指定して、そのタイム ゾーンで終了時刻を表現し、UTC からの時間オフセットを含めることができます。EndTimeZone を使用する場合、StartTimeZone の値も指定する必要があります。<br/><br/>この例では、太平洋標準時で 2015 年 2 月 25 日午後 9:34 を指定します ("2015-02-25T21:34:00-08:00")。 |
| importance|String|イベントの重要度。 可能な値は `low`、`normal`、`high` です。|
| isAllDay|Boolean|イベントが一日中続く場合に、true に設定します。|
| isReminderOn|Boolean|ユーザーにイベントを通知するアラートを設定する場合は、true に設定します。|
| location|Location|イベントの場所。|
|locations|[Location](../resources/location.md) コレクション|イベントを開催する場所、または参加者がいる場所。 **location** プロパティと **locations** プロパティは常に互いに一致します。 **location** プロパティを更新すると、**locations** コレクションに含まれる既存のすべての場所が削除されて、**location** の新しい値に置き換えられます。 |
| recurrence|PatternedRecurrence|イベントの繰り返しパターン。|
| reminderMinutesBeforeStart|Int32|アラーム通知を行う、イベント開始時間前の分数。|
| responseRequested|Boolean|イベントが承諾または辞退されたときに、送信者が応答を要求する場合に、true に設定します。|
| sensitivity|String| 可能な値は、`normal`、`personal`、`private`、`confidential` です。|
| showAs|String|表示するステータス。 使用可能な値: `free` 、 `tentative`、 `busy`、 `oof`、 `workingElsewhere`、 `unknown`。|
| 開始|DateTimeTimeZone|イベントの開始時刻です。 <br/><br/>既定で、開始時刻は UTC 単位です。EndTimeZone でオプションのタイム ゾーンを指定して、そのタイム ゾーンで開始時刻を表現し、UTC からの時間オフセットを含めることができます。StartTimeZone を使用する場合、EndTimeZone の値も指定する必要があります。<br/><br/>この例では、太平洋標準時で 2015 年 2 月 25 日午後 7:34 を指定します "2015-02-25T19:34:00-08:00".  |
| subject|String|イベントの件名行のテキスト。|

**イベント**のリソースは、[拡張機能](/graph/extensibility-overview)をサポートするため、使用して、`PATCH`を追加、更新、または既存の**イベント**インスタンスで拡張機能のカスタム プロパティに独自のアプリケーション固有データを削除する操作です。

更新する**イベント**がマスターし、定期的な一連のイベントの場合は、複数の出席者が含まれていて、個別に更新されたインスタンス、複数の通知の電子メールが送信されます: マスターのシリーズとは、インスタンスごとに 1 つのいずれか更新されました。

## <a name="response"></a>応答

成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で、更新された [event](../resources/event.md) オブジェクトを返します。

>**注:** このメソッドは、HTTP 400 正しくない要求を含む応答のエラー コードを返すことができます`ErrorOccurrenceCrossingBoundary`し、次のエラー メッセージ: 変更されたアイテムを越えるまたは隣接するアイテムが重複しています。 更新プログラムには、定期的なアイテムの例外では、以下の Outlook 制限が違反していることを示します: 発生または日の前の出現箇所では、前日に移動することはできませんし、出現する位置は、次の日の前後に移動することはできません。

## <a name="example"></a>例

##### <a name="request"></a>要求

以下は、要求の例です。
<!-- {
  "blockType": "request",
  "name": "update_event"
}-->
```http
PATCH https://graph.microsoft.com/beta/me/events/{id}
Content-type: application/json
Content-length: 285

{
  "originalStartTimeZone": "originalStartTimeZone-value",
  "originalEndTimeZone": "originalEndTimeZone-value",
  "responseStatus": {
    "response": "",
    "time": "2016-10-19T10:37:00Z"
  },
  "recurrence": null,
  "uid": "iCalUId-value",
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
    "time": "2016-10-19T10:37:00Z"
  },
  "recurrence": null,
  "uid": "iCalUId-value",
  "reminderMinutesBeforeStart": 99,
  "isReminderOn": true
}
```


## <a name="see-also"></a>関連項目

- [拡張機能を使用してカスタム データをリソースに追加する](/graph/extensibility-overview)
- [オープン拡張機能を使用したユーザーへのカスタム データの追加 (プレビュー)](/graph/extensibility-open-users)
- [スキーマ拡張機能を使用したグループへのカスタム データの追加 (プレビュー)](/graph/extensibility-schema-groups)


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Update event",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/event-update.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
