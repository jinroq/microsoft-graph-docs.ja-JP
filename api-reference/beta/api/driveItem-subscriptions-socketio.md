---
title: Websocket エンドポイントを取得する
description: 実稼働アプリケーションでこれらの API を使用することは、サポートされていません。
localization_priority: Normal
ms.prod: sharepoint
ms.openlocfilehash: 03dbaf8522005c2bb0c038c8ba885becc41f72dc
ms.sourcegitcommit: b8d01acfc1cb7610a0e1f5c18065da415bae0777
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/06/2019
ms.locfileid: "33591820"
---
# <a name="get-websocket-endpoint"></a><span data-ttu-id="8a0e0-103">Websocket エンドポイントを取得する</span><span class="sxs-lookup"><span data-stu-id="8a0e0-103">Get websocket endpoint</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]
<span data-ttu-id="8a0e0-104">実稼働アプリケーションでこれらの API を使用することは、サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="8a0e0-104">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="8a0e0-105">[Socket.io][]を使用して、[ドライブ][]のほぼリアルタイムの変更通知を受け取ることができます。</span><span class="sxs-lookup"><span data-stu-id="8a0e0-105">Allows you to receive near-real-time change notifications for a [drive][] using [socket.io][].</span></span>
<span data-ttu-id="8a0e0-106">Socket.io は、Websocket を利用する JavaScript の一般的な通知ライブラリです。</span><span class="sxs-lookup"><span data-stu-id="8a0e0-106">Socket.io is a popular notifications library for JavaScript that utilizes WebSockets.</span></span> <span data-ttu-id="8a0e0-107">詳細については、「 [socket.io](https://socket.io)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="8a0e0-107">To learn more, see [socket.io](https://socket.io).</span></span>

[drive]: ../resources/drive.md
[socket.io]: https://socket.io/

## <a name="permissions"></a><span data-ttu-id="8a0e0-110">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="8a0e0-110">Permissions</span></span>

<span data-ttu-id="8a0e0-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="8a0e0-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="8a0e0-113">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="8a0e0-113">Permission type</span></span>                        | <span data-ttu-id="8a0e0-114">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="8a0e0-114">Permissions (from least to most privileged)</span></span>
|:---------------------------------------|:-------------------------------------------
| <span data-ttu-id="8a0e0-115">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="8a0e0-115">Delegated (work or school account)</span></span>     | <span data-ttu-id="8a0e0-116">ファイル。読み取り、ファイルの読み取り/書き込み。すべてのファイル。</span><span class="sxs-lookup"><span data-stu-id="8a0e0-116">Files.Read, Files.ReadWrite, Files.ReadWrite.All, Sites.ReadWrite.All</span></span>
| <span data-ttu-id="8a0e0-117">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="8a0e0-117">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="8a0e0-118">ファイル。読み取り、ファイルの読み取り/書き込み。</span><span class="sxs-lookup"><span data-stu-id="8a0e0-118">Files.Read, Files.ReadWrite, Files.ReadWrite.All</span></span>
| <span data-ttu-id="8a0e0-119">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="8a0e0-119">Application</span></span>                            | <span data-ttu-id="8a0e0-120">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="8a0e0-120">Not supported.</span></span>

## <a name="http-request"></a><span data-ttu-id="8a0e0-121">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="8a0e0-121">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /me/drive/root/subscriptions/socketIo
GET /drives/{driveId}/root/subscriptions/socketIo
GET /groups/{groupId}/drive/root/subscriptions/socketIo
GET /sites/{siteId}/lists/{listId}/drive/root/subscriptions/socketIo
```

## <a name="example"></a><span data-ttu-id="8a0e0-122">例</span><span class="sxs-lookup"><span data-stu-id="8a0e0-122">Example</span></span>

### <a name="request"></a><span data-ttu-id="8a0e0-123">要求</span><span class="sxs-lookup"><span data-stu-id="8a0e0-123">Request</span></span>

<!-- { "blockType": "request", "name": "drive_root_subscriptions_socketIo" } -->
```http
GET /me/drive/root/subscriptions/socketIo
```

### <a name="response"></a><span data-ttu-id="8a0e0-124">応答</span><span class="sxs-lookup"><span data-stu-id="8a0e0-124">Response</span></span>

<span data-ttu-id="8a0e0-125">成功した場合、このメソッド`200 OK`は応答コードと、応答本文で[subscription](../resources/subscription.md)オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="8a0e0-125">If successful, this method returns a `200 OK` response code and a [subscription](../resources/subscription.md) object in the response body.</span></span>

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
#### <a name="sdk-sample-code"></a><span data-ttu-id="8a0e0-126">SDK サンプルコード</span><span class="sxs-lookup"><span data-stu-id="8a0e0-126">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="8a0e0-127">Visual</span><span class="sxs-lookup"><span data-stu-id="8a0e0-127">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/drive_root_subscriptions_socketIo-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="8a0e0-128">Java</span><span class="sxs-lookup"><span data-stu-id="8a0e0-128">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/drive_root_subscriptions_socketIo-Javascript-snippets.md)]

---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

<span data-ttu-id="8a0e0-129">返さ`notificationUrl`れるのは、socket.io エンドポイントの URL です。</span><span class="sxs-lookup"><span data-stu-id="8a0e0-129">The `notificationUrl` returned is a socket.io endpoint URL.</span></span>
<span data-ttu-id="8a0e0-130">Socket.io クライアントでこれを使用するには、 `/callback?`トークンの文字列を分割します。</span><span class="sxs-lookup"><span data-stu-id="8a0e0-130">To use it with a socket.io client, split the string on the `/callback?` token.</span></span>
<span data-ttu-id="8a0e0-131">Before `/callback?`文字列の部分は socket.io エンドポイント URL で、after 文字列の部分は、ライブラリに指定する必要がある非透過のクエリ文字列です。</span><span class="sxs-lookup"><span data-stu-id="8a0e0-131">The part of the string before `/callback?` is the socket.io endpoint URL and the part of the string after is an opaque query string that must be given to the libary.</span></span>

<span data-ttu-id="8a0e0-132">次の例は、 `notificationUrl` JavaScript で with socket.io を使用する方法を示しています。</span><span class="sxs-lookup"><span data-stu-id="8a0e0-132">The following example shows how to use the `notificationUrl` with socket.io in JavaScript.</span></span>

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

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79 
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Example",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/driveItem-subscriptions-socketio.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/beta/api/driveItem-subscriptions-socketio.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}-->
