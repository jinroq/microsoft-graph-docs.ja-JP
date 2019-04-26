---
author: daspek
ms.author: dspektor
title: websocket エンドポイントを取得する
localization_priority: Normal
ms.prod: sharepoint
ms.openlocfilehash: 2172015e446b57706caeecf73b8da2b6b486f7d3
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/26/2019
ms.locfileid: "33345835"
---
# <a name="get-websocket-endpoint"></a><span data-ttu-id="84eb9-102">websocket エンドポイントを取得する</span><span class="sxs-lookup"><span data-stu-id="84eb9-102">Get websocket endpoint</span></span>

<span data-ttu-id="84eb9-103">[socket.io][]を使用して、[ドライブ][]のほぼリアルタイムの変更通知を受け取ることができます。</span><span class="sxs-lookup"><span data-stu-id="84eb9-103">Allows you to receive near-real-time change notifications for a [drive][] using [socket.io][].</span></span>
<span data-ttu-id="84eb9-104">Socket.io は、websocket を利用する JavaScript の一般的な通知ライブラリです。</span><span class="sxs-lookup"><span data-stu-id="84eb9-104">Socket.io is a popular notifications library for JavaScript that utilizes WebSockets.</span></span> <span data-ttu-id="84eb9-105">詳細については、「 [socket.io](https://socket.io)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="84eb9-105">To learn more, see [socket.io](https://socket.io).</span></span>

[ドライブ]: ../resources/drive.md
[drive]: ../resources/drive.md
[socket.io]: https://socket.io/

## <a name="permissions"></a><span data-ttu-id="84eb9-108">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="84eb9-108">Permissions</span></span>

<span data-ttu-id="84eb9-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="84eb9-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="84eb9-111">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="84eb9-111">Permission type</span></span>                        | <span data-ttu-id="84eb9-112">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="84eb9-112">Permissions (from least to most privileged)</span></span>
|:---------------------------------------|:-------------------------------------------
| <span data-ttu-id="84eb9-113">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="84eb9-113">Delegated (work or school account)</span></span>     | <span data-ttu-id="84eb9-114">ファイル。読み取り、ファイルの読み取り/書き込み。すべてのファイル。</span><span class="sxs-lookup"><span data-stu-id="84eb9-114">Files.Read, Files.ReadWrite, Files.ReadWrite.All, Sites.ReadWrite.All</span></span>
| <span data-ttu-id="84eb9-115">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="84eb9-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="84eb9-116">ファイル。読み取り、ファイルの読み取り/書き込み。</span><span class="sxs-lookup"><span data-stu-id="84eb9-116">Files.Read, Files.ReadWrite, Files.ReadWrite.All</span></span>
| <span data-ttu-id="84eb9-117">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="84eb9-117">Application</span></span>                            | <span data-ttu-id="84eb9-118">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="84eb9-118">Not supported.</span></span>

## <a name="http-request"></a><span data-ttu-id="84eb9-119">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="84eb9-119">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /me/drive/root/subscriptions/socketIo
GET /drives/{driveId}/root/subscriptions/socketIo
GET /groups/{groupId}/drive/root/subscriptions/socketIo
GET /sites/{siteId}/lists/{listId}/drive/root/subscriptions/socketIo
```

## <a name="example"></a><span data-ttu-id="84eb9-120">例</span><span class="sxs-lookup"><span data-stu-id="84eb9-120">Example</span></span>

### <a name="request"></a><span data-ttu-id="84eb9-121">要求</span><span class="sxs-lookup"><span data-stu-id="84eb9-121">Request</span></span>

<!-- { "blockType": "request", "name": "drive_root_subscriptions_socketIo" } -->
```http
GET /me/drive/root/subscriptions/socketIo
```

### <a name="response"></a><span data-ttu-id="84eb9-122">応答</span><span class="sxs-lookup"><span data-stu-id="84eb9-122">Response</span></span>

<span data-ttu-id="84eb9-123">成功した場合、このメソッド`200 OK`は応答コードと、応答本文で[subscription](../resources/subscription.md)オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="84eb9-123">If successful, this method returns a `200 OK` response code and a [subscription](../resources/subscription.md) object in the response body.</span></span>

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

<span data-ttu-id="84eb9-124">返さ`notificationUrl`れるのは、socket.io エンドポイントの URL です。</span><span class="sxs-lookup"><span data-stu-id="84eb9-124">The `notificationUrl` returned is a socket.io endpoint URL.</span></span>
<span data-ttu-id="84eb9-125">socket.io クライアントでこれを使用するには、 `/callback?`トークンの文字列を分割します。</span><span class="sxs-lookup"><span data-stu-id="84eb9-125">To use it with a socket.io client, split the string on the `/callback?` token.</span></span>
<span data-ttu-id="84eb9-126">before `/callback?`文字列の部分は socket.io エンドポイント URL で、after 文字列の部分は、ライブラリに指定する必要がある非透過のクエリ文字列です。</span><span class="sxs-lookup"><span data-stu-id="84eb9-126">The part of the string before `/callback?` is the socket.io endpoint URL and the part of the string after is an opaque query string that must be given to the libary.</span></span>

<span data-ttu-id="84eb9-127">次の例は、 `notificationUrl` JavaScript で with socket.io を使用する方法を示しています。</span><span class="sxs-lookup"><span data-stu-id="84eb9-127">The following example shows how to use the `notificationUrl` with socket.io in JavaScript.</span></span>

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

