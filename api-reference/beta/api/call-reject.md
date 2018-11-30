---
title: '呼び出す: 元に戻す'
description: 着信呼び出しを拒否します。
ms.openlocfilehash: 4731d377021871569fcec895af832aeea66b3431
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27070259"
---
# <a name="call-reject"></a><span data-ttu-id="120f6-103">呼び出す: 元に戻す</span><span class="sxs-lookup"><span data-stu-id="120f6-103">call: reject</span></span>

> <span data-ttu-id="120f6-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="120f6-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="120f6-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="120f6-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="120f6-106">着信呼び出しを拒否します。</span><span class="sxs-lookup"><span data-stu-id="120f6-106">Reject an incoming call.</span></span>

## <a name="permissions"></a><span data-ttu-id="120f6-107">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="120f6-107">Permissions</span></span>
<span data-ttu-id="120f6-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="120f6-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="120f6-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="120f6-110">Permission type</span></span> | <span data-ttu-id="120f6-111">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="120f6-111">Permissions (from least to most privileged)</span></span>                |
| :-------------- | :--------------------------------------------------------- |
| <span data-ttu-id="120f6-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="120f6-112">Delegated (work or school account)</span></span>     | <span data-ttu-id="120f6-113">サポート対象外</span><span class="sxs-lookup"><span data-stu-id="120f6-113">Not Supported</span></span>                       |
| <span data-ttu-id="120f6-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="120f6-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="120f6-115">サポート対象外</span><span class="sxs-lookup"><span data-stu-id="120f6-115">Not Supported</span></span>                       |
| <span data-ttu-id="120f6-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="120f6-116">Application</span></span>     | <span data-ttu-id="120f6-117">なし</span><span class="sxs-lookup"><span data-stu-id="120f6-117">None</span></span>                                                       |

## <a name="http-request"></a><span data-ttu-id="120f6-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="120f6-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /app/calls/{id}/reject
POST /applications/{id}/calls/{id}/reject
```

## <a name="request-headers"></a><span data-ttu-id="120f6-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="120f6-119">Request headers</span></span>
| <span data-ttu-id="120f6-120">名前</span><span class="sxs-lookup"><span data-stu-id="120f6-120">Name</span></span>          | <span data-ttu-id="120f6-121">説明</span><span class="sxs-lookup"><span data-stu-id="120f6-121">Description</span></span>               |
|:--------------|:--------------------------|
| <span data-ttu-id="120f6-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="120f6-122">Authorization</span></span> | <span data-ttu-id="120f6-p103">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="120f6-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="120f6-125">要求本文</span><span class="sxs-lookup"><span data-stu-id="120f6-125">Request body</span></span>
<span data-ttu-id="120f6-126">要求本文で、次のパラメーターを含む JSON オブジェクトを指定します。</span><span class="sxs-lookup"><span data-stu-id="120f6-126">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="120f6-127">パラメーター</span><span class="sxs-lookup"><span data-stu-id="120f6-127">Parameter</span></span>      | <span data-ttu-id="120f6-128">型</span><span class="sxs-lookup"><span data-stu-id="120f6-128">Type</span></span>    |<span data-ttu-id="120f6-129">説明</span><span class="sxs-lookup"><span data-stu-id="120f6-129">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="120f6-130">理由</span><span class="sxs-lookup"><span data-stu-id="120f6-130">reason</span></span>|<span data-ttu-id="120f6-131">String</span><span class="sxs-lookup"><span data-stu-id="120f6-131">String</span></span>|<span data-ttu-id="120f6-132">却下の理由です。</span><span class="sxs-lookup"><span data-stu-id="120f6-132">The rejection reason.</span></span>|

## <a name="response"></a><span data-ttu-id="120f6-133">応答</span><span class="sxs-lookup"><span data-stu-id="120f6-133">Response</span></span>
<span data-ttu-id="120f6-p104">成功した場合、このメソッドは `200 OK` 応答コードを返します。応答本文には何も返されません。</span><span class="sxs-lookup"><span data-stu-id="120f6-p104">If successful, this method returns `200 OK` response code. It does not return anything in the response body.</span></span>

```http
Returns `202 Accepted` response code
```

## <a name="example"></a><span data-ttu-id="120f6-136">例</span><span class="sxs-lookup"><span data-stu-id="120f6-136">Example</span></span>
<span data-ttu-id="120f6-137">次の例は、この API を呼び出す方法を示しています。</span><span class="sxs-lookup"><span data-stu-id="120f6-137">The following example shows how to call this API.</span></span>

##### <a name="notification---incoming"></a><span data-ttu-id="120f6-138">通知の受信</span><span class="sxs-lookup"><span data-stu-id="120f6-138">Notification - incoming</span></span>

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

##### <a name="request"></a><span data-ttu-id="120f6-139">要求</span><span class="sxs-lookup"><span data-stu-id="120f6-139">Request</span></span>
<span data-ttu-id="120f6-140">次の例は要求を示しています。</span><span class="sxs-lookup"><span data-stu-id="120f6-140">The following example shows the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "call_reject"
}-->
```http
POST https://graph.microsoft.com/beta/app/calls/{id}/reject
Content-Type: application/json
Content-Length: 24

{
  "reason": "none"
}
```

##### <a name="response"></a><span data-ttu-id="120f6-141">応答</span><span class="sxs-lookup"><span data-stu-id="120f6-141">Response</span></span>
<span data-ttu-id="120f6-142">以下は、応答の例です。</span><span class="sxs-lookup"><span data-stu-id="120f6-142">Here is an example of the response.</span></span> 

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.None"
} -->
```http
HTTP/1.1 202 Accepted
```

##### <a name="notification---deleted"></a><span data-ttu-id="120f6-143">通知の削除</span><span class="sxs-lookup"><span data-stu-id="120f6-143">Notification - deleted</span></span>

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
        "@odata.etag": "W/\"5445\""
      }
    }
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "call: reject",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->