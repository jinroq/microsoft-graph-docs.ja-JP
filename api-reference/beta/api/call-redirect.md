---
title: 'call: redirect'
description: 着信をリダイレクトします。
author: VinodRavichandran
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: 9dcb8b6fd83f431bf5048bcc42b0de5d1ff55110
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/26/2019
ms.locfileid: "33328041"
---
# <a name="call-redirect"></a><span data-ttu-id="de06e-103">call: redirect</span><span class="sxs-lookup"><span data-stu-id="de06e-103">call: redirect</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="de06e-104">着信をリダイレクトします。</span><span class="sxs-lookup"><span data-stu-id="de06e-104">Redirect an incoming call.</span></span>

## <a name="permissions"></a><span data-ttu-id="de06e-105">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="de06e-105">Permissions</span></span>
<span data-ttu-id="de06e-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="de06e-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="de06e-108">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="de06e-108">Permission type</span></span> | <span data-ttu-id="de06e-109">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="de06e-109">Permissions (from least to most privileged)</span></span>         |
| :-------------- | :-------------------------------------------------- |
| <span data-ttu-id="de06e-110">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="de06e-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="de06e-111">サポート対象外</span><span class="sxs-lookup"><span data-stu-id="de06e-111">Not Supported</span></span>                |
| <span data-ttu-id="de06e-112">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="de06e-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="de06e-113">サポート対象外</span><span class="sxs-lookup"><span data-stu-id="de06e-113">Not Supported</span></span>                |
| <span data-ttu-id="de06e-114">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="de06e-114">Application</span></span>     | <span data-ttu-id="de06e-115">Calls.Initiate.All</span><span class="sxs-lookup"><span data-stu-id="de06e-115">Calls.Initiate.All</span></span>                                  |

## <a name="http-request"></a><span data-ttu-id="de06e-116">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="de06e-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /app/calls/{id}/redirect
POST /applications/{id}/calls/{id}/redirect
```

## <a name="request-headers"></a><span data-ttu-id="de06e-117">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="de06e-117">Request headers</span></span>
| <span data-ttu-id="de06e-118">名前</span><span class="sxs-lookup"><span data-stu-id="de06e-118">Name</span></span>          | <span data-ttu-id="de06e-119">説明</span><span class="sxs-lookup"><span data-stu-id="de06e-119">Description</span></span>               |
|:--------------|:--------------------------|
| <span data-ttu-id="de06e-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="de06e-120">Authorization</span></span> | <span data-ttu-id="de06e-p102">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="de06e-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="de06e-123">要求本文</span><span class="sxs-lookup"><span data-stu-id="de06e-123">Request body</span></span>
<span data-ttu-id="de06e-124">要求本文で、次のパラメーターを含む JSON オブジェクトを指定します。</span><span class="sxs-lookup"><span data-stu-id="de06e-124">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="de06e-125">パラメーター</span><span class="sxs-lookup"><span data-stu-id="de06e-125">Parameter</span></span>      | <span data-ttu-id="de06e-126">型</span><span class="sxs-lookup"><span data-stu-id="de06e-126">Type</span></span>    |<span data-ttu-id="de06e-127">説明</span><span class="sxs-lookup"><span data-stu-id="de06e-127">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="de06e-128">Targets</span><span class="sxs-lookup"><span data-stu-id="de06e-128">targets</span></span>|<span data-ttu-id="de06e-129">[invitationParticipantInfo](../resources/invitationparticipantinfo.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="de06e-129">[invitationParticipantInfo](../resources/invitationparticipantinfo.md) collection</span></span>|<span data-ttu-id="de06e-130">リダイレクト操作の対象となる参加者。</span><span class="sxs-lookup"><span data-stu-id="de06e-130">The target participants of the redirect operation.</span></span>|
|<span data-ttu-id="de06e-131">targetdisposition ポジション</span><span class="sxs-lookup"><span data-stu-id="de06e-131">targetDisposition</span></span>|<span data-ttu-id="de06e-132">String</span><span class="sxs-lookup"><span data-stu-id="de06e-132">String</span></span>|<span data-ttu-id="de06e-133">指定できる値は次のとおりです。`default`</span><span class="sxs-lookup"><span data-stu-id="de06e-133">The possible value is: `default`</span></span>|
|<span data-ttu-id="de06e-134">timeout</span><span class="sxs-lookup"><span data-stu-id="de06e-134">timeout</span></span>|<span data-ttu-id="de06e-135">Int32</span><span class="sxs-lookup"><span data-stu-id="de06e-135">Int32</span></span>|<span data-ttu-id="de06e-136">リダイレクト操作のタイムアウト (秒単位)。</span><span class="sxs-lookup"><span data-stu-id="de06e-136">The timeout in seconds for the redirect operation.</span></span>|
|<span data-ttu-id="de06e-137">maskcallee 先</span><span class="sxs-lookup"><span data-stu-id="de06e-137">maskCallee</span></span>|<span data-ttu-id="de06e-138">Boolean</span><span class="sxs-lookup"><span data-stu-id="de06e-138">Boolean</span></span>|<span data-ttu-id="de06e-139">呼び出し先をマスクするかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="de06e-139">Indicates whether to mask the callee.</span></span>|
|<span data-ttu-id="de06e-140">maskcaller</span><span class="sxs-lookup"><span data-stu-id="de06e-140">maskCaller</span></span>|<span data-ttu-id="de06e-141">Boolean</span><span class="sxs-lookup"><span data-stu-id="de06e-141">Boolean</span></span>|<span data-ttu-id="de06e-142">発信者をマスクするかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="de06e-142">Indicates whether to mask the caller.</span></span>|

## <a name="response"></a><span data-ttu-id="de06e-143">応答</span><span class="sxs-lookup"><span data-stu-id="de06e-143">Response</span></span>
<span data-ttu-id="de06e-144">応答`202 Accepted`コードを返します。</span><span class="sxs-lookup"><span data-stu-id="de06e-144">Returns `202 Accepted` response code</span></span>

## <a name="examples"></a><span data-ttu-id="de06e-145">例</span><span class="sxs-lookup"><span data-stu-id="de06e-145">Examples</span></span>

### <a name="redirect-a-call"></a><span data-ttu-id="de06e-146">通話をリダイレクトする</span><span class="sxs-lookup"><span data-stu-id="de06e-146">Redirect a call</span></span>

##### <a name="request"></a><span data-ttu-id="de06e-147">要求</span><span class="sxs-lookup"><span data-stu-id="de06e-147">Request</span></span>
<span data-ttu-id="de06e-148">次の例は要求を示しています。</span><span class="sxs-lookup"><span data-stu-id="de06e-148">The following example shows the request.</span></span>

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

##### <a name="response"></a><span data-ttu-id="de06e-149">応答</span><span class="sxs-lookup"><span data-stu-id="de06e-149">Response</span></span>

> <span data-ttu-id="de06e-p103">**注:** 読みやすくするために、ここに示す応答オブジェクトは短くされている場合があります。実際の呼び出しからは、すべてのプロパティが返されます。</span><span class="sxs-lookup"><span data-stu-id="de06e-p103">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.None"
} -->
```http
HTTP/1.1 202 Accepted
```

### <a name="forward-a-call"></a><span data-ttu-id="de06e-152">通話を転送する</span><span class="sxs-lookup"><span data-stu-id="de06e-152">Forward a call</span></span>

##### <a name="notification---incoming"></a><span data-ttu-id="de06e-153">通知-受信</span><span class="sxs-lookup"><span data-stu-id="de06e-153">Notification - incoming</span></span>

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

##### <a name="request"></a><span data-ttu-id="de06e-154">要求</span><span class="sxs-lookup"><span data-stu-id="de06e-154">Request</span></span>

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

##### <a name="response"></a><span data-ttu-id="de06e-155">応答</span><span class="sxs-lookup"><span data-stu-id="de06e-155">Response</span></span>

```http
HTTP/1.1 202 Accepted
```

##### <a name="notification---redirecting"></a><span data-ttu-id="de06e-156">通知-リダイレクト</span><span class="sxs-lookup"><span data-stu-id="de06e-156">Notification - redirecting</span></span>

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

##### <a name="notification---terminated"></a><span data-ttu-id="de06e-157">通知の終了</span><span class="sxs-lookup"><span data-stu-id="de06e-157">Notification - terminated</span></span>

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
  "suppressions": []
}
-->
