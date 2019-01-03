---
title: '呼び出す: 転送'
description: アクティブな呼び出しを転送します。
author: VinodRavichandran
ms.openlocfilehash: 71d250453051c705dcc0646a8e4ad298253d0ee6
ms.sourcegitcommit: 0b3a57ac8b99871e56389f9be15e4f96e219f635
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 12/20/2018
ms.locfileid: "27380507"
---
# <a name="call-transfer"></a><span data-ttu-id="1cc26-103">呼び出す: 転送</span><span class="sxs-lookup"><span data-stu-id="1cc26-103">call: transfer</span></span>

> <span data-ttu-id="1cc26-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="1cc26-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="1cc26-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="1cc26-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="1cc26-106">アクティブな呼び出しを転送します。</span><span class="sxs-lookup"><span data-stu-id="1cc26-106">Transfer an active call.</span></span>

## <a name="permissions"></a><span data-ttu-id="1cc26-107">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="1cc26-107">Permissions</span></span>
<span data-ttu-id="1cc26-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="1cc26-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="1cc26-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="1cc26-110">Permission type</span></span> | <span data-ttu-id="1cc26-111">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="1cc26-111">Permissions (from least to most privileged)</span></span>         |
| :-------------- | :-------------------------------------------------- |
| <span data-ttu-id="1cc26-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="1cc26-112">Delegated (work or school account)</span></span>     | <span data-ttu-id="1cc26-113">サポート対象外</span><span class="sxs-lookup"><span data-stu-id="1cc26-113">Not Supported</span></span>                |
| <span data-ttu-id="1cc26-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="1cc26-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="1cc26-115">サポート対象外</span><span class="sxs-lookup"><span data-stu-id="1cc26-115">Not Supported</span></span>                |
| <span data-ttu-id="1cc26-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="1cc26-116">Application</span></span>     | <span data-ttu-id="1cc26-117">Calls.Initiate.All</span><span class="sxs-lookup"><span data-stu-id="1cc26-117">Calls.Initiate.All</span></span>                                  |

## <a name="http-request"></a><span data-ttu-id="1cc26-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="1cc26-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /app/calls/{id}/transfer
POST /applications/{id}/calls/{id}/transfer
```

## <a name="request-headers"></a><span data-ttu-id="1cc26-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="1cc26-119">Request headers</span></span>
| <span data-ttu-id="1cc26-120">名前</span><span class="sxs-lookup"><span data-stu-id="1cc26-120">Name</span></span>          | <span data-ttu-id="1cc26-121">説明</span><span class="sxs-lookup"><span data-stu-id="1cc26-121">Description</span></span>               |
|:--------------|:--------------------------|
| <span data-ttu-id="1cc26-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="1cc26-122">Authorization</span></span> | <span data-ttu-id="1cc26-p103">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="1cc26-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="1cc26-125">要求本文</span><span class="sxs-lookup"><span data-stu-id="1cc26-125">Request body</span></span>
<span data-ttu-id="1cc26-126">要求本文で、次のパラメーターを含む JSON オブジェクトを指定します。</span><span class="sxs-lookup"><span data-stu-id="1cc26-126">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="1cc26-127">パラメーター</span><span class="sxs-lookup"><span data-stu-id="1cc26-127">Parameter</span></span>      | <span data-ttu-id="1cc26-128">型</span><span class="sxs-lookup"><span data-stu-id="1cc26-128">Type</span></span>    |<span data-ttu-id="1cc26-129">説明</span><span class="sxs-lookup"><span data-stu-id="1cc26-129">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="1cc26-130">transferTarget</span><span class="sxs-lookup"><span data-stu-id="1cc26-130">transferTarget</span></span>|[<span data-ttu-id="1cc26-131">invitationParticipantInfo</span><span class="sxs-lookup"><span data-stu-id="1cc26-131">invitationParticipantInfo</span></span>](../resources/invitationparticipantinfo.md)|<span data-ttu-id="1cc26-132">転送の対象である構成要素です。</span><span class="sxs-lookup"><span data-stu-id="1cc26-132">The participant which is the target of the transfer.</span></span>|
|<span data-ttu-id="1cc26-133">clientContext</span><span class="sxs-lookup"><span data-stu-id="1cc26-133">clientContext</span></span>|<span data-ttu-id="1cc26-134">String</span><span class="sxs-lookup"><span data-stu-id="1cc26-134">String</span></span>|<span data-ttu-id="1cc26-135">クライアントのコンテキスト。</span><span class="sxs-lookup"><span data-stu-id="1cc26-135">The client context.</span></span>|

## <a name="response"></a><span data-ttu-id="1cc26-136">応答</span><span class="sxs-lookup"><span data-stu-id="1cc26-136">Response</span></span>
<span data-ttu-id="1cc26-137">返します。`202 Accepted`応答コード。</span><span class="sxs-lookup"><span data-stu-id="1cc26-137">Returns `202 Accepted` response code.</span></span>

## <a name="examples"></a><span data-ttu-id="1cc26-138">例</span><span class="sxs-lookup"><span data-stu-id="1cc26-138">Examples</span></span>

### <a name="transfer-call-directly-with-no-user-involvement"></a><span data-ttu-id="1cc26-139">ユーザーの関与なしに直接、電話を転送します。</span><span class="sxs-lookup"><span data-stu-id="1cc26-139">Transfer call directly, with no user involvement</span></span>

<span data-ttu-id="1cc26-140">次の例は、この API を呼び出す方法を示しています。</span><span class="sxs-lookup"><span data-stu-id="1cc26-140">The following example shows how to call this API.</span></span>

##### <a name="request"></a><span data-ttu-id="1cc26-141">要求</span><span class="sxs-lookup"><span data-stu-id="1cc26-141">Request</span></span>
<span data-ttu-id="1cc26-142">次の例は要求を示しています。</span><span class="sxs-lookup"><span data-stu-id="1cc26-142">The following example shows the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "call-transfer"
}-->
```http
POST https://graph.microsoft.com/beta/app/calls/{id}/transfer
Content-Type: application/json
Content-Length: 430

{
  "transferTarget": {
    "endpointType": "default",
    "identity": {
      "user": {
        "id": "550fae72-d251-43ec-868c-373732c2704f",
        "tenantId": "72f988bf-86f1-41af-91ab-2d7cd011db47",
        "displayName": "Heidi Steen"
      }
    },
    "languageId": "languageId-value",
    "region": "region-value",
    "replacesCallId": "replacesCallId-value"
  },
  "clientContext": "clientContext-value"
}
```

##### <a name="response"></a><span data-ttu-id="1cc26-143">応答</span><span class="sxs-lookup"><span data-stu-id="1cc26-143">Response</span></span>

> <span data-ttu-id="1cc26-p104">**注:** 読みやすくするために、ここに示す応答オブジェクトは短くされている場合があります。実際の呼び出しからは、すべてのプロパティが返されます。</span><span class="sxs-lookup"><span data-stu-id="1cc26-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.None"
}-->
```http
HTTP/1.1 202 Accepted
```

##### <a name="notification---transferring"></a><span data-ttu-id="1cc26-146">通知を転送します。</span><span class="sxs-lookup"><span data-stu-id="1cc26-146">Notification - transferring</span></span>

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
      "resource": "/app/calls/57DAB8B1894C409AB240BD8BEAE78896/operations/0FE0623FD62842EDB4BD8AC290072CC5",
      "resourceData": {
        "@odata.type": "#microsoft.graph.commsOperation",
        "@odata.id": "/app/calls/57DAB8B1894C409AB240BD8BEAE78896/operations/0FE0623FD62842EDB4BD8AC290072CC5",
        "@odata.etag": "W/\"54451\"",
        "clientContext": "d45324c1-fcb5-430a-902c-f20af696537c",
        "resultInfo": {
          "code": "200",
          "subCode": "transferring"
        },
        "status": "running"
      }
    }
  ]
}
```

##### <a name="notification---transfer-accepted"></a><span data-ttu-id="1cc26-147">通知の転送を許可</span><span class="sxs-lookup"><span data-stu-id="1cc26-147">Notification - transfer accepted</span></span>

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
      "resource": "/app/calls/57DAB8B1894C409AB240BD8BEAE78896/operations/0FE0623FD62842EDB4BD8AC290072CC5",
      "resourceData": {
        "@odata.type": "#microsoft.graph.commsOperation",
        "@odata.id": "/app/calls/57DAB8B1894C409AB240BD8BEAE78896/operations/0FE0623FD62842EDB4BD8AC290072CC5",
        "@odata.etag": "W/\"54451\"",
        "clientContext": "d45324c1-fcb5-430a-902c-f20af696537c",
        "resultInfo": {
          "code": "200",
          "subCode": "transferAccepted"
        },
        "status": "completed"
      }
    }
  ]
}
```

##### <a name="notification---terminated"></a><span data-ttu-id="1cc26-148">終了の通知-</span><span class="sxs-lookup"><span data-stu-id="1cc26-148">Notification - terminated</span></span>

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
        "terminationReason": "AppTransferred"
      }
    }
  ]
}
```

### <a name="consultative-transfer"></a><span data-ttu-id="1cc26-149">提案型の転送</span><span class="sxs-lookup"><span data-stu-id="1cc26-149">Consultative transfer</span></span>

##### <a name="request"></a><span data-ttu-id="1cc26-150">要求</span><span class="sxs-lookup"><span data-stu-id="1cc26-150">Request</span></span>

```http
POST /app/calls/57DAB8B1894C409AB240BD8BEAE78896/transfer
Authorization: Bearer <TOKEN>
Content-Type: application/json
```
<!-- {
  "blockType": "ignored",
  "@odata.type": "call-transfer"
}-->
```json
{
  "clientContext": "d45324c1-fcb5-430a-902c-f20af696537c",
  "transferTarget": {
    "endpointType": "default",
    "identity": {
      "user": {
        "id": "550fae72-d251-43ec-868c-373732c2704f",
        "tenantId": "72f988bf-86f1-41af-91ab-2d7cd011db47",
        "displayName": "Heidi Steen"
      }
    },
    "languageId": "en-US",
    "region": "westus",
    "replacesCallId": "e5d39592-99bd-4db8-bca8-30fb894ec51d"
  }
}
```

##### <a name="response"></a><span data-ttu-id="1cc26-151">応答</span><span class="sxs-lookup"><span data-stu-id="1cc26-151">Response</span></span>

> <span data-ttu-id="1cc26-p105">**注:** 読みやすくするために、ここに示す応答オブジェクトは短くされている場合があります。実際の呼び出しからは、すべてのプロパティが返されます。</span><span class="sxs-lookup"><span data-stu-id="1cc26-p105">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

```http
HTTP/1.1 202 Accepted
```

##### <a name="notification---transferring"></a><span data-ttu-id="1cc26-154">通知を転送します。</span><span class="sxs-lookup"><span data-stu-id="1cc26-154">Notification - transferring</span></span>

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
      "resource": "/app/calls/57DAB8B1894C409AB240BD8BEAE78896/operations/0FE0623FD62842EDB4BD8AC290072CC5",
      "resourceData": {
        "@odata.type": "#microsoft.graph.commsOperation",
        "@odata.id": "/app/calls/57DAB8B1894C409AB240BD8BEAE78896/operations/0FE0623FD62842EDB4BD8AC290072CC5",
        "@odata.etag": "W/\"54451\"",
        "clientContext": "d45324c1-fcb5-430a-902c-f20af696537c",
        "resultInfo": {
          "code": "200",
          "subCode": "transferring"
        },
        "status": "running"
      }
    }
  ]
}
```

##### <a name="notification---transfer-accepted"></a><span data-ttu-id="1cc26-155">通知の転送を許可</span><span class="sxs-lookup"><span data-stu-id="1cc26-155">Notification - transfer accepted</span></span>

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
      "resource": "/app/calls/57DAB8B1894C409AB240BD8BEAE78896/operations/0FE0623FD62842EDB4BD8AC290072CC5",
      "resourceData": {
        "@odata.type": "#microsoft.graph.commsOperation",
        "@odata.id": "/app/calls/57DAB8B1894C409AB240BD8BEAE78896/operations/0FE0623FD62842EDB4BD8AC290072CC5",
        "@odata.etag": "W/\"54451\"",
        "clientContext": "d45324c1-fcb5-430a-902c-f20af696537c",
        "resultInfo": {
          "code": "200",
          "subCode": "transferAccepted"
        },
        "status": "completed"
      }
    }
  ]
}
```

##### <a name="notification---terminated"></a><span data-ttu-id="1cc26-156">終了の通知-</span><span class="sxs-lookup"><span data-stu-id="1cc26-156">Notification - terminated</span></span>

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
        "terminationReason": "AppTransferred"
      }
    }
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "call: transfer",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->