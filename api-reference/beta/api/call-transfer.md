---
title: '呼び出す: 転送'
description: アクティブな呼び出しを転送します。
author: VinodRavichandran
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: b1c503be31b17fb608abbec340aa9390ce315435
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/24/2019
ms.locfileid: "29516253"
---
# <a name="call-transfer"></a><span data-ttu-id="12f25-103">呼び出す: 転送</span><span class="sxs-lookup"><span data-stu-id="12f25-103">call: transfer</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="12f25-104">アクティブな呼び出しを転送します。</span><span class="sxs-lookup"><span data-stu-id="12f25-104">Transfer an active call.</span></span>

## <a name="permissions"></a><span data-ttu-id="12f25-105">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="12f25-105">Permissions</span></span>
<span data-ttu-id="12f25-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="12f25-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="12f25-108">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="12f25-108">Permission type</span></span> | <span data-ttu-id="12f25-109">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="12f25-109">Permissions (from least to most privileged)</span></span>         |
| :-------------- | :-------------------------------------------------- |
| <span data-ttu-id="12f25-110">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="12f25-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="12f25-111">サポート対象外</span><span class="sxs-lookup"><span data-stu-id="12f25-111">Not Supported</span></span>                |
| <span data-ttu-id="12f25-112">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="12f25-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="12f25-113">サポート対象外</span><span class="sxs-lookup"><span data-stu-id="12f25-113">Not Supported</span></span>                |
| <span data-ttu-id="12f25-114">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="12f25-114">Application</span></span>     | <span data-ttu-id="12f25-115">Calls.Initiate.All</span><span class="sxs-lookup"><span data-stu-id="12f25-115">Calls.Initiate.All</span></span>                                  |

## <a name="http-request"></a><span data-ttu-id="12f25-116">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="12f25-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /app/calls/{id}/transfer
POST /applications/{id}/calls/{id}/transfer
```

## <a name="request-headers"></a><span data-ttu-id="12f25-117">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="12f25-117">Request headers</span></span>
| <span data-ttu-id="12f25-118">名前</span><span class="sxs-lookup"><span data-stu-id="12f25-118">Name</span></span>          | <span data-ttu-id="12f25-119">説明</span><span class="sxs-lookup"><span data-stu-id="12f25-119">Description</span></span>               |
|:--------------|:--------------------------|
| <span data-ttu-id="12f25-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="12f25-120">Authorization</span></span> | <span data-ttu-id="12f25-p102">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="12f25-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="12f25-123">要求本文</span><span class="sxs-lookup"><span data-stu-id="12f25-123">Request body</span></span>
<span data-ttu-id="12f25-124">要求本文で、次のパラメーターを含む JSON オブジェクトを指定します。</span><span class="sxs-lookup"><span data-stu-id="12f25-124">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="12f25-125">パラメーター</span><span class="sxs-lookup"><span data-stu-id="12f25-125">Parameter</span></span>      | <span data-ttu-id="12f25-126">型</span><span class="sxs-lookup"><span data-stu-id="12f25-126">Type</span></span>    |<span data-ttu-id="12f25-127">説明</span><span class="sxs-lookup"><span data-stu-id="12f25-127">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="12f25-128">transferTarget</span><span class="sxs-lookup"><span data-stu-id="12f25-128">transferTarget</span></span>|[<span data-ttu-id="12f25-129">invitationParticipantInfo</span><span class="sxs-lookup"><span data-stu-id="12f25-129">invitationParticipantInfo</span></span>](../resources/invitationparticipantinfo.md)|<span data-ttu-id="12f25-130">転送の対象である構成要素です。</span><span class="sxs-lookup"><span data-stu-id="12f25-130">The participant which is the target of the transfer.</span></span>|
|<span data-ttu-id="12f25-131">ClientContext</span><span class="sxs-lookup"><span data-stu-id="12f25-131">clientContext</span></span>|<span data-ttu-id="12f25-132">String</span><span class="sxs-lookup"><span data-stu-id="12f25-132">String</span></span>|<span data-ttu-id="12f25-133">クライアントのコンテキスト。</span><span class="sxs-lookup"><span data-stu-id="12f25-133">The client context.</span></span>|

## <a name="response"></a><span data-ttu-id="12f25-134">応答</span><span class="sxs-lookup"><span data-stu-id="12f25-134">Response</span></span>
<span data-ttu-id="12f25-135">応答コードを返します。</span><span class="sxs-lookup"><span data-stu-id="12f25-135">Returns `202 Accepted` response code.</span></span>

## <a name="examples"></a><span data-ttu-id="12f25-136">例</span><span class="sxs-lookup"><span data-stu-id="12f25-136">Examples</span></span>

### <a name="transfer-call-directly-with-no-user-involvement"></a><span data-ttu-id="12f25-137">ユーザーの関与なしに直接、電話を転送します。</span><span class="sxs-lookup"><span data-stu-id="12f25-137">Transfer call directly, with no user involvement</span></span>

<span data-ttu-id="12f25-138">次の例は、この API を呼び出す方法を示しています。</span><span class="sxs-lookup"><span data-stu-id="12f25-138">The following example shows how to call this API.</span></span>

##### <a name="request"></a><span data-ttu-id="12f25-139">要求</span><span class="sxs-lookup"><span data-stu-id="12f25-139">Request</span></span>
<span data-ttu-id="12f25-140">次の例は要求を示しています。</span><span class="sxs-lookup"><span data-stu-id="12f25-140">The following example shows the request.</span></span>

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

##### <a name="response"></a><span data-ttu-id="12f25-141">応答</span><span class="sxs-lookup"><span data-stu-id="12f25-141">Response</span></span>

> <span data-ttu-id="12f25-p103">**注:** 読みやすくするために、ここに示す応答オブジェクトは短くされている場合があります。実際の呼び出しからは、すべてのプロパティが返されます。</span><span class="sxs-lookup"><span data-stu-id="12f25-p103">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.None"
}-->
```http
HTTP/1.1 202 Accepted
```

##### <a name="notification---transferring"></a><span data-ttu-id="12f25-144">通知を転送します。</span><span class="sxs-lookup"><span data-stu-id="12f25-144">Notification - transferring</span></span>

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

##### <a name="notification---transfer-accepted"></a><span data-ttu-id="12f25-145">通知の転送を許可</span><span class="sxs-lookup"><span data-stu-id="12f25-145">Notification - transfer accepted</span></span>

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

##### <a name="notification---terminated"></a><span data-ttu-id="12f25-146">終了の通知-</span><span class="sxs-lookup"><span data-stu-id="12f25-146">Notification - terminated</span></span>

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

### <a name="consultative-transfer"></a><span data-ttu-id="12f25-147">提案型の転送</span><span class="sxs-lookup"><span data-stu-id="12f25-147">Consultative transfer</span></span>

##### <a name="request"></a><span data-ttu-id="12f25-148">要求</span><span class="sxs-lookup"><span data-stu-id="12f25-148">Request</span></span>

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

##### <a name="response"></a><span data-ttu-id="12f25-149">応答</span><span class="sxs-lookup"><span data-stu-id="12f25-149">Response</span></span>

> <span data-ttu-id="12f25-p104">**注:** 読みやすくするために、ここに示す応答オブジェクトは短くされている場合があります。実際の呼び出しからは、すべてのプロパティが返されます。</span><span class="sxs-lookup"><span data-stu-id="12f25-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

```http
HTTP/1.1 202 Accepted
```

##### <a name="notification---transferring"></a><span data-ttu-id="12f25-152">通知を転送します。</span><span class="sxs-lookup"><span data-stu-id="12f25-152">Notification - transferring</span></span>

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

##### <a name="notification---transfer-accepted"></a><span data-ttu-id="12f25-153">通知の転送を許可</span><span class="sxs-lookup"><span data-stu-id="12f25-153">Notification - transfer accepted</span></span>

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

##### <a name="notification---terminated"></a><span data-ttu-id="12f25-154">終了の通知-</span><span class="sxs-lookup"><span data-stu-id="12f25-154">Notification - terminated</span></span>

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
<!--
{
  "type": "#page.annotation",
  "description": "call: transfer",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/call-transfer.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
