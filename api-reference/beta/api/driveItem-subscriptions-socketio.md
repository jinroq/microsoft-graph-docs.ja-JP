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
# <a name="get-websocket-endpoint"></a><span data-ttu-id="ebbcc-103">Websocket のエンドポイントを取得します。</span><span class="sxs-lookup"><span data-stu-id="ebbcc-103">Get websocket endpoint</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]
<span data-ttu-id="ebbcc-104">実稼働アプリケーションでこれらの API を使用することは、サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="ebbcc-104">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="ebbcc-105">[Socket.io][]を使用して[ドライブ][]の近くにあるリアルタイム変更通知を受信できます。</span><span class="sxs-lookup"><span data-stu-id="ebbcc-105">Allows you to receive near-real-time change notifications for a [drive][] using [socket.io][].</span></span>
<span data-ttu-id="ebbcc-106">Socket.io は、Websocket を使用している javascript のコードの一般的な通知ライブラリです。</span><span class="sxs-lookup"><span data-stu-id="ebbcc-106">Socket.io is a popular notifications library for JavaScript that utilizes WebSockets.</span></span> <span data-ttu-id="ebbcc-107">詳細については、 [socket.io](https://socket.io)を参照してください。</span><span class="sxs-lookup"><span data-stu-id="ebbcc-107">To learn more, see [socket.io](https://socket.io).</span></span>

[drive]: ../resources/drive.md
[socket.io]: https://socket.io/

## <a name="permissions"></a><span data-ttu-id="ebbcc-110">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="ebbcc-110">Permissions</span></span>

<span data-ttu-id="ebbcc-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="ebbcc-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="ebbcc-113">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="ebbcc-113">Permission type</span></span>                        | <span data-ttu-id="ebbcc-114">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="ebbcc-114">Permissions (from least to most privileged)</span></span>
|:---------------------------------------|:-------------------------------------------
| <span data-ttu-id="ebbcc-115">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="ebbcc-115">Delegated (work or school account)</span></span>     | <span data-ttu-id="ebbcc-116">Files.Read、Files.ReadWrite、Files.ReadWrite.All、Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ebbcc-116">Files.Read, Files.ReadWrite, Files.ReadWrite.All, Sites.ReadWrite.All</span></span>
| <span data-ttu-id="ebbcc-117">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="ebbcc-117">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="ebbcc-118">Files.Read、Files.ReadWrite、Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ebbcc-118">Files.Read, Files.ReadWrite, Files.ReadWrite.All</span></span>
| <span data-ttu-id="ebbcc-119">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="ebbcc-119">Application</span></span>                            | <span data-ttu-id="ebbcc-120">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="ebbcc-120">Not supported.</span></span>

## <a name="http-request"></a><span data-ttu-id="ebbcc-121">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="ebbcc-121">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /me/drive/root/subscriptions/socketIo
GET /drives/{driveId}/root/subscriptions/socketIo
GET /groups/{groupId}/drive/root/subscriptions/socketIo
GET /sites/{siteId}/lists/{listId}/drive/root/subscriptions/socketIo
```

## <a name="example"></a><span data-ttu-id="ebbcc-122">例</span><span class="sxs-lookup"><span data-stu-id="ebbcc-122">Example</span></span>

### <a name="request"></a><span data-ttu-id="ebbcc-123">要求</span><span class="sxs-lookup"><span data-stu-id="ebbcc-123">Request</span></span>

<!-- { "blockType": "request", "name": "drive_root_subscriptions_socketIo" } -->
```http
GET /me/drive/root/subscriptions/socketIo
```

### <a name="response"></a><span data-ttu-id="ebbcc-124">応答</span><span class="sxs-lookup"><span data-stu-id="ebbcc-124">Response</span></span>

<span data-ttu-id="ebbcc-125">かどうかは成功すると、このメソッドが返されます、`200 OK`応答コードおよび応答の本文の[サブスクリプション](../resources/subscription.md)オブジェクトです。</span><span class="sxs-lookup"><span data-stu-id="ebbcc-125">If successful, this method returns a `200 OK` response code and a [subscription](../resources/subscription.md) object in the response body.</span></span>

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

<span data-ttu-id="ebbcc-126">`notificationUrl`は、socket.io のエンドポイントの URL が返されます。</span><span class="sxs-lookup"><span data-stu-id="ebbcc-126">The `notificationUrl` returned is a socket.io endpoint URL.</span></span>
<span data-ttu-id="ebbcc-127">Socket.io クライアントを使用してこれを使用するに、文字列を分割する、`/callback?`トークンです。</span><span class="sxs-lookup"><span data-stu-id="ebbcc-127">To use it with a socket.io client, split the string on the `/callback?` token.</span></span>
<span data-ttu-id="ebbcc-128">前に文字列の中で`/callback?`socket.io のエンドポイントの URL は、後の文字列の中でライブラリを指定する必要がありますが、不透明なクエリ文字列です。</span><span class="sxs-lookup"><span data-stu-id="ebbcc-128">The part of the string before `/callback?` is the socket.io endpoint URL and the part of the string after is an opaque query string that must be given to the libary.</span></span>

<span data-ttu-id="ebbcc-129">使用する方法の例を次の`notificationUrl`JavaScript で socket.io をします。</span><span class="sxs-lookup"><span data-stu-id="ebbcc-129">The following example shows how to use the `notificationUrl` with socket.io in JavaScript.</span></span>

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
