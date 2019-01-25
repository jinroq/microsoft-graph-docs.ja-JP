---
title: Websocket のエンドポイントを取得します。
description: 実稼働アプリケーションでこれらの API を使用することは、サポートされていません。
localization_priority: Normal
ms.prod: sharepoint
ms.openlocfilehash: 736684812d2cbc10affed82a3f946d75731f6768
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/24/2019
ms.locfileid: "29519795"
---
# <a name="get-websocket-endpoint"></a>Websocket のエンドポイントを取得します。

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]
実稼働アプリケーションでこれらの API を使用することは、サポートされていません。

[Socket.io][]を使用して[ドライブ][]の近くにあるリアルタイム変更通知を受信できます。
Socket.io は、Websocket を使用している javascript のコードの一般的な通知ライブラリです。 詳細については、 [socket.io](https://socket.io)を参照してください。

[drive]: ../resources/drive.md
[socket.io]: https://socket.io/

## <a name="permissions"></a>アクセス許可

この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。

| アクセス許可の種類                        | アクセス許可 (特権の小さいものから大きいものへ)
|:---------------------------------------|:-------------------------------------------
| 委任 (職場または学校のアカウント)     | Files.Read、Files.ReadWrite、Files.ReadWrite.All、Sites.ReadWrite.All
| 委任 (個人用 Microsoft アカウント) | Files.Read、Files.ReadWrite、Files.ReadWrite.All
| アプリケーション                            | サポートされていません。

## <a name="http-request"></a>HTTP 要求

<!-- { "blockType": "ignored" } -->

```http
GET /me/drive/root/subscriptions/socketIo
GET /drives/{driveId}/root/subscriptions/socketIo
GET /groups/{groupId}/drive/root/subscriptions/socketIo
GET /sites/{siteId}/lists/{listId}/drive/root/subscriptions/socketIo
```

## <a name="example"></a>例

### <a name="request"></a>要求

<!-- { "blockType": "request", "name": "drive_root_subscriptions_socketIo" } -->
```http
GET /me/drive/root/subscriptions/socketIo
```

### <a name="response"></a>応答

かどうかは成功すると、このメソッドが返されます、`200 OK`応答コードおよび応答の本文の[サブスクリプション](../resources/subscription.md)オブジェクトです。

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.subscription"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "id": "opaqueId-fj3hd7yf283jfk193726nvc2w3i2diemdu8",
  "notificationUrl": "https://f3hb0mpua.svc.ms/zbaehwg/callback?snthgk=1ff3-2345672zz831837523"
}
```

`notificationUrl`は、socket.io のエンドポイントの URL が返されます。
Socket.io クライアントを使用してこれを使用するに、文字列を分割する、`/callback?`トークンです。
前に文字列の中で`/callback?`socket.io のエンドポイントの URL は、後の文字列の中でライブラリを指定する必要がありますが、不透明なクエリ文字列です。

使用する方法の例を次の`notificationUrl`JavaScript で socket.io をします。

```javascript
// this is the notificationUrl returned from this API
var notificationUrl = "https://f3hb0mpua.svc.ms/zbaehwg/callback?snthgk=1ff3-2345672zz831837523";

// after the split, split[0] will be everything leading up to '/callback?' and split[1] will be everything after.
var split = notificationUrl.split("/callback?");

// 'io' comes from the socket.io client library
var socket = io(split[0], { query: split[1] });

// these examples log to the console.
// your app would provide its own callbacks
socket.on("connect", ()=>console.log("Connected!"));
socket.on("notification", (data)=>console.log("Notification!", data));
```

<!--
{
  "type": "#page.annotation",
  "suppressions": [
    "Error: /api-reference/beta/api/driveItem-subscriptions-socketio.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
