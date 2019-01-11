---
title: Websocket のエンドポイントを取得します。
description: 実稼働アプリケーションでの、これらの API の使用はサポートされていません。
localization_priority: Normal
ms.openlocfilehash: a981a4d02d2e40fec0cb2bca397c7b7794d36867
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/11/2019
ms.locfileid: "27859795"
---
# <a name="get-websocket-endpoint"></a>Websocket のエンドポイントを取得します。

> **重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。
実稼働アプリケーションでの、これらの API の使用はサポートされていません。

[Socket.io][]を使用して[ドライブ][]の近くにあるリアルタイム変更通知を受信できます。
Socket.io は、Websocket を使用している javascript のコードの一般的な通知ライブラリです。 詳細については、 [socket.io](https://socket.io)を参照してください。

[ドライブ]: ../resources/drive.md
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

<!-- {
  "type": "#page.annotation"
}-->
