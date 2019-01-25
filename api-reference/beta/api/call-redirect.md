---
title: '呼び出す: リダイレクト'
description: 着信呼び出しをリダイレクトします。
author: VinodRavichandran
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: a6a926aa082cc35896d11ec4124091b0d2c838c0
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/24/2019
ms.locfileid: "29511990"
---
# <a name="call-redirect"></a><span data-ttu-id="d603d-103">呼び出す: リダイレクト</span><span class="sxs-lookup"><span data-stu-id="d603d-103">call: redirect</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="d603d-104">着信呼び出しをリダイレクトします。</span><span class="sxs-lookup"><span data-stu-id="d603d-104">Redirect an incoming call.</span></span>

## <a name="permissions"></a><span data-ttu-id="d603d-105">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="d603d-105">Permissions</span></span>
<span data-ttu-id="d603d-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="d603d-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="d603d-108">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="d603d-108">Permission type</span></span> | <span data-ttu-id="d603d-109">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="d603d-109">Permissions (from least to most privileged)</span></span>         |
| :-------------- | :-------------------------------------------------- |
| <span data-ttu-id="d603d-110">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="d603d-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="d603d-111">サポート対象外</span><span class="sxs-lookup"><span data-stu-id="d603d-111">Not Supported</span></span>                |
| <span data-ttu-id="d603d-112">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="d603d-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="d603d-113">サポート対象外</span><span class="sxs-lookup"><span data-stu-id="d603d-113">Not Supported</span></span>                |
| <span data-ttu-id="d603d-114">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="d603d-114">Application</span></span>     | <span data-ttu-id="d603d-115">Calls.Initiate.All</span><span class="sxs-lookup"><span data-stu-id="d603d-115">Calls.Initiate.All</span></span>                                  |

## <a name="http-request"></a><span data-ttu-id="d603d-116">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="d603d-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /app/calls/{id}/redirect
POST /applications/{id}/calls/{id}/redirect
```

## <a name="request-headers"></a><span data-ttu-id="d603d-117">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="d603d-117">Request headers</span></span>
| <span data-ttu-id="d603d-118">名前</span><span class="sxs-lookup"><span data-stu-id="d603d-118">Name</span></span>          | <span data-ttu-id="d603d-119">説明</span><span class="sxs-lookup"><span data-stu-id="d603d-119">Description</span></span>               |
|:--------------|:--------------------------|
| <span data-ttu-id="d603d-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="d603d-120">Authorization</span></span> | <span data-ttu-id="d603d-p102">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="d603d-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="d603d-123">要求本文</span><span class="sxs-lookup"><span data-stu-id="d603d-123">Request body</span></span>
<span data-ttu-id="d603d-124">要求本文で、次のパラメーターを含む JSON オブジェクトを指定します。</span><span class="sxs-lookup"><span data-stu-id="d603d-124">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="d603d-125">パラメーター</span><span class="sxs-lookup"><span data-stu-id="d603d-125">Parameter</span></span>      | <span data-ttu-id="d603d-126">型</span><span class="sxs-lookup"><span data-stu-id="d603d-126">Type</span></span>    |<span data-ttu-id="d603d-127">説明</span><span class="sxs-lookup"><span data-stu-id="d603d-127">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="d603d-128">Targets</span><span class="sxs-lookup"><span data-stu-id="d603d-128">targets</span></span>|<span data-ttu-id="d603d-129">[invitationParticipantInfo](../resources/invitationparticipantinfo.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="d603d-129">[invitationParticipantInfo](../resources/invitationparticipantinfo.md) collection</span></span>|<span data-ttu-id="d603d-130">リダイレクト操作のターゲットの参加者です。</span><span class="sxs-lookup"><span data-stu-id="d603d-130">The target participants of the redirect operation.</span></span>|
|<span data-ttu-id="d603d-131">targetDisposition</span><span class="sxs-lookup"><span data-stu-id="d603d-131">targetDisposition</span></span>|<span data-ttu-id="d603d-132">String</span><span class="sxs-lookup"><span data-stu-id="d603d-132">String</span></span>|<span data-ttu-id="d603d-133">使用可能な値は次のとおりです。`default`</span><span class="sxs-lookup"><span data-stu-id="d603d-133">The possible value is: `default`</span></span>|
|<span data-ttu-id="d603d-134">timeout</span><span class="sxs-lookup"><span data-stu-id="d603d-134">timeout</span></span>|<span data-ttu-id="d603d-135">Int32</span><span class="sxs-lookup"><span data-stu-id="d603d-135">Int32</span></span>|<span data-ttu-id="d603d-136">リダイレクト処理を秒単位でタイムアウトします。</span><span class="sxs-lookup"><span data-stu-id="d603d-136">The timeout in seconds for the redirect operation.</span></span>|
|<span data-ttu-id="d603d-137">maskCallee</span><span class="sxs-lookup"><span data-stu-id="d603d-137">maskCallee</span></span>|<span data-ttu-id="d603d-138">ブール値</span><span class="sxs-lookup"><span data-stu-id="d603d-138">Boolean</span></span>|<span data-ttu-id="d603d-139">呼び出し先をマスクするかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="d603d-139">Indicates whether to mask the callee.</span></span>|
|<span data-ttu-id="d603d-140">maskCaller</span><span class="sxs-lookup"><span data-stu-id="d603d-140">maskCaller</span></span>|<span data-ttu-id="d603d-141">ブール値</span><span class="sxs-lookup"><span data-stu-id="d603d-141">Boolean</span></span>|<span data-ttu-id="d603d-142">呼び出し元をマスクするかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="d603d-142">Indicates whether to mask the caller.</span></span>|

## <a name="response"></a><span data-ttu-id="d603d-143">応答</span><span class="sxs-lookup"><span data-stu-id="d603d-143">Response</span></span>
<span data-ttu-id="d603d-144">応答コードを返します。</span><span class="sxs-lookup"><span data-stu-id="d603d-144">Returns `202 Accepted` response code</span></span>

## <a name="examples"></a><span data-ttu-id="d603d-145">例</span><span class="sxs-lookup"><span data-stu-id="d603d-145">Examples</span></span>

### <a name="redirect-a-call"></a><span data-ttu-id="d603d-146">呼び出しをリダイレクトします。</span><span class="sxs-lookup"><span data-stu-id="d603d-146">Redirect a call</span></span>

##### <a name="request"></a><span data-ttu-id="d603d-147">要求</span><span class="sxs-lookup"><span data-stu-id="d603d-147">Request</span></span>
<span data-ttu-id="d603d-148">次の例は要求を示しています。</span><span class="sxs-lookup"><span data-stu-id="d603d-148">The following example shows the request.</span></span>

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

##### <a name="response"></a><span data-ttu-id="d603d-149">応答</span><span class="sxs-lookup"><span data-stu-id="d603d-149">Response</span></span>

> <span data-ttu-id="d603d-p103">**注:** 読みやすくするために、ここに示す応答オブジェクトは短くされている場合があります。実際の呼び出しからは、すべてのプロパティが返されます。</span><span class="sxs-lookup"><span data-stu-id="d603d-p103">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.None"
} -->
```http
HTTP/1.1 202 Accepted
```

### <a name="forward-a-call"></a><span data-ttu-id="d603d-152">呼び出しを転送します。</span><span class="sxs-lookup"><span data-stu-id="d603d-152">Forward a call</span></span>

##### <a name="notification---incoming"></a><span data-ttu-id="d603d-153">通知の受信</span><span class="sxs-lookup"><span data-stu-id="d603d-153">Notification - incoming</span></span>

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

##### <a name="request"></a><span data-ttu-id="d603d-154">要求</span><span class="sxs-lookup"><span data-stu-id="d603d-154">Request</span></span>

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

##### <a name="response"></a><span data-ttu-id="d603d-155">応答</span><span class="sxs-lookup"><span data-stu-id="d603d-155">Response</span></span>

```http
HTTP/1.1 202 Accepted
```

##### <a name="notification---redirecting"></a><span data-ttu-id="d603d-156">通知のリダイレクト</span><span class="sxs-lookup"><span data-stu-id="d603d-156">Notification - redirecting</span></span>

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

##### <a name="notification---terminated"></a><span data-ttu-id="d603d-157">終了の通知-</span><span class="sxs-lookup"><span data-stu-id="d603d-157">Notification - terminated</span></span>

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
    "Error: /api-reference/beta/api/call-redirect.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
