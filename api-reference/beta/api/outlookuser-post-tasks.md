---
title: outlooktask の作成
description: ユーザーのメールボックスの既定のタスクグループ (`My Tasks`) および既定のタスクフォルダー`Tasks`() に Outlook のタスクを作成します。
localization_priority: Normal
author: angelgolfer-ms
ms.prod: outlook
ms.openlocfilehash: 4de57847638ef98347a7561291d12486468428ee
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32539649"
---
# <a name="create-outlooktask"></a>outlooktask の作成

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

ユーザーのメールボックスの既定のタスクグループ (`My Tasks`) および既定のタスクフォルダー`Tasks`() に Outlook のタスクを作成します。

POST メソッドは、要求本文の**startDateTime**および**dueDateTime**の時間部分を常に無視し、指定されたタイムゾーンで常に深夜になる時刻を想定します。

既定では、この操作 (およびタスクの取得、パッチ、[完了](../api/outlooktask-complete.md)) は、日付関連プロパティを UTC で返します。 `Prefer: outlook.timezone` ヘッダーを使用して、応答内のすべての日付関連プロパティを UTC 以外のタイム ゾーンで表すことができます。

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
POST /me/outlook/tasks
POST /users/{id|userPrincipalName}/outlook/tasks
```
## <a name="request-headers"></a>要求ヘッダー
| 名前       | 説明|
|:---------------|:----------|
| Authorization  | ベアラー {トークン}。必須。 |
| 優先: outlook.timezone | 応答の時間プロパティのタイムゾーンを指定します。このヘッダーが指定されていない場合は、UTC になります。 省略可能。|

## <a name="request-body"></a>要求本文
要求本文で、 [outlooktask](../resources/outlooktask.md)オブジェクトの JSON 表記を指定します。

## <a name="response"></a>応答

成功した場合、この`201 Created`メソッドは応答コードと、応答本文で[outlooktask](../resources/outlooktask.md)オブジェクトを返します。

## <a name="example"></a>例
##### <a name="request"></a>要求
次の例は、 `Prefer: outlook.timezone`ヘッダーの使用方法を示しています。 この例では、タスクを作成し、 **startDateTime**と**dueDateTime**を東部標準時 (EST) で表し`Prefer` 、太平洋標準時 (PST) のヘッダーを含みます。
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
要求本文で、 [outlooktask](../resources/outlooktask.md)オブジェクトの JSON 表記を指定します。
##### <a name="response"></a>応答
POST メソッドは、要求本文の**startDateTime**および**dueDateTime**の時間部分を無視し、指定されたタイムゾーン (EST) で常に午前0時になる時間を想定します。

`Prefer` ヘッダーでは PST が指定されているため、POST メソッドは応答内のすべての日付関連プロパティを PST で表記します。 特に、 **startDateTime**プロパティと**dueDateTime**プロパティの場合、POST メソッドは EST の午前0時を pst に変換し、それらを応答で pst で返します。

注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。実際の呼び出しではすべてのプロパティが返されます。
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
<!--
{
  "type": "#page.annotation",
  "description": "Create outlookTask",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/outlookuser-post-tasks.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
