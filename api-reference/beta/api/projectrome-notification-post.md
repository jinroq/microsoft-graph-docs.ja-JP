---
title: 作成し、通知を送信します。
description: '作成し、Microsoft Graph を使用してユーザーを対象とする通知を送信します。 通知は、フィード ストア、Microsoft Graph の通知に格納され、ユーザーがサインインしてデバイスのすべてのエンドポイント上のすべてのアプリケーション クライアントに送信されます。  '
localization_priority: Normal
ms.prod: project-rome
ms.openlocfilehash: d8258e0da04f199a0f40bdb2a2ec85e01d5d5faf
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/12/2019
ms.locfileid: "27975933"
---
# <a name="create-and-send-a-notification"></a>作成し、通知を送信します。
> **重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。 実稼働アプリケーションでの、これらの API の使用はサポートされていません。

作成し、Microsoft Graph を使用してユーザーを対象とする通知を送信します。 通知は、フィード ストア、Microsoft Graph の通知に格納され、ユーザーがサインインしてデバイスのすべてのエンドポイント上のすべてのアプリケーション クライアントに送信されます。  
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
|名前 | 種類 | 説明|
|:----|:-----|:-----------|
|Authorization | string |承認ヘッダーを使用して、呼び出し元の関係者の資格情報を渡します。 ベアラー {トークンが記述されています。 必須。 |
## <a name="request-body"></a>要求本文
要求の本文には、[通知](../resources/projectrome-notification.md)オブジェクトの JSON の形式を指定します。

## <a name="response"></a>応答
かどうかは成功すると、このメソッドが返されます、 `201 Created` 、通知が正常に作成され保存されていることを示す応答コード。 
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


