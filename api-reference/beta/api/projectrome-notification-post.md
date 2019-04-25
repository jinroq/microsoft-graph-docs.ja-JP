---
title: 通知を作成し送信する
description: 'Microsoft Graph を使用してユーザーを対象にした通知を作成し、送信します。 通知は Microsoft Graph 通知フィードストアに格納され、ユーザーがサインインしているすべてのデバイスエンドポイント上のすべてのアプリクライアントに送信されます。  '
localization_priority: Normal
ms.prod: project-rome
ms.openlocfilehash: 70c7992a6fd323b909d948976132304fa04393c4
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32546399"
---
# <a name="create-and-send-a-notification"></a>通知を作成し送信する
[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Microsoft Graph を使用してユーザーを対象にした通知を作成し、送信します。 通知は Microsoft Graph 通知フィードストアに格納され、ユーザーがサインインしているすべてのデバイスエンドポイント上のすべてのアプリクライアントに送信されます。  
## <a name="permissions"></a>アクセス許可
この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。

|アクセス許可の種類      | アクセス許可 (特権の小さいものから大きいものへ)              |
|:--------------------|:---------------------------------------------------------|
|委任 (職場または学校のアカウント) | Notifications.ReadWrite.CreatedByApp    |
|委任 (個人用 Microsoft アカウント) | Notifications.ReadWrite.CreatedByApp    |

## <a name="http-request"></a>HTTP 要求

<!-- { "blockType": "ignored" } -->

```http
POST /me/notifications/
```
## <a name="request-headers"></a>要求ヘッダー
|名前 | 型 | 説明|
|:----|:-----|:-----------|
|Authorization | string |認証ヘッダーは、呼び出し元の資格情報を渡すために使用されます。 ベアラー {token}。 必須です。 |
## <a name="request-body"></a>要求本文
要求本文で、[通知](../resources/projectrome-notification.md)オブジェクトの JSON 表記を指定します。

## <a name="response"></a>応答
成功した場合、このメソッド`201 Created`は通知が正常に作成され、保存されたことを示す応答コードを返します。 
## <a name="example"></a>例
#### <a name="request"></a>要求
要求の例を次に示します。

```http
POST https://graph.microsoft.com/beta/me/notifications/
Content-type: application/json

{
    "targetHostName": "graphnotifications.sample.windows.com",
    "appNotificationId": "testDirectToastNotification",
    "expirationDateTime": "2018-08-29T23:51:33.000Z",
    "payload": {
        "visualContent": {
            "title": "Hello World!",
            "body": "Notifications are Great!"
        }
    },
    "targetPolicy": {
        "platformTypes": [
        "windows",
        "android"
        ]
    },
    "priority": "High",
    "groupName": "TestGroup",
    "displayTimeToLive": "23"
}
```

#### <a name="response"></a>応答
応答の例を次に示します。

```http
HTTP/1.1 201
Content-Type: application/json
location: https://graph.microsoft.com/beta/me/notifications/518c4fb1-c565-4d67-95c4-bcc3eb8eda1b

{
    "@odata.context": "https://graph.microsoft.com/test872018/$metadata#users('graphNotificationsUser%40contoso.com')/notifications/$entity",
    "appNotificationId": "testDirectToastNotification",
    "displayTimeToLive": 23,
    "expirationDateTime": "2018-08-24T12:31:53.858Z",
    "groupName": "TestGroup",
    "id": "cd5c5e6a-99ce-470a-9982-c47635e73620",
    "priority": "1",
    "payload": {
        "visualContent": {
            "title": "Hello World!",
            "body": "Notifications are Great!"
        }
    }
}
```


<!--
{
  "type": "#page.annotation",
  "suppressions": [
    "Error: /api-reference/beta/api/projectrome-notification-post.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
