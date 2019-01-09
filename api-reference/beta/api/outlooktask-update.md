---
title: Outlooktask を更新します。
description: Outlook のタスクの書き込み可能なプロパティを変更します。
author: angelgolfer-ms
ms.openlocfilehash: 0cd4907c4ab1cb517ab2611cc4dc30431e496440
ms.sourcegitcommit: 6b1ba9b3be038cd6247de54a255bad560034fe42
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/08/2019
ms.locfileid: "27771731"
---
# <a name="update-outlooktask"></a>Outlooktask を更新します。

> **重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。 実稼働アプリケーションでの、これらの API の使用はサポートされていません。

Outlook のタスクの書き込み可能なプロパティを変更します。

**完全な**アクション、または明示的に修正プログラムの操作では、 **completedDateTime**プロパティを設定できます。 **状態**を設定するに**completedDateTime**の設定を確認して修正プログラムを使用する場合は、`completed`も同様です。

既定では、この操作 (および投稿、取得、および[完了](../api/outlooktask-complete.md)タスクの操作) は UTC の日付に関連するプロパティを返します。 ヘッダーを使用して、応答内のすべての日付関連プロパティを UTC 以外のタイム ゾーンで表すことができます。`Prefer: outlook.timezone`

## <a name="permissions"></a>アクセス許可

この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。

|アクセス許可の種類      | アクセス許可 (特権の小さいものから大きいものへ)              |
|:--------------------|:---------------------------------------------------------|
|委任 (職場または学校のアカウント) | Tasks.ReadWrite    |
|委任 (個人用 Microsoft アカウント) | Tasks.ReadWrite    |
|アプリケーション | サポートされていません。 |

## <a name="http-request"></a>HTTP 要求

<!-- { "blockType": "ignored" } -->

```http
PATCH /me/outlook/tasks/{id}
PATCH /users/{id|userPrincipalName}/outlook/tasks/{id}
```

## <a name="request-headers"></a>要求ヘッダー

| 名前       | 説明|
|:-----------|:-----------|
| Authorization  | ベアラー {トークン}。必須。 |
| 優先: outlook.timezone | このヘッダーが指定されていない場合は、UTC である応答でタイム ゾーンの時刻のプロパティを指定します。 省略可能。|

## <a name="request-body"></a>要求本文

要求本文で、更新する関連フィールドの値を指定します。要求本文に含まれない既存のプロパティは、以前の値のままになるか、他のプロパティ値の変化に基づいて再計算されます。最適なパフォーマンスを得るためには、変更されていない既存の値を含めないでください。

| プロパティ | 型 | 説明 |
|:---------------|:--------|:----------|
|担当者|String|タスクが割り当てられているユーザーの名前。|
|body|[itemBody](../resources/itembody.md)|通常はタスクに関する情報を含むタスク本体。HTML 型のみがサポートされていることに注意してください。|
|categories|String コレクション|タスクに関連付けられたカテゴリ。|
|changeKey|String|タスクのバージョン。|
|CompletedDateTime|[dateTimeTimeZone](../resources/datetimetimezone.md)|タスクが終了した日付 (指定のタイム ゾーン)。|
|createdDateTime|DateTimeOffset|日付と時刻、タスクが作成された日時です。 既定では、UTC であります。 要求ヘッダーにカスタム タイム ゾーンを使用できます。 プロパティの値は、ISO 8601 形式を使用します。 たとえば、2014 年 1 月 1 日午前 0 時 (UTC) は、次のようになります。`'2014-01-01T00:00:00Z'`|
|dueDateTime|[dateTimeTimeZone](../resources/datetimetimezone.md)|タスクが終了する予定の日時 (指定のタイム ゾーン)。|
|hasAttachments|Boolean|タスクに添付ファイルが含まれている場合、true に設定します。|
|importance|string|イベントの重要度。 可能な値は `low`、`normal`、`high` です。|
|isReminderOn|Boolean|ユーザーにタスクを通知するアラートを設定する場合は、true に設定します。|
|lastModifiedDateTime|DateTimeOffset|日付と、タスクが最後に修正されました。 既定では、UTC であります。 要求ヘッダーにカスタム タイム ゾーンを使用できます。 プロパティの値は、ISO 8601 形式を使用し、UTC 時刻が常に。 たとえば、2014 年 1 月 1 日午前 0 時 (UTC) は、次のようになります。`'2014-01-01T00:00:00Z'`|
|owner|String|タスクを作成したユーザーの名前。|
|parentFolderId|String|タスクの親フォルダーの一意の識別子。|
|recurrence|[patternedRecurrence](../resources/patternedrecurrence.md)|タスクの繰り返しパターン。|
|reminderDateTime|[dateTimeTimeZone](../resources/datetimetimezone.md)|タスクのアラーム通知を行う日時。|
|sensitivity|string|タスクのプライバシーのレベルを示します。 可能な値は、`normal`、`personal`、`private`、`confidential` です。|
|startDateTime|[dateTimeTimeZone](../resources/datetimetimezone.md)|タスクを開始する日付 (指定のタイム ゾーン)。|
|status|string|状態またはタスクの進行状況を示します。 可能な値は、`notStarted`、`inProgress`、`completed`、`waitingOnOthers`、`deferred` です。|
|subject|String|タスクのタイトルまたは簡単な説明。|

## <a name="response"></a>応答

かどうかは成功すると、このメソッドが返されます、`200 OK`応答コードおよび応答の本文の更新された[outlookTask](../resources/outlooktask.md)オブジェクトです。

## <a name="example"></a>例

### <a name="request"></a>要求

次の使用例は、 **dueDateTime**プロパティを変更してを使用して、`Prefer: outlook.timezone`の東部標準時 (EST) の応答での日付に関連するプロパティを表現することを指定するヘッダー。
<!-- {
  "blockType": "request",
  "name": "update_outlooktask"
}-->

```http
PATCH https://graph.microsoft.com/beta/me/outlook/tasks('AAMkADA1MTHgwAAA=')

Prefer: outlook.timezone="Eastern Standard Time"
Content-type: application/json
Content-length: 76

{
  "dueDateTime":  {
      "dateTime": "2016-05-06T16:00:00",
      "timeZone": "Eastern Standard Time"
  }
}
```

### <a name="response"></a>応答

以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.outlookTask"
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 376

{
    "id": "AAMkADA1MTHgwAAA=",
    "createdDateTime": "2016-04-22T18:19:18.9526004-04:00",
    "lastModifiedDateTime": "2016-04-22T18:38:20.5541528-04:00",
    "changeKey": "1/KC9Vmu40G3DwB6Lgs7MAAAIW9XXg==",
    "categories": [
    ],
    "assignedTo": null,
    "body": {
        "contentType": "text",
        "content": ""
    },
    "completedDateTime": null,
    "dueDateTime": {
        "dateTime": "2016-05-06T00:00:00.0000000",
        "timeZone": "Eastern Standard Time"
    },
    "hasAttachments":false,
    "importance": "normal",
    "isReminderOn": false,
    "owner": "Administrator",
    "parentFolderId": "AQMkADA1MTIBEgAAAA==",
    "recurrence": null,
    "reminderDateTime": null,
    "sensitivity": "normal",
    "startDateTime": {
        "dateTime": "2016-05-03T00:00:00.0000000",
        "timeZone": "Eastern Standard Time"
    },
    "status": "notStarted",
    "subject": "Shop for children's weekend"

}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Update outlooktask",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->