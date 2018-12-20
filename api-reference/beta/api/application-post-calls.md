---
title: 呼び出しを作成します。
description: 新しい呼び出しを作成します。
author: VinodRavichandran
ms.openlocfilehash: a2d34ccf3d77d165b8a92114353d5f6cb8bed674
ms.sourcegitcommit: 0b3a57ac8b99871e56389f9be15e4f96e219f635
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 12/20/2018
ms.locfileid: "27380388"
---
# <a name="create-call"></a><span data-ttu-id="7318d-103">呼び出しを作成します。</span><span class="sxs-lookup"><span data-stu-id="7318d-103">Create call</span></span>

> <span data-ttu-id="7318d-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="7318d-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="7318d-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="7318d-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="7318d-106">新しい呼び出しを作成します。</span><span class="sxs-lookup"><span data-stu-id="7318d-106">Create a new call.</span></span>

## <a name="permissions"></a><span data-ttu-id="7318d-107">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="7318d-107">Permissions</span></span>
<span data-ttu-id="7318d-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="7318d-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="7318d-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="7318d-110">Permission type</span></span>                        | <span data-ttu-id="7318d-111">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="7318d-111">Permissions (from least to most privileged)</span></span>                                             |
|:---------------------------------------|:----------------------------------------------------------------------------------------|
| <span data-ttu-id="7318d-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="7318d-112">Delegated (work or school account)</span></span>     | <span data-ttu-id="7318d-113">サポート対象外</span><span class="sxs-lookup"><span data-stu-id="7318d-113">Not Supported</span></span>                                                                           |
| <span data-ttu-id="7318d-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="7318d-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="7318d-115">サポート対象外</span><span class="sxs-lookup"><span data-stu-id="7318d-115">Not Supported</span></span>                                                                           |
| <span data-ttu-id="7318d-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="7318d-116">Application</span></span>                            | <span data-ttu-id="7318d-117">Calls.JoinGroupCallsasGuest.All、Calls.JoinGroupCalls.All、Calls.Initiate.All、Calls.InitiateGroupCalls.All</span><span class="sxs-lookup"><span data-stu-id="7318d-117">Calls.JoinGroupCallsasGuest.All, Calls.JoinGroupCalls.All, Calls.Initiate.All, Calls.InitiateGroupCalls.All</span></span> |

> <span data-ttu-id="7318d-118">**注:** アプリケーションがホストされているメディアを使用して呼び出し、上記の表に記載されているアクセス許可のいずれかで Calls.AccessMedia.All のアクセス許可が必要です。</span><span class="sxs-lookup"><span data-stu-id="7318d-118">**Note:** For a call with app hosted media, you need the Calls.AccessMedia.All permission with one of the permissions listed in the previous table.</span></span>

## <a name="http-request"></a><span data-ttu-id="7318d-119">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="7318d-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /app/calls
POST /applications/{id}/calls
```

## <a name="request-headers"></a><span data-ttu-id="7318d-120">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="7318d-120">Request headers</span></span>
| <span data-ttu-id="7318d-121">名前</span><span class="sxs-lookup"><span data-stu-id="7318d-121">Name</span></span>          | <span data-ttu-id="7318d-122">説明</span><span class="sxs-lookup"><span data-stu-id="7318d-122">Description</span></span>               |
|:--------------|:--------------------------|
| <span data-ttu-id="7318d-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="7318d-123">Authorization</span></span> | <span data-ttu-id="7318d-p103">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="7318d-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="7318d-126">要求本文</span><span class="sxs-lookup"><span data-stu-id="7318d-126">Request body</span></span>
<span data-ttu-id="7318d-127">要求の本体[を呼び出す](../resources/call.md)オブジェクトの JSON の形式を指定します。</span><span class="sxs-lookup"><span data-stu-id="7318d-127">In the request body, supply a JSON representation of a [call](../resources/call.md) object.</span></span>

> <span data-ttu-id="7318d-128">**注:** プロパティとしてマーク`Server generated`を処理するときに無視されます`POST`の`app/calls`。</span><span class="sxs-lookup"><span data-stu-id="7318d-128">**Note:** Properties marked as `Server generated` are ignored when processing `POST` on `app/calls`.</span></span>

## <a name="response"></a><span data-ttu-id="7318d-129">応答</span><span class="sxs-lookup"><span data-stu-id="7318d-129">Response</span></span>
<span data-ttu-id="7318d-130">かどうかは成功すると、このメソッドが返されます、`201 Created`応答コードと応答の本文[を呼び出す](../resources/call.md)オブジェクト。</span><span class="sxs-lookup"><span data-stu-id="7318d-130">If successful, this method returns a `201 Created` response code and a [call](../resources/call.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="7318d-131">例</span><span class="sxs-lookup"><span data-stu-id="7318d-131">Examples</span></span>

### <a name="create-peer-to-peer-voip-call-with-service-hosted-media"></a><span data-ttu-id="7318d-132">サービスがホストされているメディアを使用してピア ツー ピアの VOIP 呼び出しを作成します。</span><span class="sxs-lookup"><span data-stu-id="7318d-132">Create peer to peer VOIP call with service hosted media</span></span>

> <span data-ttu-id="7318d-133">**注:** この呼び出しでは、Calls.Initiate.All アクセス許可が必要です。</span><span class="sxs-lookup"><span data-stu-id="7318d-133">**Note:** This call needs the Calls.Initiate.All permission.</span></span>

##### <a name="request"></a><span data-ttu-id="7318d-134">要求</span><span class="sxs-lookup"><span data-stu-id="7318d-134">Request</span></span>
<span data-ttu-id="7318d-135">次の例は要求を示しています。</span><span class="sxs-lookup"><span data-stu-id="7318d-135">The following example shows the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "create-call-from-application"
}-->
```http
POST https://graph.microsoft.com/beta/app/calls
Content-Type: application/json

{
  "callbackUri": "https://bot.contoso.com/api/calls",
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
  },
  "source": {
    "identity": {
      "application": {
        "id": "8A34A46B-3D17-4ADC-8DCE-DC4E7D572698"
      }
    },
    "languageId": "languageId-value",
    "region": "region-value"
  },
  "subject": "Test Call",
  "targets": [
    {
      "identity": {
        "user": {
          "id": "550fae72-d251-43ec-868c-373732c2704f",
          "tenantId": "72f988bf-86f1-41af-91ab-2d7cd011db47",
          "displayName": "Heidi Steen"
        }
      }
    }
  ],
  "tenantId": "tenantId-value"
}
```

##### <a name="response"></a><span data-ttu-id="7318d-136">応答</span><span class="sxs-lookup"><span data-stu-id="7318d-136">Response</span></span>

> <span data-ttu-id="7318d-p104">**注:** 読みやすくするために、ここに示す応答オブジェクトは短くされている場合があります。実際の呼び出しからは、すべてのプロパティが返されます。</span><span class="sxs-lookup"><span data-stu-id="7318d-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.call"
} -->
```http
HTTP/1.1 201 Created
Content-Type: application/json


{
  "id": "57DAB8B1894C409AB240BD8BEAE78896",
  "callbackUri": "https://bot.contoso.com/api/calls",
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
  },
  "source": {
    "identity": {
      "application": {
        "id": "8A34A46B-3D17-4ADC-8DCE-DC4E7D572698"
      }
    },
    "languageId": "languageId-value",
    "region": "region-value"
  },
  "subject": "Test Call",
  "targets": [
    {
      "identity": {
        "user": {
          "id": "550fae72-d251-43ec-868c-373732c2704f",
          "tenantId": "72f988bf-86f1-41af-91ab-2d7cd011db47",
          "displayName": "Heidi Steen"
        }
      }
    }
  ],
  "tenantId": "tenantId-value"
}
```

##### <a name="notification---establishing"></a><span data-ttu-id="7318d-139">通知を確立します。</span><span class="sxs-lookup"><span data-stu-id="7318d-139">Notification - establishing</span></span>

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
        "state": "establishing",
        "direction": "outgoing"
      }
    }
  ]
}
```
##### <a name="notification---established"></a><span data-ttu-id="7318d-140">通知の設定</span><span class="sxs-lookup"><span data-stu-id="7318d-140">Notification - established</span></span>

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

### <a name="create-peer-to-peer-voip-call-with-application-hosted-media"></a><span data-ttu-id="7318d-141">アプリケーションがホストされているメディアを使用してピア ツー ピアの VOIP 呼び出しを作成します。</span><span class="sxs-lookup"><span data-stu-id="7318d-141">Create peer to peer VOIP call with application hosted media</span></span>

> <span data-ttu-id="7318d-142">注: 必要な権限を Calls.Initiate.All と Calls.AccessMedia.All。</span><span class="sxs-lookup"><span data-stu-id="7318d-142">Note: Needs Calls.Initiate.All and Calls.AccessMedia.All permission.</span></span>

##### <a name="request"></a><span data-ttu-id="7318d-143">要求</span><span class="sxs-lookup"><span data-stu-id="7318d-143">Request</span></span>
<span data-ttu-id="7318d-144">次の例は要求を示しています。</span><span class="sxs-lookup"><span data-stu-id="7318d-144">The following example shows the request.</span></span>

```http
POST https://graph.microsoft.com/beta/app/calls
Content-Type: application/json
```

<!-- {
  "blockType": "example",
  "@odata.type": "microsoft.graph.call"
}-->
```json
{
  "callbackUri": "https://bot.contoso.com/api/calls",
  "mediaConfig": {
    "@odata.type": "#microsoft.graph.appHostedMediaConfig",
    "blob": "<media config blob>"
  },
  "requestedModalities": [ "audio" ],
  "source": {
    "identity": {
      "application": {
        "id": "550fae72-d251-43ec-868c-373732c2704f",
        "tenantId": "72f988bf-86f1-41af-91ab-2d7cd011db47",
        "displayName": "IT Bot"
      }
    },
    "languageId": "languageId-value",
    "region": "region-value"
  },
  "subject": "Test Call",
  "targets": [
    {
      "identity": {
        "user": {
          "id": "550fae72-d251-43ec-868c-373732c2704f",
          "tenantId": "72f988bf-86f1-41af-91ab-2d7cd011db47",
          "displayName": "Heidi Steen"
        }
      }
    }
  ],
  "tenantId": "tenantId-value"
}
```

### <a name="create-group-call-with-service-hosted-media"></a><span data-ttu-id="7318d-145">サービスがホストされているメディアを使用して呼び出しのグループを作成します。</span><span class="sxs-lookup"><span data-stu-id="7318d-145">Create group call with service hosted media</span></span>

> <span data-ttu-id="7318d-146">**注:** この例では、Calls.InitiateGroupCalls.All と Calls.AccessMedia.All のアクセス許可が必要です。</span><span class="sxs-lookup"><span data-stu-id="7318d-146">**Note:** This example needs the Calls.InitiateGroupCalls.All and Calls.AccessMedia.All permissions.</span></span>

##### <a name="request"></a><span data-ttu-id="7318d-147">要求</span><span class="sxs-lookup"><span data-stu-id="7318d-147">Request</span></span>

```http
POST https://graph.microsoft.com/beta/app/calls
Content-Type: application/json
```

<!-- {
  "blockType": "example",
  "@odata.type": "microsoft.graph.call"
}-->
```json
{
  "subject": "Test Call",
  "callbackUri": "https://bot.contoso.com/api/calls",
  "source": {
    "identity": {
      "application": {
        "id": "8A34A46B-3D17-4ADC-8DCE-DC4E7D572698"
      }
    }
  },
  "targets": [
    {
      "identity": {
        "user": {
          "id": "29362BD4-CD58-4ED0-A206-0E4A33DBB0B6",
          "displayName": "Heidi Steen"
        }
      }
    },
    {
      "identity": {
        "phone": {
          "displayName": "+12345678890",
          "id": "+12345678890"
        }
      }
    }
  ],
  "requestedModalities": [ "audio", "video" ],
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
  },
  "chatInfo": {
    "threadId": "19:meeting_NTg0NmQ3NTctZDVkZC00YzRhLThmNmEtOGQ3M2E0ODdmZDZk@thread.v2",
    "messageId": "0",
    "replyChainMessageId": null
  }
}
```

### <a name="join-private-meeting-with-service-hosted-media"></a><span data-ttu-id="7318d-148">サービスがホストされているメディアを使用してプライベートな会議に参加します。</span><span class="sxs-lookup"><span data-stu-id="7318d-148">Join private meeting with service hosted media</span></span>

> <span data-ttu-id="7318d-149">**注:** この例では、Calls.JoinGroupCalls.All アクセス許可が必要です。</span><span class="sxs-lookup"><span data-stu-id="7318d-149">**Note:** This example needs the Calls.JoinGroupCalls.All permission.</span></span>

##### <a name="request"></a><span data-ttu-id="7318d-150">要求</span><span class="sxs-lookup"><span data-stu-id="7318d-150">Request</span></span>

```http
POST https://graph.microsoft.com/beta/app/calls
Content-Type: application/json
```

<!-- {
  "blockType": "example",
  "@odata.type": "microsoft.graph.call"
}-->
```json
{
  "subject": "Test Call",
  "callbackUri": "https://bot.contoso.com/api/calls",
  "source": {
    "identity": {
      "application": {
        "id": "8A34A46B-3D17-4ADC-8DCE-DC4E7D572698"
      }
    }
  },
  "requestedModalities": [ "audio", "video" ],
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
  },
  "chatInfo": {
    "threadId": "19:meeting_NTg0NmQ3NTctZDVkZC00YzRhLThmNmEtOGQ3M2E0ODdmZDZk@thread.v2",
    "messageId": "0"
  },
  "meetingInfo": {
    "@odata.type": "#microsoft.graph.organizerMeetingInfo",
    "organizer": {
      "user": {
        "id": "90ED37DC-D8E3-4E11-9DE3-30A955DDA06F",
        "tenantId": "49BFC225-8482-4AB8-94E7-76B48FDB9849"
      }
    }
  }
}
```

### <a name="join-channel-meeting-with-service-hosted-media"></a><span data-ttu-id="7318d-151">サービスがホストされているメディアを使用してチャネルの会議に参加します。</span><span class="sxs-lookup"><span data-stu-id="7318d-151">Join channel meeting with service hosted media</span></span>

> <span data-ttu-id="7318d-152">**注:** この例では、Calls.JoinGroupCalls.All アクセス許可が必要です。</span><span class="sxs-lookup"><span data-stu-id="7318d-152">**Note:** This example needs the Calls.JoinGroupCalls.All permission.</span></span>

##### <a name="request"></a><span data-ttu-id="7318d-153">要求</span><span class="sxs-lookup"><span data-stu-id="7318d-153">Request</span></span>

```http
POST https://graph.microsoft.com/beta/app/calls
Content-Type: application/json
```

<!-- {
  "blockType": "example",
  "@odata.type": "microsoft.graph.call"
}-->
```json
{
  "subject": "Test Call",
  "callbackUri": "https://bot.contoso.com/api/calls",
  "source": {
    "identity": {
      "application": {
        "id": "8A34A46B-3D17-4ADC-8DCE-DC4E7D572698"
      }
    }
  },
  "requestedModalities": [ "audio", "video" ],
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
  },
  "chatInfo": {
    "threadId": "19:meeting_NTg0NmQ3NTctZDVkZC00YzRhLThmNmEtOGQ3M2E0ODdmZDZk@thread.v2",
    "messageId": "1507228578052",
    "replyChainMessageId": null
  },
  "meetingInfo": {
    "@odata.type": "#microsoft.graph.organizerMeetingInfo",
    "organizer": {
      "user": {
        "id": "90ED37DC-D8E3-4E11-9DE3-30A955DDA06F",
        "tenantId": "49BFC225-8482-4AB8-94E7-76B48FDB9849"
      }
    }
  }
}
```

### <a name="join-channel-meeting-as-a-guest-with-service-hosted-media"></a><span data-ttu-id="7318d-154">サービスがホストされているメディアを使用してゲストとしてチャネルの会議に参加します。</span><span class="sxs-lookup"><span data-stu-id="7318d-154">Join channel meeting as a guest with service hosted media</span></span>

> <span data-ttu-id="7318d-155">**注:** この例では、Calls.JoinGroupCallsAsGuest.All アクセス許可が必要です。</span><span class="sxs-lookup"><span data-stu-id="7318d-155">**Note:** This example needs the Calls.JoinGroupCallsAsGuest.All permission.</span></span>

##### <a name="request"></a><span data-ttu-id="7318d-156">要求</span><span class="sxs-lookup"><span data-stu-id="7318d-156">Request</span></span>

```http
POST https://graph.microsoft.com/beta/app/calls
Content-Type: application/json
```
<!-- {
  "blockType": "example",
  "@odata.type": "microsoft.graph.call"
}-->
```json
{
  "subject": "Test Call",
  "callbackUri": "https://bot.contoso.com/api/calls",
  "source": {
    "identity": {
      "user": {
        "id": "8A34A46B-3D17-4ADC-8DCE-DC4E7D572698",
        "displayName": "App_Guest_DisplayName",
        "identityProvider": "None"
      }
    }
  },
  "requestedModalities": [ "audio", "video" ],
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
  },
  "chatInfo": {
    "threadId": "19:meeting_NTg0NmQ3NTctZDVkZC00YzRhLThmNmEtOGQ3M2E0ODdmZDZk@thread.v2",
    "messageId": "1507228578052",
    "replyChainMessageId": null
  },
  "meetingInfo": {
    "@odata.type": "#microsoft.graph.organizerMeetingInfo",
    "organizer": {
      "user": {
        "id": "90ED37DC-D8E3-4E11-9DE3-30A955DDA06F",
        "tenantId": "49BFC225-8482-4AB8-94E7-76B48FDB9849"
      }
    }
  }
}
```
<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Create call",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
