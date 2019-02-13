---
title: outlookTask を取得する
description: ユーザーのメールボックスにある Outlook タスクのプロパティとリレーションシップを取得します。
localization_priority: Normal
author: angelgolfer-ms
ms.prod: outlook
ms.openlocfilehash: f140734b6e5fa3e6488b71dbe183a9e3d82fc795
ms.sourcegitcommit: bdbc68ed8eaf43386d2cdf7b79e64ebbe1e860c0
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 02/13/2019
ms.locfileid: "29967292"
---
# <a name="get-outlooktask"></a>outlookTask を取得する

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

ユーザーのメールボックスにある Outlook タスクのプロパティとリレーションシップを取得します。

既定では、この操作 (および投稿、パッチ、および[完了](../api/outlooktask-complete.md)タスクの操作) は UTC の日付に関連するプロパティを返します。 `Prefer: outlook.timezone` ヘッダーを使用して、応答内のすべての日付関連プロパティを UTC 以外のタイム ゾーンで表すことができます。

## <a name="permissions"></a>アクセス許可

この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。

| アクセス許可の種類                        | アクセス許可 (特権の小さいものから大きいものへ) |
|:---------------------------------------|:------------------------------------|
| 委任 (職場または学校のアカウント)     | Tasks.Read                          |
| 委任 (個人用 Microsoft アカウント) | Tasks.Read                          |
| アプリケーション                            | サポートされていません。                      |

## <a name="http-request"></a>HTTP 要求

<!-- { "blockType": "ignored" } -->

```http
GET /me/outlook/tasks/{id}
GET /users/{id|userPrincipalName}/outlook/tasks/{id}
```

## <a name="optional-query-parameters"></a>オプションのクエリ パラメーター

このメソッドは、応答をカスタマイズするための [OData クエリ パラメーター](https://developer.microsoft.com/graph/docs/concepts/query_parameters)をサポートします。

## <a name="request-headers"></a>要求ヘッダー

| 名前                     | 説明                                       |
|:-------------------------|:--------------------------------------------------|
| Authorization            | ベアラー {トークン}。必須。                         |
| 優先: outlook.timezone | このヘッダーが指定されていない場合は、UTC である応答でタイム ゾーンの時刻のプロパティを指定します。 省略可能。 |

## <a name="request-body"></a>要求本文

このメソッドには、要求本文を指定しません。

## <a name="response"></a>応答

かどうかは成功すると、このメソッドが返されます、 `200 OK` 、応答の本体で応答コードと[outlookTask](../resources/outlooktask.md)のオブジェクトです。

## <a name="examples"></a>例

### <a name="example-1-get-an-outlook-task"></a>例 1: Outlook のタスクを取得します。

#### <a name="request"></a>要求

以下は、要求の例です。
<!-- {
  "blockType": "request",
  "name": "get_outlooktask"
}-->

```http
GET https://graph.microsoft.com/beta/me/outlook/tasks('AAMkADA1MTrgAAA=')
```

<!-- markdownlint-disable MD024 -->

#### <a name="response"></a>応答

以下は、応答の例です。 既定では、応答に含まれる日時のプロパティは UTC 形式になります。

> **注:** 簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。 実際の呼び出しではすべてのプロパティが返されます。

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.outlookTask"
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "id": "AAMkADA1MTrgAAA=",
  "createdDateTime": "2016-04-22T06:03:35.9279794Z",
  "lastModifiedDateTime": "2016-04-22T06:03:35.9436052Z",
  "changeKey": "1/KC9Vmu40G3DwB6Lgs7MAAAIOJMyQ==",
  "categories": [],
  "assignedTo": null,
  "body": {
    "contentType": "text",
    "content": ""
  },
  "completedDateTime": null,
  "dueDateTime": {
    "dateTime": "2016-04-27T04:00:00.0000000",
    "timeZone": "UTC"
  },
  "hasAttachments": false,
  "importance": "normal",
  "isReminderOn": false,
  "owner": "Administrator",
  "parentFolderId": "AQMkADA1MTBEgAAAA==",
  "recurrence": null,
  "reminderDateTime": null,
  "sensitivity": "normal",
  "startDateTime": {
    "dateTime": "2016-04-26T04:00:00.0000000",
    "timeZone": "UTC"
  },
  "status": "notStarted",
  "subject": "Shop for dinner"
}
```

### <a name="example-2-get-outlook-task-with-date-time-properties-in-pacific-standard-time"></a>例 2: 太平洋標準時の日付と時刻のプロパティを使用して Outlook のタスクを取得します。

#### <a name="request"></a>要求

この例では、 `Prefer: outlook.timezone` API が太平洋標準時の応答で日付と時刻のプロパティを返すことを指定するヘッダー。

<!-- {
  "blockType": "request",
  "name": "get_outlooktask"
}-->

```http
GET https://graph.microsoft.com/beta/me/outlook/tasks('AAMkADA1MHgwAAA=')
Prefer: outlook.timezone="Pacific Standard Time"
```

### <a name="response"></a>応答

以下は、応答の例です。 指定の太平洋標準時では、応答内の日付と時刻のプロパティが返されます。

> **注:** 簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。 実際の呼び出しではすべてのプロパティが返されます。

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.outlookTask"
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "id": "AAMkADA1MHgwAAA=",
  "createdDateTime": "2016-04-22T15:19:18.9526004-07:00",
  "lastModifiedDateTime": "2016-04-22T15:19:19.015101-07:00",
  "changeKey": "1/KC9Vmu40G3DwB6Lgs7MAAAIW9XXA==",
  "categories": [],
  "assignedTo": "Dana Swope",
  "body": {
    "contentType": "text",
    "content": ""
  },
  "completedDateTime": null,
  "dueDateTime": {
    "dateTime": "2016-05-04T021:00:00.0000000",
    "timeZone": "Pacific Standard Time"
  },
  "hasAttachments": false,
  "importance": "normal",
  "isReminderOn": false,
  "owner": "Administrator",
  "parentFolderId": "AQMkADA1MTEgAAAA==",
  "recurrence": null,
  "reminderDateTime": null,
  "sensitivity": "normal",
  "startDateTime": {
    "dateTime": "2016-05-02T21:00:00.0000000",
    "timeZone": "Pacific Standard Time"
  },
  "status": "notStarted",
  "subject": "Shop for children's weekend"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Get outlookTask",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/outlooktask-get.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
