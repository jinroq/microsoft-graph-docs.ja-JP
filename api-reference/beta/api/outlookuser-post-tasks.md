---
title: OutlookTask を作成します。
description: デフォルトのタスク グループに Outlook のタスクを作成する (`My Tasks`) と既定の作業フォルダー (`Tasks`) ユーザーのメールボックスにします。
localization_priority: Normal
author: angelgolfer-ms
ms.prod: outlook
ms.openlocfilehash: 04cc91f9c6eee09f71783d0548470d167911ec91
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/12/2019
ms.locfileid: "27925596"
---
# <a name="create-outlooktask"></a>OutlookTask を作成します。

> **重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。 実稼働アプリケーションでの、これらの API の使用はサポートされていません。

デフォルトのタスク グループに Outlook のタスクを作成する (`My Tasks`) と既定の作業フォルダー (`Tasks`) ユーザーのメールボックスにします。

POST メソッドは常に**させる**と、要求の本文では、 **dueDateTime**の時刻部分を無視し、指定されたタイム ゾーンで午前 0 時を常に時間を想定しています。

既定では、この操作 (と取得、パッチ、および[完了](../api/outlooktask-complete.md)タスクの操作) は UTC の日付に関連するプロパティを返します。 ヘッダーを使用して、応答内のすべての日付関連プロパティを UTC 以外のタイム ゾーンで表すことができます。`Prefer: outlook.timezone`

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
POST /users/{id|userPrincipalName}/outlook/tasks
```
## <a name="request-headers"></a>要求ヘッダー
| 名前       | 説明|
|:---------------|:----------|
| Authorization  | ベアラー {トークン}。必須。 |
| 優先: outlook.timezone | このヘッダーが指定されていない場合は、UTC である応答でタイム ゾーンの時刻のプロパティを指定します。 省略可能。|

## <a name="request-body"></a>要求本文
要求の本文には、 [outlookTask](../resources/outlooktask.md)オブジェクトの JSON 表現を指定します。

## <a name="response"></a>応答

かどうかは成功すると、このメソッドを返します`201 Created`、応答の本体で応答コードと[outlookTask](../resources/outlooktask.md)のオブジェクトです。

## <a name="example"></a>例
##### <a name="request"></a>要求
次の例を使用して、`Prefer: outlook.timezone`ヘッダー。 タスクを作成**させる**と**dueDateTime**東部標準時 (EST) で表されますが含まれています、`Prefer`ヘッダーの太平洋標準時 (PST) です。
<!-- {
  "blockType": "request",
  "name": "create_outlooktask_from_outlookuser"
}-->
```http
POST https://graph.microsoft.com/beta/me/outlook/tasks
Prefer: outlook.timezone="Pacific Standard Time"
Content-type: application/json
Content-length: 276

{
  "assignedTo": "Dana Swope",
  "subject": "Shop for children's weekend",
  "startDateTime": {
      "dateTime": "2016-05-03T09:00:00",
      "timeZone": "Eastern Standard Time"
  },
  "dueDateTime":  {
      "dateTime": "2016-05-05T16:00:00",
      "timeZone": "Eastern Standard Time"
  }
}
```
要求の本文には、 [outlookTask](../resources/outlooktask.md)オブジェクトの JSON 表現を指定します。
##### <a name="response"></a>応答
POST メソッドでは、**示す**および要求の本文では、 **dueDateTime**の時刻部分は無視され、指定されたタイム ゾーン (EST) の午前 0 時を常に時間を想定しています。

ヘッダーでは PST が指定されているため、POST メソッドは応答内のすべての日付関連プロパティを PST で表記します。`Prefer` 具体的には、**させる**と**dueDateTime**のプロパティの POST メソッドは EST の午前 0 時を PST に変換し、PST の応答で返します。

注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.outlookTask"
} -->
```http
HTTP/1.1 201 Created
Content-type: application/json
Content-length: 576

{
  "id": "AAMkADA1MHgwAAA=",
  "createdDateTime": "2016-04-22T15:19:18.9526004-07:00",
  "lastModifiedDateTime": "2016-04-22T15:19:19.015101-07:00",
  "changeKey": "1/KC9Vmu40G3DwB6Lgs7MAAAIW9XXA==",
  "categories": [ ],
  "assignedTo": "Dana Swope",
  "body": {
    "contentType": "Text",
    "content": ""
  },
  "completedDateTime": null,
  "dueDateTime": {
    "dateTime": "2016-05-04T021:00:00.0000000",
    "timeZone": "Pacific Standard Time"
  },
  "hasAttachments":false,
  "importance": "normal",
  "isReminderOn": false,
  "owner": "Administrator",
  "parentFolderId": "AQMkADA1MTEgAAAA==",
  "recurrence": null,
  "reminderDateTime": null,
  "sensitivity": "Normal",
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
<!-- {
  "type": "#page.annotation",
  "description": "Create outlookTask",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
