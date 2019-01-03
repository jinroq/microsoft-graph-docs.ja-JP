---
title: '呼び出す: 回答'
description: 着信呼び出しに応答します。
author: VinodRavichandran
ms.openlocfilehash: c7de038e2323ab844590c884e15a639a3839dd86
ms.sourcegitcommit: 0b3a57ac8b99871e56389f9be15e4f96e219f635
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 12/20/2018
ms.locfileid: "27380514"
---
# <a name="call-answer"></a><span data-ttu-id="5a4de-103">呼び出す: 回答</span><span class="sxs-lookup"><span data-stu-id="5a4de-103">call: answer</span></span>

> <span data-ttu-id="5a4de-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="5a4de-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="5a4de-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="5a4de-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="5a4de-106">着信呼び出しに応答します。</span><span class="sxs-lookup"><span data-stu-id="5a4de-106">Answer an incoming call.</span></span>

## <a name="permissions"></a><span data-ttu-id="5a4de-107">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="5a4de-107">Permissions</span></span>
<span data-ttu-id="5a4de-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="5a4de-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="5a4de-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="5a4de-110">Permission type</span></span> | <span data-ttu-id="5a4de-111">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="5a4de-111">Permissions (from least to most privileged)</span></span>                 |
| :-------------- | :-----------------------------------------------------------|
| <span data-ttu-id="5a4de-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="5a4de-112">Delegated (work or school account)</span></span>     | <span data-ttu-id="5a4de-113">サポート対象外</span><span class="sxs-lookup"><span data-stu-id="5a4de-113">Not Supported</span></span>                        |
| <span data-ttu-id="5a4de-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="5a4de-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="5a4de-115">サポート対象外</span><span class="sxs-lookup"><span data-stu-id="5a4de-115">Not Supported</span></span>                        |
| <span data-ttu-id="5a4de-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="5a4de-116">Application</span></span>     | <span data-ttu-id="5a4de-117">なし</span><span class="sxs-lookup"><span data-stu-id="5a4de-117">None</span></span>                                                        |

## <a name="http-request"></a><span data-ttu-id="5a4de-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="5a4de-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /app/calls/{id}/answer
POST /applications/{id}/calls/{id}/answer
```

## <a name="request-headers"></a><span data-ttu-id="5a4de-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="5a4de-119">Request headers</span></span>
| <span data-ttu-id="5a4de-120">名前</span><span class="sxs-lookup"><span data-stu-id="5a4de-120">Name</span></span>          | <span data-ttu-id="5a4de-121">説明</span><span class="sxs-lookup"><span data-stu-id="5a4de-121">Description</span></span>               |
|:--------------|:--------------------------|
| <span data-ttu-id="5a4de-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="5a4de-122">Authorization</span></span> | <span data-ttu-id="5a4de-p103">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="5a4de-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="5a4de-125">要求本文</span><span class="sxs-lookup"><span data-stu-id="5a4de-125">Request body</span></span>
<span data-ttu-id="5a4de-126">要求本文で、次のパラメーターを含む JSON オブジェクトを指定します。</span><span class="sxs-lookup"><span data-stu-id="5a4de-126">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="5a4de-127">パラメーター</span><span class="sxs-lookup"><span data-stu-id="5a4de-127">Parameter</span></span>        | <span data-ttu-id="5a4de-128">型</span><span class="sxs-lookup"><span data-stu-id="5a4de-128">Type</span></span>                                     |<span data-ttu-id="5a4de-129">説明</span><span class="sxs-lookup"><span data-stu-id="5a4de-129">Description</span></span>                                                                                                                                    |
|:-----------------|:-----------------------------------------|:----------------------------------------------------------------------------------------------------------------------------------------------|
|<span data-ttu-id="5a4de-130">callbackUri</span><span class="sxs-lookup"><span data-stu-id="5a4de-130">callbackUri</span></span>       |<span data-ttu-id="5a4de-131">String</span><span class="sxs-lookup"><span data-stu-id="5a4de-131">String</span></span>                                    |<span data-ttu-id="5a4de-132">コールバックまたはサブスクリプションの ID をコールバックが配信されます。</span><span class="sxs-lookup"><span data-stu-id="5a4de-132">The callback or subscription ID on which callbacks will be delivered.</span></span> <span data-ttu-id="5a4de-133">(必須)</span><span class="sxs-lookup"><span data-stu-id="5a4de-133">(Required)</span></span>                                                               |
|<span data-ttu-id="5a4de-134">acceptedModalities</span><span class="sxs-lookup"><span data-stu-id="5a4de-134">acceptedModalities</span></span>|<span data-ttu-id="5a4de-135">String コレクション</span><span class="sxs-lookup"><span data-stu-id="5a4de-135">String collection</span></span>                         |<span data-ttu-id="5a4de-136">一覧には、様相がそのまま使用します。</span><span class="sxs-lookup"><span data-stu-id="5a4de-136">The list of accept modalities.</span></span> <span data-ttu-id="5a4de-137">使用可能な値: `unknown`、 `audio`、 `video`、 `screenSharing`、 `videoBasedScreenSharing`、 `data`。</span><span class="sxs-lookup"><span data-stu-id="5a4de-137">Possible value are: `unknown`, `audio`, `video`, `screenSharing`, `videoBasedScreenSharing`, `data`.</span></span> <span data-ttu-id="5a4de-138">(必須)</span><span class="sxs-lookup"><span data-stu-id="5a4de-138">(Required)</span></span> |
|<span data-ttu-id="5a4de-139">mediaConfig</span><span class="sxs-lookup"><span data-stu-id="5a4de-139">mediaConfig</span></span>       |[<span data-ttu-id="5a4de-140">mediaConfig</span><span class="sxs-lookup"><span data-stu-id="5a4de-140">mediaConfig</span></span>](../resources/mediaconfig.md)|<span data-ttu-id="5a4de-141">メディアの構成です。</span><span class="sxs-lookup"><span data-stu-id="5a4de-141">The media configuration.</span></span> <span data-ttu-id="5a4de-142">(必須)</span><span class="sxs-lookup"><span data-stu-id="5a4de-142">(Required)</span></span>                                                                                                            |

## <a name="response"></a><span data-ttu-id="5a4de-143">応答</span><span class="sxs-lookup"><span data-stu-id="5a4de-143">Response</span></span>
<span data-ttu-id="5a4de-144">このメソッドを返します`202 Accepted`応答コード。</span><span class="sxs-lookup"><span data-stu-id="5a4de-144">This method returns `202 Accepted` response code.</span></span>

## <a name="examples"></a><span data-ttu-id="5a4de-145">例</span><span class="sxs-lookup"><span data-stu-id="5a4de-145">Examples</span></span>
<span data-ttu-id="5a4de-146">次の例は、この API を呼び出す方法を示しています。</span><span class="sxs-lookup"><span data-stu-id="5a4de-146">The following example shows how to call this API.</span></span>

##### <a name="request"></a><span data-ttu-id="5a4de-147">要求</span><span class="sxs-lookup"><span data-stu-id="5a4de-147">Request</span></span>
<span data-ttu-id="5a4de-148">次の例は要求を示しています。</span><span class="sxs-lookup"><span data-stu-id="5a4de-148">The following example shows the request.</span></span>

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

##### <a name="response"></a><span data-ttu-id="5a4de-149">応答</span><span class="sxs-lookup"><span data-stu-id="5a4de-149">Response</span></span>
<span data-ttu-id="5a4de-150">以下は、応答の例です。</span><span class="sxs-lookup"><span data-stu-id="5a4de-150">Here is an example of the response.</span></span> 

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.None"
} -->
```http
HTTP/1.1 202 Accepted
```

### <a name="answer-voip-call-with-service-hosted-media"></a><span data-ttu-id="5a4de-151">サービスがホストされているメディアを使用して VOIP 通話に応答します。</span><span class="sxs-lookup"><span data-stu-id="5a4de-151">Answer VOIP call with service hosted media</span></span>

##### <a name="notification---incoming"></a><span data-ttu-id="5a4de-152">通知の受信</span><span class="sxs-lookup"><span data-stu-id="5a4de-152">Notification - incoming</span></span>

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

##### <a name="request"></a><span data-ttu-id="5a4de-153">要求</span><span class="sxs-lookup"><span data-stu-id="5a4de-153">Request</span></span>

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

##### <a name="response"></a><span data-ttu-id="5a4de-154">応答</span><span class="sxs-lookup"><span data-stu-id="5a4de-154">Response</span></span>

```http
HTTP/1.1 202 Accepted
```

##### <a name="notification---establishing"></a><span data-ttu-id="5a4de-155">通知を確立します。</span><span class="sxs-lookup"><span data-stu-id="5a4de-155">Notification - establishing</span></span>

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

##### <a name="notification---established"></a><span data-ttu-id="5a4de-156">通知の設定</span><span class="sxs-lookup"><span data-stu-id="5a4de-156">Notification - established</span></span>

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

### <a name="answer-voip-call-with-application-hosted-media"></a><span data-ttu-id="5a4de-157">アプリケーションがホストされているメディアを使用して VOIP 通話に応答します。</span><span class="sxs-lookup"><span data-stu-id="5a4de-157">Answer VOIP call with application hosted media</span></span>

##### <a name="notification---incoming"></a><span data-ttu-id="5a4de-158">通知の受信</span><span class="sxs-lookup"><span data-stu-id="5a4de-158">Notification - incoming</span></span>

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

##### <a name="request"></a><span data-ttu-id="5a4de-159">要求</span><span class="sxs-lookup"><span data-stu-id="5a4de-159">Request</span></span>

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

##### <a name="response"></a><span data-ttu-id="5a4de-160">応答</span><span class="sxs-lookup"><span data-stu-id="5a4de-160">Response</span></span>

```http
HTTP/1.1 202 Accepted
```

##### <a name="notification---establishing"></a><span data-ttu-id="5a4de-161">通知を確立します。</span><span class="sxs-lookup"><span data-stu-id="5a4de-161">Notification - establishing</span></span>

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

##### <a name="notification---established"></a><span data-ttu-id="5a4de-162">通知の設定</span><span class="sxs-lookup"><span data-stu-id="5a4de-162">Notification - established</span></span>

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
<!-- {
  "type": "#page.annotation",
  "description": "call: answer",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->