---
title: 呼び出しを作成します。
description: 新しい呼び出しを作成します。
author: VinodRavichandran
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: 60bd69bbef636f9e46f8f50a124b9a5a246dbe63
ms.sourcegitcommit: 66066b71d353fd7c2481d43b1dba2c33390eee61
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/26/2019
ms.locfileid: "29573943"
---
# <a name="create-call"></a><span data-ttu-id="6d9ee-103">呼び出しを作成します。</span><span class="sxs-lookup"><span data-stu-id="6d9ee-103">Create call</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="6d9ee-104">新しい呼び出しを作成します。</span><span class="sxs-lookup"><span data-stu-id="6d9ee-104">Create a new call.</span></span>

## <a name="permissions"></a><span data-ttu-id="6d9ee-105">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="6d9ee-105">Permissions</span></span>
<span data-ttu-id="6d9ee-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="6d9ee-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="6d9ee-108">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="6d9ee-108">Permission type</span></span>                        | <span data-ttu-id="6d9ee-109">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="6d9ee-109">Permissions (from least to most privileged)</span></span>                                             |
|:---------------------------------------|:----------------------------------------------------------------------------------------|
| <span data-ttu-id="6d9ee-110">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="6d9ee-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="6d9ee-111">サポート対象外</span><span class="sxs-lookup"><span data-stu-id="6d9ee-111">Not Supported</span></span>                                                                           |
| <span data-ttu-id="6d9ee-112">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="6d9ee-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="6d9ee-113">サポート対象外</span><span class="sxs-lookup"><span data-stu-id="6d9ee-113">Not Supported</span></span>                                                                           |
| <span data-ttu-id="6d9ee-114">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="6d9ee-114">Application</span></span>                            | <span data-ttu-id="6d9ee-115">Calls.JoinGroupCallsasGuest.All、Calls.JoinGroupCalls.All、Calls.Initiate.All、Calls.InitiateGroupCalls.All</span><span class="sxs-lookup"><span data-stu-id="6d9ee-115">Calls.JoinGroupCallsasGuest.All, Calls.JoinGroupCalls.All, Calls.Initiate.All, Calls.InitiateGroupCalls.All</span></span> |

> <span data-ttu-id="6d9ee-116">**注:** アプリケーションがホストされているメディアを使用して呼び出し、上記の表に記載されているアクセス許可のいずれかで Calls.AccessMedia.All のアクセス許可が必要です。</span><span class="sxs-lookup"><span data-stu-id="6d9ee-116">**Note:** For a call with app hosted media, you need the Calls.AccessMedia.All permission with one of the permissions listed in the previous table.</span></span>

## <a name="http-request"></a><span data-ttu-id="6d9ee-117">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="6d9ee-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /app/calls
POST /applications/{id}/calls
```

## <a name="request-headers"></a><span data-ttu-id="6d9ee-118">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="6d9ee-118">Request headers</span></span>
| <span data-ttu-id="6d9ee-119">名前</span><span class="sxs-lookup"><span data-stu-id="6d9ee-119">Name</span></span>          | <span data-ttu-id="6d9ee-120">説明</span><span class="sxs-lookup"><span data-stu-id="6d9ee-120">Description</span></span>               |
|:--------------|:--------------------------|
| <span data-ttu-id="6d9ee-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="6d9ee-121">Authorization</span></span> | <span data-ttu-id="6d9ee-p102">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="6d9ee-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="6d9ee-124">要求本文</span><span class="sxs-lookup"><span data-stu-id="6d9ee-124">Request body</span></span>
<span data-ttu-id="6d9ee-125">要求の本体[を呼び出す](../resources/call.md)オブジェクトの JSON の形式を指定します。</span><span class="sxs-lookup"><span data-stu-id="6d9ee-125">In the request body, supply a JSON representation of a [call](../resources/call.md) object.</span></span>

> <span data-ttu-id="6d9ee-126">**注:** プロパティとしてマーク`Server generated`を処理するときに無視されます`POST`の`app/calls`。</span><span class="sxs-lookup"><span data-stu-id="6d9ee-126">**Note:** Properties marked as `Server generated` are ignored when processing `POST` on `app/calls`.</span></span>

## <a name="response"></a><span data-ttu-id="6d9ee-127">応答</span><span class="sxs-lookup"><span data-stu-id="6d9ee-127">Response</span></span>
<span data-ttu-id="6d9ee-128">かどうかは成功すると、このメソッドが返されます、`201 Created`応答コードと応答の本文[を呼び出す](../resources/call.md)オブジェクト。</span><span class="sxs-lookup"><span data-stu-id="6d9ee-128">If successful, this method returns a `201 Created` response code and a [call](../resources/call.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="6d9ee-129">例</span><span class="sxs-lookup"><span data-stu-id="6d9ee-129">Examples</span></span>

### <a name="create-peer-to-peer-voip-call-with-service-hosted-media"></a><span data-ttu-id="6d9ee-130">サービスがホストされているメディアを使用してピア ツー ピアの VOIP 呼び出しを作成します。</span><span class="sxs-lookup"><span data-stu-id="6d9ee-130">Create peer to peer VOIP call with service hosted media</span></span>

> <span data-ttu-id="6d9ee-131">**注:** この呼び出しでは、Calls.Initiate.All アクセス許可が必要です。</span><span class="sxs-lookup"><span data-stu-id="6d9ee-131">**Note:** This call needs the Calls.Initiate.All permission.</span></span>

##### <a name="request"></a><span data-ttu-id="6d9ee-132">要求</span><span class="sxs-lookup"><span data-stu-id="6d9ee-132">Request</span></span>
<span data-ttu-id="6d9ee-133">次の例は要求を示しています。</span><span class="sxs-lookup"><span data-stu-id="6d9ee-133">The following example shows the request.</span></span>

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

##### <a name="response"></a><span data-ttu-id="6d9ee-134">応答</span><span class="sxs-lookup"><span data-stu-id="6d9ee-134">Response</span></span>

> <span data-ttu-id="6d9ee-p103">**注:** 読みやすくするために、ここに示す応答オブジェクトは短くされている場合があります。実際の呼び出しからは、すべてのプロパティが返されます。</span><span class="sxs-lookup"><span data-stu-id="6d9ee-p103">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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

##### <a name="notification---establishing"></a><span data-ttu-id="6d9ee-137">通知を確立します。</span><span class="sxs-lookup"><span data-stu-id="6d9ee-137">Notification - establishing</span></span>

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
##### <a name="notification---established"></a><span data-ttu-id="6d9ee-138">通知の設定</span><span class="sxs-lookup"><span data-stu-id="6d9ee-138">Notification - established</span></span>

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

### <a name="create-peer-to-peer-voip-call-with-application-hosted-media"></a><span data-ttu-id="6d9ee-139">アプリケーションがホストされているメディアを使用してピア ツー ピアの VOIP 呼び出しを作成します。</span><span class="sxs-lookup"><span data-stu-id="6d9ee-139">Create peer to peer VOIP call with application hosted media</span></span>

> <span data-ttu-id="6d9ee-140">注: 必要な権限を Calls.Initiate.All と Calls.AccessMedia.All。</span><span class="sxs-lookup"><span data-stu-id="6d9ee-140">Note: Needs Calls.Initiate.All and Calls.AccessMedia.All permission.</span></span>

##### <a name="request"></a><span data-ttu-id="6d9ee-141">要求</span><span class="sxs-lookup"><span data-stu-id="6d9ee-141">Request</span></span>
<span data-ttu-id="6d9ee-142">次の例は要求を示しています。</span><span class="sxs-lookup"><span data-stu-id="6d9ee-142">The following example shows the request.</span></span>

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

### <a name="create-group-call-with-service-hosted-media"></a><span data-ttu-id="6d9ee-143">サービスがホストされているメディアを使用して呼び出しのグループを作成します。</span><span class="sxs-lookup"><span data-stu-id="6d9ee-143">Create group call with service hosted media</span></span>

> <span data-ttu-id="6d9ee-144">**注:** この例では、Calls.InitiateGroupCalls.All と Calls.AccessMedia.All のアクセス許可が必要です。</span><span class="sxs-lookup"><span data-stu-id="6d9ee-144">**Note:** This example needs the Calls.InitiateGroupCalls.All and Calls.AccessMedia.All permissions.</span></span>

##### <a name="request"></a><span data-ttu-id="6d9ee-145">要求</span><span class="sxs-lookup"><span data-stu-id="6d9ee-145">Request</span></span>

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

### <a name="join-private-meeting-with-service-hosted-media"></a><span data-ttu-id="6d9ee-146">サービスがホストされているメディアを使用してプライベートな会議に参加します。</span><span class="sxs-lookup"><span data-stu-id="6d9ee-146">Join private meeting with service hosted media</span></span>

> <span data-ttu-id="6d9ee-147">**注:** この例では、Calls.JoinGroupCalls.All アクセス許可が必要です。</span><span class="sxs-lookup"><span data-stu-id="6d9ee-147">**Note:** This example needs the Calls.JoinGroupCalls.All permission.</span></span>

##### <a name="request"></a><span data-ttu-id="6d9ee-148">要求</span><span class="sxs-lookup"><span data-stu-id="6d9ee-148">Request</span></span>

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

### <a name="join-channel-meeting-with-service-hosted-media"></a><span data-ttu-id="6d9ee-149">サービスがホストされているメディアを使用してチャネルの会議に参加します。</span><span class="sxs-lookup"><span data-stu-id="6d9ee-149">Join channel meeting with service hosted media</span></span>

> <span data-ttu-id="6d9ee-150">**注:** この例では、Calls.JoinGroupCalls.All アクセス許可が必要です。</span><span class="sxs-lookup"><span data-stu-id="6d9ee-150">**Note:** This example needs the Calls.JoinGroupCalls.All permission.</span></span>

##### <a name="request"></a><span data-ttu-id="6d9ee-151">要求</span><span class="sxs-lookup"><span data-stu-id="6d9ee-151">Request</span></span>

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

### <a name="join-channel-meeting-as-a-guest-with-service-hosted-media"></a><span data-ttu-id="6d9ee-152">サービスがホストされているメディアを使用してゲストとしてチャネルの会議に参加します。</span><span class="sxs-lookup"><span data-stu-id="6d9ee-152">Join channel meeting as a guest with service hosted media</span></span>

> <span data-ttu-id="6d9ee-153">**注:** この例では、Calls.JoinGroupCallsAsGuest.All アクセス許可が必要です。</span><span class="sxs-lookup"><span data-stu-id="6d9ee-153">**Note:** This example needs the Calls.JoinGroupCallsAsGuest.All permission.</span></span>

##### <a name="request"></a><span data-ttu-id="6d9ee-154">要求</span><span class="sxs-lookup"><span data-stu-id="6d9ee-154">Request</span></span>

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
<!--
{
  "type": "#page.annotation",
  "description": "Create call",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/application-post-calls.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
