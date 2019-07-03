---
title: '通話: 応答'
description: 着信に応答します。
author: VinodRavichandran
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: 6220210b88974a7769acb95a8ca62d29b98a33ab
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/02/2019
ms.locfileid: "35438833"
---
# <a name="call-answer"></a><span data-ttu-id="0c311-103">通話: 応答</span><span class="sxs-lookup"><span data-stu-id="0c311-103">call: answer</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="0c311-104">着信に応答します。</span><span class="sxs-lookup"><span data-stu-id="0c311-104">Answer an incoming call.</span></span>

## <a name="permissions"></a><span data-ttu-id="0c311-105">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="0c311-105">Permissions</span></span>
<span data-ttu-id="0c311-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="0c311-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="0c311-108">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="0c311-108">Permission type</span></span> | <span data-ttu-id="0c311-109">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="0c311-109">Permissions (from least to most privileged)</span></span>                 |
| :-------------- | :-----------------------------------------------------------|
| <span data-ttu-id="0c311-110">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="0c311-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="0c311-111">サポート対象外</span><span class="sxs-lookup"><span data-stu-id="0c311-111">Not Supported</span></span>                        |
| <span data-ttu-id="0c311-112">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="0c311-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="0c311-113">サポート対象外</span><span class="sxs-lookup"><span data-stu-id="0c311-113">Not Supported</span></span>                        |
| <span data-ttu-id="0c311-114">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="0c311-114">Application</span></span>     | <span data-ttu-id="0c311-115">None</span><span class="sxs-lookup"><span data-stu-id="0c311-115">None</span></span>                                                        |

## <a name="http-request"></a><span data-ttu-id="0c311-116">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="0c311-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /app/calls/{id}/answer
POST /applications/{id}/calls/{id}/answer
```

## <a name="request-headers"></a><span data-ttu-id="0c311-117">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="0c311-117">Request headers</span></span>
| <span data-ttu-id="0c311-118">名前</span><span class="sxs-lookup"><span data-stu-id="0c311-118">Name</span></span>          | <span data-ttu-id="0c311-119">説明</span><span class="sxs-lookup"><span data-stu-id="0c311-119">Description</span></span>               |
|:--------------|:--------------------------|
| <span data-ttu-id="0c311-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="0c311-120">Authorization</span></span> | <span data-ttu-id="0c311-p102">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="0c311-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="0c311-123">要求本文</span><span class="sxs-lookup"><span data-stu-id="0c311-123">Request body</span></span>
<span data-ttu-id="0c311-124">要求本文で、次のパラメーターを含む JSON オブジェクトを指定します。</span><span class="sxs-lookup"><span data-stu-id="0c311-124">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="0c311-125">パラメーター</span><span class="sxs-lookup"><span data-stu-id="0c311-125">Parameter</span></span>        | <span data-ttu-id="0c311-126">型</span><span class="sxs-lookup"><span data-stu-id="0c311-126">Type</span></span>                                     |<span data-ttu-id="0c311-127">説明</span><span class="sxs-lookup"><span data-stu-id="0c311-127">Description</span></span>                                                                                                                                    |
|:-----------------|:-----------------------------------------|:----------------------------------------------------------------------------------------------------------------------------------------------|
|<span data-ttu-id="0c311-128">callbackUri</span><span class="sxs-lookup"><span data-stu-id="0c311-128">callbackUri</span></span>       |<span data-ttu-id="0c311-129">String</span><span class="sxs-lookup"><span data-stu-id="0c311-129">String</span></span>                                    |<span data-ttu-id="0c311-130">コールバック時のコールバック ID またはサブスクリプション ID。</span><span class="sxs-lookup"><span data-stu-id="0c311-130">The callback or subscription ID on which callbacks will be delivered.</span></span> <span data-ttu-id="0c311-131">要する</span><span class="sxs-lookup"><span data-stu-id="0c311-131">(Required)</span></span>                                                               |
|<span data-ttu-id="0c311-132">acceptedModalities</span><span class="sxs-lookup"><span data-stu-id="0c311-132">acceptedModalities</span></span>|<span data-ttu-id="0c311-133">文字列コレクション</span><span class="sxs-lookup"><span data-stu-id="0c311-133">String collection</span></span>                         |<span data-ttu-id="0c311-134">Accept モダリティのリスト。</span><span class="sxs-lookup"><span data-stu-id="0c311-134">The list of accept modalities.</span></span> <span data-ttu-id="0c311-135">使用可能な値`unknown`は`audio`、 `video`、 `screenSharing` `videoBasedScreenSharing`、、 `data`、、です。</span><span class="sxs-lookup"><span data-stu-id="0c311-135">Possible value are: `unknown`, `audio`, `video`, `screenSharing`, `videoBasedScreenSharing`, `data`.</span></span> <span data-ttu-id="0c311-136">要する</span><span class="sxs-lookup"><span data-stu-id="0c311-136">(Required)</span></span> |
|<span data-ttu-id="0c311-137">mediaConfig</span><span class="sxs-lookup"><span data-stu-id="0c311-137">mediaConfig</span></span>       |[<span data-ttu-id="0c311-138">mediaConfig</span><span class="sxs-lookup"><span data-stu-id="0c311-138">mediaConfig</span></span>](../resources/mediaconfig.md)|<span data-ttu-id="0c311-139">メディア構成。</span><span class="sxs-lookup"><span data-stu-id="0c311-139">The media configuration.</span></span> <span data-ttu-id="0c311-140">要する</span><span class="sxs-lookup"><span data-stu-id="0c311-140">(Required)</span></span>                                                                                                            |

## <a name="response"></a><span data-ttu-id="0c311-141">応答</span><span class="sxs-lookup"><span data-stu-id="0c311-141">Response</span></span>
<span data-ttu-id="0c311-142">このメソッドは`202 Accepted`応答コードを返します。</span><span class="sxs-lookup"><span data-stu-id="0c311-142">This method returns `202 Accepted` response code.</span></span>

## <a name="examples"></a><span data-ttu-id="0c311-143">例</span><span class="sxs-lookup"><span data-stu-id="0c311-143">Examples</span></span>
<span data-ttu-id="0c311-144">次の例は、この API を呼び出す方法を示しています。</span><span class="sxs-lookup"><span data-stu-id="0c311-144">The following example shows how to call this API.</span></span>

##### <a name="request"></a><span data-ttu-id="0c311-145">要求</span><span class="sxs-lookup"><span data-stu-id="0c311-145">Request</span></span>
<span data-ttu-id="0c311-146">次の例は要求を示しています。</span><span class="sxs-lookup"><span data-stu-id="0c311-146">The following example shows the request.</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="0c311-147">プロトコル</span><span class="sxs-lookup"><span data-stu-id="0c311-147">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "call-answer"
}-->
```http
POST https://graph.microsoft.com/beta/app/calls/{id}/answer
Content-Type: application/json
Content-Length: 211

{
  "callbackUri": "callbackUri-value",
  "mediaConfig": {
    "@odata.type": "#microsoft.graph.appHostedMediaConfig",
    "blob": "<media config blob>"
  },
  "acceptedModalities": [
    "audio"
  ]
}
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="0c311-148">C#</span><span class="sxs-lookup"><span data-stu-id="0c311-148">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/call-answer-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="0c311-149">Javascript</span><span class="sxs-lookup"><span data-stu-id="0c311-149">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/call-answer-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="0c311-150">目的-C</span><span class="sxs-lookup"><span data-stu-id="0c311-150">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/call-answer-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="0c311-151">応答</span><span class="sxs-lookup"><span data-stu-id="0c311-151">Response</span></span>
<span data-ttu-id="0c311-152">以下は、応答の例です。</span><span class="sxs-lookup"><span data-stu-id="0c311-152">Here is an example of the response.</span></span> 

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.None"
} -->
```http
HTTP/1.1 202 Accepted
```

### <a name="answer-voip-call-with-service-hosted-media"></a><span data-ttu-id="0c311-153">サービスホストされたメディアを使用した VOIP 通話への応答</span><span class="sxs-lookup"><span data-stu-id="0c311-153">Answer VOIP call with service hosted media</span></span>

##### <a name="notification---incoming"></a><span data-ttu-id="0c311-154">通知-受信</span><span class="sxs-lookup"><span data-stu-id="0c311-154">Notification - incoming</span></span>

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
        "callRoutes": [
          {
            "routingType": "lookup",
            "original": {
              "phone": {
                "id": "+14258828080"
              }
            },
            "final": {
              "user": {
                "id": "29362BD4-CD58-4ED0-A206-0E4A33DBB0B6",
                "displayName": "Heidi Steen"
              }
            }
          }
        ],
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
            "languageId": "en-US"
          }
        ],
        "requestedModalities": [ "audio" ]
      }
    }
  ]
}
```

##### <a name="request"></a><span data-ttu-id="0c311-155">要求</span><span class="sxs-lookup"><span data-stu-id="0c311-155">Request</span></span>

```http
POST /app/calls/57DAB8B1894C409AB240BD8BEAE78896/answer
Authorization: Bearer <TOKEN>
Content-Type: application/json
```

<!-- {
  "blockType": "ignored",
  "name": "call-answer"
}-->
```json
{
  "callbackUri": "https://bot.contoso.com/api/calls",
  "acceptedModalities": [ "audio" ],
  "mediaConfig": {
    "@odata.type": "#microsoft.graph.serviceHostedMediaConfig",
    "preFetchMedia": [
      {
        "uri": "https://cdn.contoso.com/beep.wav",
        "resourceId": "1D6DE2D4-CD51-4309-8DAA-70768651088E"
      },
      {
        "uri": "https://cdn.contoso.com/cool.wav",
        "resourceId": "1D6DE2D4-CD51-4309-8DAA-70768651088F"
      }
    ]
  }
}
```

##### <a name="response"></a><span data-ttu-id="0c311-156">応答</span><span class="sxs-lookup"><span data-stu-id="0c311-156">Response</span></span>

```http
HTTP/1.1 202 Accepted
```

##### <a name="notification---establishing"></a><span data-ttu-id="0c311-157">通知-確立中</span><span class="sxs-lookup"><span data-stu-id="0c311-157">Notification - establishing</span></span>

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
        "state": "establishing"
      }
    }
  ]
}
```

##### <a name="notification---established"></a><span data-ttu-id="0c311-158">通知-確立済み</span><span class="sxs-lookup"><span data-stu-id="0c311-158">Notification - established</span></span>

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
        "state": "established"
      }
    }
  ]
}
```

### <a name="answer-voip-call-with-application-hosted-media"></a><span data-ttu-id="0c311-159">アプリケーションでホストされているメディアを使用した VOIP 通話への応答</span><span class="sxs-lookup"><span data-stu-id="0c311-159">Answer VOIP call with application hosted media</span></span>

##### <a name="notification---incoming"></a><span data-ttu-id="0c311-160">通知-受信</span><span class="sxs-lookup"><span data-stu-id="0c311-160">Notification - incoming</span></span>

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
          "@odata.type": "#microsoft.graph.participantInfo",
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
            "@odata.type": "#microsoft.graph.participantInfo",
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
        "requestedModalities": [ "audio" ]
      }
    }
  ]
}
```

##### <a name="request"></a><span data-ttu-id="0c311-161">要求</span><span class="sxs-lookup"><span data-stu-id="0c311-161">Request</span></span>

```http
POST /app/calls/57DAB8B1894C409AB240BD8BEAE78896/answer
Authorization: Bearer <TOKEN>
Content-Type: application/json
```

<!-- {
  "blockType": "ignored",
  "name": "call-answer"
}-->
```json
{
  "callbackUri": "https://bot.contoso.com/api/calls",
  "acceptedModalities": [ "audio" ],
  "mediaConfig": {
    "@odata.type": "#microsoft.graph.appHostedMediaConfig",
    "blob": "<media config blob>"
  }
}
```

##### <a name="response"></a><span data-ttu-id="0c311-162">応答</span><span class="sxs-lookup"><span data-stu-id="0c311-162">Response</span></span>

```http
HTTP/1.1 202 Accepted
```

##### <a name="notification---establishing"></a><span data-ttu-id="0c311-163">通知-確立中</span><span class="sxs-lookup"><span data-stu-id="0c311-163">Notification - establishing</span></span>

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
        "state": "establishing"
      }
    }
  ]
}
```

##### <a name="notification---established"></a><span data-ttu-id="0c311-164">通知-確立済み</span><span class="sxs-lookup"><span data-stu-id="0c311-164">Notification - established</span></span>

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
        "state": "established"
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
  "description": "call: answer",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
