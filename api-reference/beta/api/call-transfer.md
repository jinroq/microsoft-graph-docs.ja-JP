---
title: '通話: 転送'
description: アクティブな通話を転送します。
author: VinodRavichandran
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: fcee0aa486d2650c8842141b29641ed3d3a73be2
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/25/2019
ms.locfileid: "35864617"
---
# <a name="call-transfer"></a><span data-ttu-id="c3fca-103">通話: 転送</span><span class="sxs-lookup"><span data-stu-id="c3fca-103">call: transfer</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="c3fca-104">アクティブな通話を転送します。</span><span class="sxs-lookup"><span data-stu-id="c3fca-104">Transfer an active call.</span></span>

## <a name="permissions"></a><span data-ttu-id="c3fca-105">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="c3fca-105">Permissions</span></span>
<span data-ttu-id="c3fca-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="c3fca-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="c3fca-108">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="c3fca-108">Permission type</span></span> | <span data-ttu-id="c3fca-109">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="c3fca-109">Permissions (from least to most privileged)</span></span>         |
| :-------------- | :-------------------------------------------------- |
| <span data-ttu-id="c3fca-110">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="c3fca-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="c3fca-111">サポート対象外</span><span class="sxs-lookup"><span data-stu-id="c3fca-111">Not Supported</span></span>                |
| <span data-ttu-id="c3fca-112">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="c3fca-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="c3fca-113">サポート対象外</span><span class="sxs-lookup"><span data-stu-id="c3fca-113">Not Supported</span></span>                |
| <span data-ttu-id="c3fca-114">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="c3fca-114">Application</span></span>     | <span data-ttu-id="c3fca-115">Calls.Initiate.All</span><span class="sxs-lookup"><span data-stu-id="c3fca-115">Calls.Initiate.All</span></span>                                  |

## <a name="http-request"></a><span data-ttu-id="c3fca-116">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="c3fca-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /app/calls/{id}/transfer
POST /applications/{id}/calls/{id}/transfer
```

## <a name="request-headers"></a><span data-ttu-id="c3fca-117">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="c3fca-117">Request headers</span></span>
| <span data-ttu-id="c3fca-118">名前</span><span class="sxs-lookup"><span data-stu-id="c3fca-118">Name</span></span>          | <span data-ttu-id="c3fca-119">説明</span><span class="sxs-lookup"><span data-stu-id="c3fca-119">Description</span></span>               |
|:--------------|:--------------------------|
| <span data-ttu-id="c3fca-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="c3fca-120">Authorization</span></span> | <span data-ttu-id="c3fca-p102">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="c3fca-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="c3fca-123">要求本文</span><span class="sxs-lookup"><span data-stu-id="c3fca-123">Request body</span></span>
<span data-ttu-id="c3fca-124">要求本文で、次のパラメーターを含む JSON オブジェクトを指定します。</span><span class="sxs-lookup"><span data-stu-id="c3fca-124">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="c3fca-125">パラメーター</span><span class="sxs-lookup"><span data-stu-id="c3fca-125">Parameter</span></span>      | <span data-ttu-id="c3fca-126">型</span><span class="sxs-lookup"><span data-stu-id="c3fca-126">Type</span></span>    |<span data-ttu-id="c3fca-127">説明</span><span class="sxs-lookup"><span data-stu-id="c3fca-127">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="c3fca-128">transferTarget</span><span class="sxs-lookup"><span data-stu-id="c3fca-128">transferTarget</span></span>|[<span data-ttu-id="c3fca-129">invitationParticipantInfo</span><span class="sxs-lookup"><span data-stu-id="c3fca-129">invitationParticipantInfo</span></span>](../resources/invitationparticipantinfo.md)|<span data-ttu-id="c3fca-130">転送先の参加者です。</span><span class="sxs-lookup"><span data-stu-id="c3fca-130">The participant which is the target of the transfer.</span></span>|
|<span data-ttu-id="c3fca-131">clientContext</span><span class="sxs-lookup"><span data-stu-id="c3fca-131">clientContext</span></span>|<span data-ttu-id="c3fca-132">String</span><span class="sxs-lookup"><span data-stu-id="c3fca-132">String</span></span>|<span data-ttu-id="c3fca-133">クライアントコンテキスト。</span><span class="sxs-lookup"><span data-stu-id="c3fca-133">The client context.</span></span>|

## <a name="response"></a><span data-ttu-id="c3fca-134">応答</span><span class="sxs-lookup"><span data-stu-id="c3fca-134">Response</span></span>
<span data-ttu-id="c3fca-135">応答`202 Accepted`コードを返します。</span><span class="sxs-lookup"><span data-stu-id="c3fca-135">Returns `202 Accepted` response code.</span></span>

## <a name="examples"></a><span data-ttu-id="c3fca-136">例</span><span class="sxs-lookup"><span data-stu-id="c3fca-136">Examples</span></span>

### <a name="transfer-call-directly-with-no-user-involvement"></a><span data-ttu-id="c3fca-137">ユーザーが関与せずに直接通話を転送する</span><span class="sxs-lookup"><span data-stu-id="c3fca-137">Transfer call directly, with no user involvement</span></span>

<span data-ttu-id="c3fca-138">次の例は、この API を呼び出す方法を示しています。</span><span class="sxs-lookup"><span data-stu-id="c3fca-138">The following example shows how to call this API.</span></span>

##### <a name="request"></a><span data-ttu-id="c3fca-139">要求</span><span class="sxs-lookup"><span data-stu-id="c3fca-139">Request</span></span>
<span data-ttu-id="c3fca-140">次の例は要求を示しています。</span><span class="sxs-lookup"><span data-stu-id="c3fca-140">The following example shows the request.</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="c3fca-141">プロトコル</span><span class="sxs-lookup"><span data-stu-id="c3fca-141">HTTP</span></span>](#tab/http)
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
# <a name="ctabcsharp"></a>[<span data-ttu-id="c3fca-142">C#</span><span class="sxs-lookup"><span data-stu-id="c3fca-142">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/call-transfer-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="c3fca-143">Javascript</span><span class="sxs-lookup"><span data-stu-id="c3fca-143">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/call-transfer-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="c3fca-144">目的-C</span><span class="sxs-lookup"><span data-stu-id="c3fca-144">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/call-transfer-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="c3fca-145">Java</span><span class="sxs-lookup"><span data-stu-id="c3fca-145">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/call-transfer-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="c3fca-146">応答</span><span class="sxs-lookup"><span data-stu-id="c3fca-146">Response</span></span>

> <span data-ttu-id="c3fca-p103">**注:** 読みやすくするために、ここに示す応答オブジェクトは短縮されている場合があります。実際の呼び出しからは、すべてのプロパティが返されます。</span><span class="sxs-lookup"><span data-stu-id="c3fca-p103">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.None"
}-->
```http
HTTP/1.1 202 Accepted
```

##### <a name="notification---transferring"></a><span data-ttu-id="c3fca-149">通知-転送</span><span class="sxs-lookup"><span data-stu-id="c3fca-149">Notification - transferring</span></span>

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

##### <a name="notification---transfer-accepted"></a><span data-ttu-id="c3fca-150">通知-転送が承認されました</span><span class="sxs-lookup"><span data-stu-id="c3fca-150">Notification - transfer accepted</span></span>

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

##### <a name="notification---terminated"></a><span data-ttu-id="c3fca-151">通知の終了</span><span class="sxs-lookup"><span data-stu-id="c3fca-151">Notification - terminated</span></span>

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

### <a name="consultative-transfer"></a><span data-ttu-id="c3fca-152">提案転送</span><span class="sxs-lookup"><span data-stu-id="c3fca-152">Consultative transfer</span></span>

##### <a name="request"></a><span data-ttu-id="c3fca-153">要求</span><span class="sxs-lookup"><span data-stu-id="c3fca-153">Request</span></span>

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

##### <a name="response"></a><span data-ttu-id="c3fca-154">応答</span><span class="sxs-lookup"><span data-stu-id="c3fca-154">Response</span></span>

> <span data-ttu-id="c3fca-p104">**注:** 読みやすくするために、ここに示す応答オブジェクトは短縮されている場合があります。実際の呼び出しからは、すべてのプロパティが返されます。</span><span class="sxs-lookup"><span data-stu-id="c3fca-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

```http
HTTP/1.1 202 Accepted
```

##### <a name="notification---transferring"></a><span data-ttu-id="c3fca-157">通知-転送</span><span class="sxs-lookup"><span data-stu-id="c3fca-157">Notification - transferring</span></span>

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

##### <a name="notification---transfer-accepted"></a><span data-ttu-id="c3fca-158">通知-転送が承認されました</span><span class="sxs-lookup"><span data-stu-id="c3fca-158">Notification - transfer accepted</span></span>

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

##### <a name="notification---terminated"></a><span data-ttu-id="c3fca-159">通知の終了</span><span class="sxs-lookup"><span data-stu-id="c3fca-159">Notification - terminated</span></span>

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
  ]
}
-->
