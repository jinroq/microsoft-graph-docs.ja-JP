---
title: 'call: redirect'
description: 着信をリダイレクトします。
author: VinodRavichandran
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: a43f9c6164e69315d60f39c2ae0b9c1ba3df2c9f
ms.sourcegitcommit: 1066aa4045d48f9c9b764d3b2891cf4f806d17d5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/15/2019
ms.locfileid: "36418895"
---
# <a name="call-redirect"></a><span data-ttu-id="2fd99-103">call: redirect</span><span class="sxs-lookup"><span data-stu-id="2fd99-103">call: redirect</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="2fd99-104">着信をリダイレクトします。</span><span class="sxs-lookup"><span data-stu-id="2fd99-104">Redirect an incoming call.</span></span>

## <a name="permissions"></a><span data-ttu-id="2fd99-105">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="2fd99-105">Permissions</span></span>
<span data-ttu-id="2fd99-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="2fd99-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="2fd99-108">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="2fd99-108">Permission type</span></span> | <span data-ttu-id="2fd99-109">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="2fd99-109">Permissions (from least to most privileged)</span></span>         |
| :-------------- | :-------------------------------------------------- |
| <span data-ttu-id="2fd99-110">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="2fd99-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="2fd99-111">サポート対象外</span><span class="sxs-lookup"><span data-stu-id="2fd99-111">Not Supported</span></span>                |
| <span data-ttu-id="2fd99-112">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="2fd99-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="2fd99-113">サポート対象外</span><span class="sxs-lookup"><span data-stu-id="2fd99-113">Not Supported</span></span>                |
| <span data-ttu-id="2fd99-114">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="2fd99-114">Application</span></span>     | <span data-ttu-id="2fd99-115">Calls.Initiate.All</span><span class="sxs-lookup"><span data-stu-id="2fd99-115">Calls.Initiate.All</span></span>                                  |

## <a name="http-request"></a><span data-ttu-id="2fd99-116">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="2fd99-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /app/calls/{id}/redirect
POST /applications/{id}/calls/{id}/redirect
```

## <a name="request-headers"></a><span data-ttu-id="2fd99-117">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="2fd99-117">Request headers</span></span>
| <span data-ttu-id="2fd99-118">名前</span><span class="sxs-lookup"><span data-stu-id="2fd99-118">Name</span></span>          | <span data-ttu-id="2fd99-119">説明</span><span class="sxs-lookup"><span data-stu-id="2fd99-119">Description</span></span>               |
|:--------------|:--------------------------|
| <span data-ttu-id="2fd99-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="2fd99-120">Authorization</span></span> | <span data-ttu-id="2fd99-p102">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="2fd99-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="2fd99-123">要求本文</span><span class="sxs-lookup"><span data-stu-id="2fd99-123">Request body</span></span>
<span data-ttu-id="2fd99-124">要求本文で、次のパラメーターを含む JSON オブジェクトを指定します。</span><span class="sxs-lookup"><span data-stu-id="2fd99-124">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="2fd99-125">パラメーター</span><span class="sxs-lookup"><span data-stu-id="2fd99-125">Parameter</span></span>      | <span data-ttu-id="2fd99-126">型</span><span class="sxs-lookup"><span data-stu-id="2fd99-126">Type</span></span>    |<span data-ttu-id="2fd99-127">説明</span><span class="sxs-lookup"><span data-stu-id="2fd99-127">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="2fd99-128">Targets</span><span class="sxs-lookup"><span data-stu-id="2fd99-128">targets</span></span>|<span data-ttu-id="2fd99-129">[invitationParticipantInfo](../resources/invitationparticipantinfo.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="2fd99-129">[invitationParticipantInfo](../resources/invitationparticipantinfo.md) collection</span></span>|<span data-ttu-id="2fd99-130">リダイレクト操作の対象となる参加者。</span><span class="sxs-lookup"><span data-stu-id="2fd99-130">The target participants of the redirect operation.</span></span>|
|<span data-ttu-id="2fd99-131">targetDisposition ポジション</span><span class="sxs-lookup"><span data-stu-id="2fd99-131">targetDisposition</span></span>|<span data-ttu-id="2fd99-132">String</span><span class="sxs-lookup"><span data-stu-id="2fd99-132">String</span></span>|<span data-ttu-id="2fd99-133">指定できる値は次のとおりです。`default`</span><span class="sxs-lookup"><span data-stu-id="2fd99-133">The possible value is: `default`</span></span>|
|<span data-ttu-id="2fd99-134">timeout</span><span class="sxs-lookup"><span data-stu-id="2fd99-134">timeout</span></span>|<span data-ttu-id="2fd99-135">Int32</span><span class="sxs-lookup"><span data-stu-id="2fd99-135">Int32</span></span>|<span data-ttu-id="2fd99-136">リダイレクト操作のタイムアウト (秒単位)。</span><span class="sxs-lookup"><span data-stu-id="2fd99-136">The timeout in seconds for the redirect operation.</span></span>|
|<span data-ttu-id="2fd99-137">maskCallee 先</span><span class="sxs-lookup"><span data-stu-id="2fd99-137">maskCallee</span></span>|<span data-ttu-id="2fd99-138">Boolean</span><span class="sxs-lookup"><span data-stu-id="2fd99-138">Boolean</span></span>|<span data-ttu-id="2fd99-139">呼び出し先をマスクするかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="2fd99-139">Indicates whether to mask the callee.</span></span>|
|<span data-ttu-id="2fd99-140">maskCaller</span><span class="sxs-lookup"><span data-stu-id="2fd99-140">maskCaller</span></span>|<span data-ttu-id="2fd99-141">Boolean</span><span class="sxs-lookup"><span data-stu-id="2fd99-141">Boolean</span></span>|<span data-ttu-id="2fd99-142">発信者をマスクするかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="2fd99-142">Indicates whether to mask the caller.</span></span>|

## <a name="response"></a><span data-ttu-id="2fd99-143">応答</span><span class="sxs-lookup"><span data-stu-id="2fd99-143">Response</span></span>
<span data-ttu-id="2fd99-144">応答`202 Accepted`コードを返します。</span><span class="sxs-lookup"><span data-stu-id="2fd99-144">Returns `202 Accepted` response code</span></span>

## <a name="examples"></a><span data-ttu-id="2fd99-145">例</span><span class="sxs-lookup"><span data-stu-id="2fd99-145">Examples</span></span>

### <a name="redirect-a-call"></a><span data-ttu-id="2fd99-146">通話をリダイレクトする</span><span class="sxs-lookup"><span data-stu-id="2fd99-146">Redirect a call</span></span>

##### <a name="request"></a><span data-ttu-id="2fd99-147">要求</span><span class="sxs-lookup"><span data-stu-id="2fd99-147">Request</span></span>
<span data-ttu-id="2fd99-148">次の例は要求を示しています。</span><span class="sxs-lookup"><span data-stu-id="2fd99-148">The following example shows the request.</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="2fd99-149">プロトコル</span><span class="sxs-lookup"><span data-stu-id="2fd99-149">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "call-redirect"
}-->
```http
POST https://graph.microsoft.com/beta/app/calls/{id}/redirect
Content-Type: application/json
Content-Length: 515

{
  "targets": [
    {
      "endpointType": "default",
      "identity": {
        "user": {
          "id": "550fae72-d251-43ec-868c-373732c2704f",
          "tenantId": "72f988bf-86f1-41af-91ab-2d7cd011db47",
          "displayName": "Heidi Steen"
        }
      },
      "languageId": "en-US",
      "region": "westus"
    }
  ],
  "targetDisposition": "default",
  "timeout": 99,
  "maskCallee": false,
  "maskCaller": false
}
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="2fd99-150">C#</span><span class="sxs-lookup"><span data-stu-id="2fd99-150">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/call-redirect-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="2fd99-151">JavaScript</span><span class="sxs-lookup"><span data-stu-id="2fd99-151">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/call-redirect-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="2fd99-152">目的-C</span><span class="sxs-lookup"><span data-stu-id="2fd99-152">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/call-redirect-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="2fd99-153">応答</span><span class="sxs-lookup"><span data-stu-id="2fd99-153">Response</span></span>

> <span data-ttu-id="2fd99-p103">**注:** 読みやすくするために、ここに示す応答オブジェクトは短縮されている場合があります。実際の呼び出しからは、すべてのプロパティが返されます。</span><span class="sxs-lookup"><span data-stu-id="2fd99-p103">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.None"
} -->
```http
HTTP/1.1 202 Accepted
```

### <a name="forward-a-call"></a><span data-ttu-id="2fd99-156">通話を転送する</span><span class="sxs-lookup"><span data-stu-id="2fd99-156">Forward a call</span></span>

##### <a name="notification---incoming"></a><span data-ttu-id="2fd99-157">通知-受信</span><span class="sxs-lookup"><span data-stu-id="2fd99-157">Notification - incoming</span></span>

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
      "changeType": "created",
      "resource": "/app/calls/57DAB8B1894C409AB240BD8BEAE78896",
      "resourceData": {
        "@odata.type": "#microsoft.graph.call",
        "@odata.id": "/app/calls/57DAB8B1894C409AB240BD8BEAE78896",
        "@odata.etag": "W/\"5445\"",
        "state": "incoming",
        "direction": "incoming",
        "source": {
          "identity": {
            "user": {
              "displayName": "Test User",
              "id": "8A34A46B-3D17-4ADC-8DCE-DC4E7D572698"
            }
          },
          "region": "westus",
          "languageId": "en-US"
        },
        "targets": [
          {
            "identity": {
              "application": {
                "displayName": "Test BOT",
                "id": "8A34A46B-3D17-4ADC-8DCE-DC4E7D572698"
              }
            },
            "region": "westus",
            "languageId": "en-US"
          }
        ],
        "requestedModalities": [ "audio", "video" ]
      }
    }
  ]
}
```

##### <a name="request"></a><span data-ttu-id="2fd99-158">要求</span><span class="sxs-lookup"><span data-stu-id="2fd99-158">Request</span></span>

```http
POST https://graph.microsoft.com/beta/app/calls/57DAB8B1894C409AB240BD8BEAE78896/redirect
Authorization: Bearer <TOKEN>
Content-Type: application/json

{
  "targets": [
    {
      "endpointType": "default",
      "identity": {
        "user": {
          "id": "8A34A46B-3D17-4ADC-8DCE-DC4E7D572699"
        }
      },
      "languageId": "en-US",
      "region": "westus"
    }
  ],
  "targetDisposition": "default",
  "timeout": 60,
  "maskCallee": false,
  "maskCaller": false
}
```

##### <a name="response"></a><span data-ttu-id="2fd99-159">応答</span><span class="sxs-lookup"><span data-stu-id="2fd99-159">Response</span></span>

```http
HTTP/1.1 202 Accepted
```

##### <a name="notification---redirecting"></a><span data-ttu-id="2fd99-160">通知-リダイレクト</span><span class="sxs-lookup"><span data-stu-id="2fd99-160">Notification - redirecting</span></span>

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
      "resource": "/app/calls/57DAB8B1894C409AB240BD8BEAE78896",
      "resourceData": {
        "@odata.type": "#microsoft.graph.call",
        "@odata.id": "/app/calls/57DAB8B1894C409AB240BD8BEAE78896",
        "@odata.etag": "W/\"5445\"",
        "state": "redirecting"
      }
    }
  ]
}
```

##### <a name="notification---terminated"></a><span data-ttu-id="2fd99-161">通知の終了</span><span class="sxs-lookup"><span data-stu-id="2fd99-161">Notification - terminated</span></span>

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
      "changeType": "deleted",
      "resource": "/app/calls/57DAB8B1894C409AB240BD8BEAE78896",
      "resourceData": {
        "@odata.type": "#microsoft.graph.call",
        "@odata.id": "/app/calls/57DAB8B1894C409AB240BD8BEAE78896",
        "@odata.etag": "W/\"5445\"",
        "state": "terminated",
        "answeredBy": {
          "identity": {
            "user": {
              "displayName": "Test User 2",
              "id": "8A34A46B-3D17-4ADC-8DCE-DC4E7D572699"
            }
          }
        },
        "terminationReason": "AppRedirected"
      }
    }
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "call: redirect",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
