---
title: '参加者: ミュート'
description: 通話で特定の参加者をミュートします。
author: VinodRavichandran
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: c8c78d23dd0fc80f3990160ad74e5c98fb09dc0e
ms.sourcegitcommit: 1066aa4045d48f9c9b764d3b2891cf4f806d17d5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/15/2019
ms.locfileid: "36413777"
---
# <a name="participant-mute"></a><span data-ttu-id="b84d9-103">参加者: ミュート</span><span class="sxs-lookup"><span data-stu-id="b84d9-103">participant: mute</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="b84d9-104">通話で特定の参加者をミュートします。</span><span class="sxs-lookup"><span data-stu-id="b84d9-104">Mute a specific participant in the call.</span></span>

## <a name="permissions"></a><span data-ttu-id="b84d9-105">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="b84d9-105">Permissions</span></span>
<span data-ttu-id="b84d9-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="b84d9-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="b84d9-108">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="b84d9-108">Permission type</span></span> | <span data-ttu-id="b84d9-109">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="b84d9-109">Permissions (from least to most privileged)</span></span> |
| :-------------- | :------------------------------------------ |
| <span data-ttu-id="b84d9-110">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="b84d9-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="b84d9-111">サポート対象外</span><span class="sxs-lookup"><span data-stu-id="b84d9-111">Not Supported</span></span>        |
| <span data-ttu-id="b84d9-112">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="b84d9-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="b84d9-113">サポート対象外</span><span class="sxs-lookup"><span data-stu-id="b84d9-113">Not Supported</span></span>        |
| <span data-ttu-id="b84d9-114">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="b84d9-114">Application</span></span>     | <span data-ttu-id="b84d9-115">None</span><span class="sxs-lookup"><span data-stu-id="b84d9-115">None</span></span>                                        |

## <a name="http-request"></a><span data-ttu-id="b84d9-116">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="b84d9-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /app/calls/{id}/participants/{id}/mute
POST /applications/{id}/calls/{id}/participants/{id}/mute
```

## <a name="request-headers"></a><span data-ttu-id="b84d9-117">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="b84d9-117">Request headers</span></span>
| <span data-ttu-id="b84d9-118">名前</span><span class="sxs-lookup"><span data-stu-id="b84d9-118">Name</span></span>          | <span data-ttu-id="b84d9-119">説明</span><span class="sxs-lookup"><span data-stu-id="b84d9-119">Description</span></span>               |
|:--------------|:--------------------------|
| <span data-ttu-id="b84d9-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="b84d9-120">Authorization</span></span> | <span data-ttu-id="b84d9-p102">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="b84d9-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="b84d9-123">要求本文</span><span class="sxs-lookup"><span data-stu-id="b84d9-123">Request body</span></span>
<span data-ttu-id="b84d9-124">要求本文で、次のパラメーターを含む JSON オブジェクトを指定します。</span><span class="sxs-lookup"><span data-stu-id="b84d9-124">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="b84d9-125">パラメーター</span><span class="sxs-lookup"><span data-stu-id="b84d9-125">Parameter</span></span>      | <span data-ttu-id="b84d9-126">型</span><span class="sxs-lookup"><span data-stu-id="b84d9-126">Type</span></span>    |<span data-ttu-id="b84d9-127">説明</span><span class="sxs-lookup"><span data-stu-id="b84d9-127">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="b84d9-128">clientContext</span><span class="sxs-lookup"><span data-stu-id="b84d9-128">clientContext</span></span>|<span data-ttu-id="b84d9-129">String</span><span class="sxs-lookup"><span data-stu-id="b84d9-129">String</span></span>|<span data-ttu-id="b84d9-130">クライアントコンテキスト。</span><span class="sxs-lookup"><span data-stu-id="b84d9-130">The client context.</span></span>|

## <a name="response"></a><span data-ttu-id="b84d9-131">応答</span><span class="sxs-lookup"><span data-stu-id="b84d9-131">Response</span></span>
<span data-ttu-id="b84d9-132">成功した場合、この`200 OK`メソッドは応答コードと、応答本文で[commsOperation](../resources/commsoperation.md)オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="b84d9-132">If successful, this method returns `200 OK` response code and [commsOperation](../resources/commsoperation.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="b84d9-133">例</span><span class="sxs-lookup"><span data-stu-id="b84d9-133">Example</span></span>
<span data-ttu-id="b84d9-134">次の例は、この API を呼び出す方法を示しています。</span><span class="sxs-lookup"><span data-stu-id="b84d9-134">The following example shows how to call this API.</span></span>

##### <a name="request"></a><span data-ttu-id="b84d9-135">要求</span><span class="sxs-lookup"><span data-stu-id="b84d9-135">Request</span></span>
<span data-ttu-id="b84d9-136">次の例は要求を示しています。</span><span class="sxs-lookup"><span data-stu-id="b84d9-136">The following example shows the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="b84d9-137">プロトコル</span><span class="sxs-lookup"><span data-stu-id="b84d9-137">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "participant-mute"
}-->
```http
POST https://graph.microsoft.com/beta/app/calls/{id}/participants/{id}/mute
Content-Type: application/json
Content-Length: 46

{
  "clientContext": "clientContext-value"
}
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="b84d9-138">C#</span><span class="sxs-lookup"><span data-stu-id="b84d9-138">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/participant-mute-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="b84d9-139">JavaScript</span><span class="sxs-lookup"><span data-stu-id="b84d9-139">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/participant-mute-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="b84d9-140">目的-C</span><span class="sxs-lookup"><span data-stu-id="b84d9-140">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/participant-mute-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="b84d9-141">応答</span><span class="sxs-lookup"><span data-stu-id="b84d9-141">Response</span></span>

> <span data-ttu-id="b84d9-p103">**注:** 読みやすくするために、ここに示す応答オブジェクトは短縮されている場合があります。実際の呼び出しからは、すべてのプロパティが返されます。</span><span class="sxs-lookup"><span data-stu-id="b84d9-p103">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "@odata.type": "microsoft.graph.commsOperation",
  "truncated": true
} -->
```http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 259

{
  "id": "17e3b46c-f61d-4f4d-9635-c626ef18e6ad",
  "status": "completed",
  "createdDateTime": "2018-09-06T15:58:41Z",
  "lastActionDateTime": "2018-09-06T15:58:41Z",
  "clientContext": "d45324c1-fcb5-430a-902c-f20af696537c"
}
```

## <a name="example---mute-specific-participant"></a><span data-ttu-id="b84d9-144">例-特定の参加者のミュート</span><span class="sxs-lookup"><span data-stu-id="b84d9-144">Example - Mute specific participant</span></span>

##### <a name="request"></a><span data-ttu-id="b84d9-145">要求</span><span class="sxs-lookup"><span data-stu-id="b84d9-145">Request</span></span>

```http
POST /app/calls/57DAB8B1894C409AB240BD8BEAE78896/participants/0698446E77E24E4D85F80597083CB830/mute
Authorization: Bearer <TOKEN>
Content-Type: application/json

{
  "clientContext": "d45324c1-fcb5-430a-902c-f20af696537c"
}
```

##### <a name="response"></a><span data-ttu-id="b84d9-146">応答</span><span class="sxs-lookup"><span data-stu-id="b84d9-146">Response</span></span>

```http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 259
```

<!-- {
  "blockType": "example",
  "@odata.type": "microsoft.graph.commsOperation",
  "truncated": true
}-->
```json
{
  "id": "17e3b46c-f61d-4f4d-9635-c626ef18e6ad",
  "status": "completed",
  "createdDateTime": "2018-09-06T15:58:41Z",
  "lastActionDateTime": "2018-09-06T15:58:41Z",
  "clientContext": "d45324c1-fcb5-430a-902c-f20af696537c"
}
```

##### <a name="notification---roster-updated-with-participant-muted"></a><span data-ttu-id="b84d9-147">通知-参加者がミュート状態で更新された名簿</span><span class="sxs-lookup"><span data-stu-id="b84d9-147">Notification - roster updated with participant muted</span></span>

```http
POST https://bot.contoso.com/api/calls
Authorization: Bearer <TOKEN>
Content-Type: application/json
```

<!-- {
  "blockType": "example",
  "@odata.type": "microsoft.graph.commsNotifications"
}-->
```json
{
  "value": [
    {
      "changeType": "updated",
      "resource": "/app/calls/57DAB8B1894C409AB240BD8BEAE78896/participants",
      "resourceData": [
        {
          "@odata.type": "#microsoft.graph.participant",
          "id": "0698446E77E24E4D85F80597083CB830",
          "info": {
            "identity": {
              "user": {
                "displayName": "Test User",
                "id": "8A34A46B-3D17-4ADC-8DCE-DC4E7D572698"
              }
            },
            "region": "westus",
            "languageId": "en-US"
          },
          "mediaStreams": [
            {
              "mediaType": "audio",
              "label": "main-audio",
              "sourceId": "1",
              "direction": "sendReceive",
              "serverMuted": false
            }
          ],
          "isMuted": true,
          "isInLobby": false
        },
        {
          "@odata.type": "#microsoft.graph.participant",
          "id": "123456W77E24E4D85F80597083CB830",
          "info": {
            "identity": {
              "application": {
                "displayName": "Test Bot",
                "id": "1234A46B-3D17-4ADC-8DCE-DC4E7D556789"
              }
            },
            "region": "westus",
            "languageId": "en-US"
          },
          "mediaStreams": [
            {
              "mediaType": "audio",
              "label": "main-audio",
              "sourceId": "2",
              "direction": "sendReceive",
              "serverMuted": false
            }
          ],
          "isInLobby": false
        }
      ]
    }
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "participant: mute",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
