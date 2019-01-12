---
title: '呼び出す: リダイレクト'
description: 着信呼び出しをリダイレクトします。
author: VinodRavichandran
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: 20470a57358caea08116bbacf6348d659d0d3636
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/12/2019
ms.locfileid: "27921725"
---
# <a name="call-redirect"></a><span data-ttu-id="bf17b-103">呼び出す: リダイレクト</span><span class="sxs-lookup"><span data-stu-id="bf17b-103">call: redirect</span></span>

> <span data-ttu-id="bf17b-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="bf17b-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="bf17b-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="bf17b-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="bf17b-106">着信呼び出しをリダイレクトします。</span><span class="sxs-lookup"><span data-stu-id="bf17b-106">Redirect an incoming call.</span></span>

## <a name="permissions"></a><span data-ttu-id="bf17b-107">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="bf17b-107">Permissions</span></span>
<span data-ttu-id="bf17b-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="bf17b-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="bf17b-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="bf17b-110">Permission type</span></span> | <span data-ttu-id="bf17b-111">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="bf17b-111">Permissions (from least to most privileged)</span></span>         |
| :-------------- | :-------------------------------------------------- |
| <span data-ttu-id="bf17b-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="bf17b-112">Delegated (work or school account)</span></span>     | <span data-ttu-id="bf17b-113">サポート対象外</span><span class="sxs-lookup"><span data-stu-id="bf17b-113">Not Supported</span></span>                |
| <span data-ttu-id="bf17b-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="bf17b-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="bf17b-115">サポート対象外</span><span class="sxs-lookup"><span data-stu-id="bf17b-115">Not Supported</span></span>                |
| <span data-ttu-id="bf17b-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="bf17b-116">Application</span></span>     | <span data-ttu-id="bf17b-117">Calls.Initiate.All</span><span class="sxs-lookup"><span data-stu-id="bf17b-117">Calls.Initiate.All</span></span>                                  |

## <a name="http-request"></a><span data-ttu-id="bf17b-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="bf17b-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /app/calls/{id}/redirect
POST /applications/{id}/calls/{id}/redirect
```

## <a name="request-headers"></a><span data-ttu-id="bf17b-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="bf17b-119">Request headers</span></span>
| <span data-ttu-id="bf17b-120">名前</span><span class="sxs-lookup"><span data-stu-id="bf17b-120">Name</span></span>          | <span data-ttu-id="bf17b-121">説明</span><span class="sxs-lookup"><span data-stu-id="bf17b-121">Description</span></span>               |
|:--------------|:--------------------------|
| <span data-ttu-id="bf17b-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="bf17b-122">Authorization</span></span> | <span data-ttu-id="bf17b-p103">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="bf17b-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="bf17b-125">要求本文</span><span class="sxs-lookup"><span data-stu-id="bf17b-125">Request body</span></span>
<span data-ttu-id="bf17b-126">要求本文で、次のパラメーターを含む JSON オブジェクトを指定します。</span><span class="sxs-lookup"><span data-stu-id="bf17b-126">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="bf17b-127">パラメーター</span><span class="sxs-lookup"><span data-stu-id="bf17b-127">Parameter</span></span>      | <span data-ttu-id="bf17b-128">型</span><span class="sxs-lookup"><span data-stu-id="bf17b-128">Type</span></span>    |<span data-ttu-id="bf17b-129">説明</span><span class="sxs-lookup"><span data-stu-id="bf17b-129">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="bf17b-130">ターゲット</span><span class="sxs-lookup"><span data-stu-id="bf17b-130">targets</span></span>|<span data-ttu-id="bf17b-131">[invitationParticipantInfo](../resources/invitationparticipantinfo.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="bf17b-131">[invitationParticipantInfo](../resources/invitationparticipantinfo.md) collection</span></span>|<span data-ttu-id="bf17b-132">リダイレクト操作のターゲットの参加者です。</span><span class="sxs-lookup"><span data-stu-id="bf17b-132">The target participants of the redirect operation.</span></span>|
|<span data-ttu-id="bf17b-133">targetDisposition</span><span class="sxs-lookup"><span data-stu-id="bf17b-133">targetDisposition</span></span>|<span data-ttu-id="bf17b-134">String</span><span class="sxs-lookup"><span data-stu-id="bf17b-134">String</span></span>|<span data-ttu-id="bf17b-135">使用可能な値は次のとおりです。`default`</span><span class="sxs-lookup"><span data-stu-id="bf17b-135">The possible value is: `default`</span></span>|
|<span data-ttu-id="bf17b-136">timeout</span><span class="sxs-lookup"><span data-stu-id="bf17b-136">timeout</span></span>|<span data-ttu-id="bf17b-137">Int32</span><span class="sxs-lookup"><span data-stu-id="bf17b-137">Int32</span></span>|<span data-ttu-id="bf17b-138">リダイレクト処理を秒単位でタイムアウトします。</span><span class="sxs-lookup"><span data-stu-id="bf17b-138">The timeout in seconds for the redirect operation.</span></span>|
|<span data-ttu-id="bf17b-139">maskCallee</span><span class="sxs-lookup"><span data-stu-id="bf17b-139">maskCallee</span></span>|<span data-ttu-id="bf17b-140">Boolean</span><span class="sxs-lookup"><span data-stu-id="bf17b-140">Boolean</span></span>|<span data-ttu-id="bf17b-141">呼び出し先をマスクするかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="bf17b-141">Indicates whether to mask the callee.</span></span>|
|<span data-ttu-id="bf17b-142">maskCaller</span><span class="sxs-lookup"><span data-stu-id="bf17b-142">maskCaller</span></span>|<span data-ttu-id="bf17b-143">Boolean</span><span class="sxs-lookup"><span data-stu-id="bf17b-143">Boolean</span></span>|<span data-ttu-id="bf17b-144">呼び出し元をマスクするかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="bf17b-144">Indicates whether to mask the caller.</span></span>|

## <a name="response"></a><span data-ttu-id="bf17b-145">応答</span><span class="sxs-lookup"><span data-stu-id="bf17b-145">Response</span></span>
<span data-ttu-id="bf17b-146">返します`202 Accepted`応答コード。</span><span class="sxs-lookup"><span data-stu-id="bf17b-146">Returns `202 Accepted` response code</span></span>

## <a name="examples"></a><span data-ttu-id="bf17b-147">例</span><span class="sxs-lookup"><span data-stu-id="bf17b-147">Examples</span></span>

### <a name="redirect-a-call"></a><span data-ttu-id="bf17b-148">呼び出しをリダイレクトします。</span><span class="sxs-lookup"><span data-stu-id="bf17b-148">Redirect a call</span></span>

##### <a name="request"></a><span data-ttu-id="bf17b-149">要求</span><span class="sxs-lookup"><span data-stu-id="bf17b-149">Request</span></span>
<span data-ttu-id="bf17b-150">次の例は要求を示しています。</span><span class="sxs-lookup"><span data-stu-id="bf17b-150">The following example shows the request.</span></span>

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

##### <a name="response"></a><span data-ttu-id="bf17b-151">応答</span><span class="sxs-lookup"><span data-stu-id="bf17b-151">Response</span></span>

> <span data-ttu-id="bf17b-p104">**注:** 読みやすくするために、ここに示す応答オブジェクトは短くされている場合があります。実際の呼び出しからは、すべてのプロパティが返されます。</span><span class="sxs-lookup"><span data-stu-id="bf17b-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.None"
} -->
```http
HTTP/1.1 202 Accepted
```

### <a name="forward-a-call"></a><span data-ttu-id="bf17b-154">呼び出しを転送します。</span><span class="sxs-lookup"><span data-stu-id="bf17b-154">Forward a call</span></span>

##### <a name="notification---incoming"></a><span data-ttu-id="bf17b-155">通知の受信</span><span class="sxs-lookup"><span data-stu-id="bf17b-155">Notification - incoming</span></span>

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

##### <a name="request"></a><span data-ttu-id="bf17b-156">要求</span><span class="sxs-lookup"><span data-stu-id="bf17b-156">Request</span></span>

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

##### <a name="response"></a><span data-ttu-id="bf17b-157">応答</span><span class="sxs-lookup"><span data-stu-id="bf17b-157">Response</span></span>

```http
HTTP/1.1 202 Accepted
```

##### <a name="notification---redirecting"></a><span data-ttu-id="bf17b-158">通知のリダイレクト</span><span class="sxs-lookup"><span data-stu-id="bf17b-158">Notification - redirecting</span></span>

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

##### <a name="notification---terminated"></a><span data-ttu-id="bf17b-159">終了の通知-</span><span class="sxs-lookup"><span data-stu-id="bf17b-159">Notification - terminated</span></span>

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
<!-- {
  "type": "#page.annotation",
  "description": "call: redirect",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
