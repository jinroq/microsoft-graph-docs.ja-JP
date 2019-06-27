---
title: Outlooktask) を更新する
description: Outlook タスクの書き込み可能なプロパティを変更します。
author: angelgolfer-ms
localization_priority: Normal
ms.prod: outlook
ms.openlocfilehash: 4967be08228990dc8921780928db1c4c24c2be9b
ms.sourcegitcommit: 0e1101d499f35b08aa2309e273871438b1774979
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/27/2019
ms.locfileid: "35266809"
---
# <a name="update-outlooktask"></a>Outlooktask) を更新する

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Outlook タスクの書き込み可能なプロパティを変更します。

**CompletedDateTime**プロパティは、**完全な**アクションによって、または明示的に PATCH 操作によって設定できます。 PATCH を使用して**completedDateTime**を設定する場合は、**状態**も`completed`同様にに設定してください。

既定では、この操作 (および POST、GET、および[完了](../api/outlooktask-complete.md)タスク操作) は、日付関連プロパティを UTC で返します。 `Prefer: outlook.timezone` ヘッダーを使用して、応答内のすべての日付関連プロパティを UTC 以外のタイム ゾーンで表すことができます。

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
| 優先: outlook.timezone | 応答の時間プロパティのタイムゾーンを指定します。このヘッダーが指定されていない場合は、UTC になります。 省略可能。|

## <a name="request-body"></a>要求本文

要求本文で、更新する関連フィールドの値を指定します。要求本文に含まれない既存のプロパティは、以前の値のままになるか、他のプロパティ値の変化に基づいて再計算されます。最適なパフォーマンスを得るためには、変更されていない既存の値を含めないでください。

| プロパティ | 型 | 説明 |
|:---------------|:--------|:----------|
|assignedTo|String|タスクが割り当てられているユーザーの名前。|
|body|[itemBody](../resources/itembody.md)|通常はタスクに関する情報を含むタスク本体。HTML 型のみがサポートされていることに注意してください。|
|categories|String コレクション|タスクに関連付けられたカテゴリ。|
|changeKey|String|タスクのバージョン。|
|completedDateTime|[dateTimeTimeZone](../resources/datetimetimezone.md)|タスクが終了した日付 (指定のタイム ゾーン)。|
|createdDateTime|DateTimeOffset|タスクが作成された日時。 既定では、UTC 時間です。 要求ヘッダーでカスタム タイム ゾーンを使用できます。 プロパティの値は、ISO 8601 形式を使用します。 たとえば、2014 年 1 月 1 日午前 0 時 (UTC) は、`'2014-01-01T00:00:00Z'` のようになります。|
|dueDateTime|[dateTimeTimeZone](../resources/datetimetimezone.md)|タスクが終了する予定の日時 (指定のタイム ゾーン)。|
|hasAttachments|ブール値|タスクに添付ファイルが含まれている場合、true に設定します。|
|importance|string|イベントの重要度。 可能な値は、`low`、`normal`、`high` です。|
|isReminderOn|Boolean|ユーザーにタスクを通知するアラートを設定する場合は、true に設定します。|
|lastModifiedDateTime|DateTimeOffset|タスクが最後に変更された日時。 既定では、UTC 時間です。 要求ヘッダーでカスタム タイム ゾーンを使用できます。 プロパティの値は、ISO 8601 形式を使って表され、常に UTC 時間です。 たとえば、2014 年 1 月 1 日午前 0 時 (UTC) は、`'2014-01-01T00:00:00Z'` のようになります。|
|owner|String|タスクを作成したユーザーの名前。|
|parentFolderId|String|タスクの親フォルダーの一意の識別子。|
|recurrence|[patternedRecurrence](../resources/patternedrecurrence.md)|タスクの繰り返しパターン。|
|reminderDateTime|[dateTimeTimeZone](../resources/datetimetimezone.md)|タスクのアラーム通知を行う日時。|
|sensitivity|string|タスクのプライバシーのレベルを示します。 使用可能な値は、`normal`、`personal`、`private`、`confidential` です。|
|startDateTime|[dateTimeTimeZone](../resources/datetimetimezone.md)|タスクを開始する日付 (指定のタイム ゾーン)。|
|status|string|タスクの状態または進行状況を示します。 可能な値は、`notStarted`、`inProgress`、`completed`、`waitingOnOthers`、`deferred` です。|
|subject|String|タスクのタイトルまたは簡単な説明。|

## <a name="response"></a>応答

成功した場合、このメソッド`200 OK`は応答コードと、応答本文で更新された[outlooktask](../resources/outlooktask.md)オブジェクトを返します。

## <a name="example"></a>例

### <a name="request"></a>要求

次の例では、 **dueDateTime**プロパティを変更`Prefer: outlook.timezone`し、ヘッダーを使用して、応答の日付関連プロパティを東部標準時 (EST) で表現するように指定しています。
<!-- {
  "blockType": "request",
  "name": "update_outlooktask"
}-->

```http
PATCH https://graph.microsoft.com/beta/me/outlook/tasks/AAMkADA1MTHgwAAA=
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
#### <a name="sdk-sample-code"></a>SDK サンプル コード
# <a name="ctabcs"></a>[C#](#tab/cs)
[!INCLUDE [sample-code](../includes/update_outlooktask-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[Javascript](#tab/javascript)
[!INCLUDE [sample-code](../includes/update_outlooktask-Javascript-snippets.md)]

# <a name="objective-ctabobjective-c"></a>[目的-C](#tab/objective-c)
[!INCLUDE [sample-code](../includes/update_outlooktask-Objective-C-snippets.md)]
---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Update outlooktask",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/outlooktask-update.md:\r\n      BookmarkMissing: '[#tab/objective-c](Objective-C)'. Did you mean: #objective-c (score: 4)",
    "Error: /api-reference/beta/api/outlooktask-update.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/beta/api/outlooktask-update.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}
-->
