---
title: websocket エンドポイントを取得する
description: 実稼働アプリケーションでは、これらの API の使用はサポートされていません。
localization_priority: Normal
ms.prod: sharepoint
ms.openlocfilehash: c1f4d793655c2f51454bbd58303d1f6141b46cc5
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/26/2019
ms.locfileid: "33325397"
---
# <a name="get-websocket-endpoint"></a><span data-ttu-id="15c80-103">websocket エンドポイントを取得する</span><span class="sxs-lookup"><span data-stu-id="15c80-103">Get websocket endpoint</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]
<span data-ttu-id="15c80-104">実稼働アプリケーションでは、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="15c80-104">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="15c80-105">[socket.io][]を使用して、[ドライブ][]のほぼリアルタイムの変更通知を受け取ることができます。</span><span class="sxs-lookup"><span data-stu-id="15c80-105">Allows you to receive near-real-time change notifications for a [drive][] using [socket.io][].</span></span>
<span data-ttu-id="15c80-106">Socket.io は、websocket を利用する JavaScript の一般的な通知ライブラリです。</span><span class="sxs-lookup"><span data-stu-id="15c80-106">Socket.io is a popular notifications library for JavaScript that utilizes WebSockets.</span></span> <span data-ttu-id="15c80-107">詳細については、「 [socket.io](https://socket.io)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="15c80-107">To learn more, see [socket.io](https://socket.io).</span></span>

[ドライブ]: ../resources/drive.md
[drive]: ../resources/drive.md
[socket.io]: https://socket.io/

## <a name="permissions"></a><span data-ttu-id="15c80-110">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="15c80-110">Permissions</span></span>

<span data-ttu-id="15c80-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="15c80-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="15c80-113">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="15c80-113">Permission type</span></span>                        | <span data-ttu-id="15c80-114">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="15c80-114">Permissions (from least to most privileged)</span></span>
|:---------------------------------------|:-------------------------------------------
| <span data-ttu-id="15c80-115">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="15c80-115">Delegated (work or school account)</span></span>     | <span data-ttu-id="15c80-116">ファイル。読み取り、ファイルの読み取り/書き込み。すべてのファイル。</span><span class="sxs-lookup"><span data-stu-id="15c80-116">Files.Read, Files.ReadWrite, Files.ReadWrite.All, Sites.ReadWrite.All</span></span>
| <span data-ttu-id="15c80-117">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="15c80-117">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="15c80-118">ファイル。読み取り、ファイルの読み取り/書き込み。</span><span class="sxs-lookup"><span data-stu-id="15c80-118">Files.Read, Files.ReadWrite, Files.ReadWrite.All</span></span>
| <span data-ttu-id="15c80-119">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="15c80-119">Application</span></span>                            | <span data-ttu-id="15c80-120">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="15c80-120">Not supported.</span></span>

## <a name="http-request"></a><span data-ttu-id="15c80-121">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="15c80-121">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /me/drive/root/subscriptions/socketIo
GET /drives/{driveId}/root/subscriptions/socketIo
GET /groups/{groupId}/drive/root/subscriptions/socketIo
GET /sites/{siteId}/lists/{listId}/drive/root/subscriptions/socketIo
```

## <a name="example"></a><span data-ttu-id="15c80-122">例</span><span class="sxs-lookup"><span data-stu-id="15c80-122">Example</span></span>

### <a name="request"></a><span data-ttu-id="15c80-123">要求</span><span class="sxs-lookup"><span data-stu-id="15c80-123">Request</span></span>

<!-- { "blockType": "request", "name": "drive_root_subscriptions_socketIo" } -->
```http
GET /me/drive/root/subscriptions/socketIo
```

### <a name="response"></a><span data-ttu-id="15c80-124">応答</span><span class="sxs-lookup"><span data-stu-id="15c80-124">Response</span></span>

<span data-ttu-id="15c80-125">成功した場合、このメソッド`200 OK`は応答コードと、応答本文で[subscription](../resources/subscription.md)オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="15c80-125">If successful, this method returns a `200 OK` response code and a [subscription](../resources/subscription.md) object in the response body.</span></span>

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

<span data-ttu-id="15c80-126">返さ`notificationUrl`れるのは、socket.io エンドポイントの URL です。</span><span class="sxs-lookup"><span data-stu-id="15c80-126">The `notificationUrl` returned is a socket.io endpoint URL.</span></span>
<span data-ttu-id="15c80-127">socket.io クライアントでこれを使用するには、 `/callback?`トークンの文字列を分割します。</span><span class="sxs-lookup"><span data-stu-id="15c80-127">To use it with a socket.io client, split the string on the `/callback?` token.</span></span>
<span data-ttu-id="15c80-128">before `/callback?`文字列の部分は socket.io エンドポイント URL で、after 文字列の部分は、ライブラリに指定する必要がある非透過のクエリ文字列です。</span><span class="sxs-lookup"><span data-stu-id="15c80-128">The part of the string before `/callback?` is the socket.io endpoint URL and the part of the string after is an opaque query string that must be given to the libary.</span></span>

<span data-ttu-id="15c80-129">次の例は、 `notificationUrl` JavaScript で with socket.io を使用する方法を示しています。</span><span class="sxs-lookup"><span data-stu-id="15c80-129">The following example shows how to use the `notificationUrl` with socket.io in JavaScript.</span></span>

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

