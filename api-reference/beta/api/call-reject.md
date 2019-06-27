---
title: '通話: 拒否'
description: 着信を拒否します。
author: VinodRavichandran
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: 718cb80f6b60e3e664c0a209fa91eb74a34691d7
ms.sourcegitcommit: 0e1101d499f35b08aa2309e273871438b1774979
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/27/2019
ms.locfileid: "35262217"
---
# <a name="call-reject"></a><span data-ttu-id="edea3-103">通話: 拒否</span><span class="sxs-lookup"><span data-stu-id="edea3-103">call: reject</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="edea3-104">着信を拒否します。</span><span class="sxs-lookup"><span data-stu-id="edea3-104">Reject an incoming call.</span></span>

## <a name="permissions"></a><span data-ttu-id="edea3-105">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="edea3-105">Permissions</span></span>
<span data-ttu-id="edea3-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="edea3-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="edea3-108">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="edea3-108">Permission type</span></span> | <span data-ttu-id="edea3-109">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="edea3-109">Permissions (from least to most privileged)</span></span>                |
| :-------------- | :--------------------------------------------------------- |
| <span data-ttu-id="edea3-110">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="edea3-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="edea3-111">サポート対象外</span><span class="sxs-lookup"><span data-stu-id="edea3-111">Not Supported</span></span>                       |
| <span data-ttu-id="edea3-112">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="edea3-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="edea3-113">サポート対象外</span><span class="sxs-lookup"><span data-stu-id="edea3-113">Not Supported</span></span>                       |
| <span data-ttu-id="edea3-114">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="edea3-114">Application</span></span>     | <span data-ttu-id="edea3-115">None</span><span class="sxs-lookup"><span data-stu-id="edea3-115">None</span></span>                                                       |

## <a name="http-request"></a><span data-ttu-id="edea3-116">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="edea3-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /app/calls/{id}/reject
POST /applications/{id}/calls/{id}/reject
```

## <a name="request-headers"></a><span data-ttu-id="edea3-117">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="edea3-117">Request headers</span></span>
| <span data-ttu-id="edea3-118">名前</span><span class="sxs-lookup"><span data-stu-id="edea3-118">Name</span></span>          | <span data-ttu-id="edea3-119">説明</span><span class="sxs-lookup"><span data-stu-id="edea3-119">Description</span></span>               |
|:--------------|:--------------------------|
| <span data-ttu-id="edea3-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="edea3-120">Authorization</span></span> | <span data-ttu-id="edea3-p102">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="edea3-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="edea3-123">要求本文</span><span class="sxs-lookup"><span data-stu-id="edea3-123">Request body</span></span>
<span data-ttu-id="edea3-124">要求本文で、次のパラメーターを含む JSON オブジェクトを指定します。</span><span class="sxs-lookup"><span data-stu-id="edea3-124">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="edea3-125">パラメーター</span><span class="sxs-lookup"><span data-stu-id="edea3-125">Parameter</span></span>      | <span data-ttu-id="edea3-126">型</span><span class="sxs-lookup"><span data-stu-id="edea3-126">Type</span></span>    |<span data-ttu-id="edea3-127">説明</span><span class="sxs-lookup"><span data-stu-id="edea3-127">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="edea3-128">したがっ</span><span class="sxs-lookup"><span data-stu-id="edea3-128">reason</span></span>|<span data-ttu-id="edea3-129">String</span><span class="sxs-lookup"><span data-stu-id="edea3-129">String</span></span>|<span data-ttu-id="edea3-130">拒否理由。</span><span class="sxs-lookup"><span data-stu-id="edea3-130">The rejection reason.</span></span>|

## <a name="response"></a><span data-ttu-id="edea3-131">応答</span><span class="sxs-lookup"><span data-stu-id="edea3-131">Response</span></span>
<span data-ttu-id="edea3-p103">成功した場合、このメソッドは `200 OK` 応答コードを返します。応答本文には何も返されません。</span><span class="sxs-lookup"><span data-stu-id="edea3-p103">If successful, this method returns `200 OK` response code. It does not return anything in the response body.</span></span>

```http
Returns `202 Accepted` response code
```

## <a name="example"></a><span data-ttu-id="edea3-134">例</span><span class="sxs-lookup"><span data-stu-id="edea3-134">Example</span></span>
<span data-ttu-id="edea3-135">次の例は、この API を呼び出す方法を示しています。</span><span class="sxs-lookup"><span data-stu-id="edea3-135">The following example shows how to call this API.</span></span>

##### <a name="notification---incoming"></a><span data-ttu-id="edea3-136">通知-受信</span><span class="sxs-lookup"><span data-stu-id="edea3-136">Notification - incoming</span></span>

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

##### <a name="request"></a><span data-ttu-id="edea3-137">要求</span><span class="sxs-lookup"><span data-stu-id="edea3-137">Request</span></span>
<span data-ttu-id="edea3-138">次の例は要求を示しています。</span><span class="sxs-lookup"><span data-stu-id="edea3-138">The following example shows the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "call-reject"
}-->
```http
POST https://graph.microsoft.com/beta/app/calls/{id}/reject
Content-Type: application/json
Content-Length: 24

{
  "reason": "none"
}
```

##### <a name="response"></a><span data-ttu-id="edea3-139">応答</span><span class="sxs-lookup"><span data-stu-id="edea3-139">Response</span></span>
<span data-ttu-id="edea3-140">以下は、応答の例です。</span><span class="sxs-lookup"><span data-stu-id="edea3-140">Here is an example of the response.</span></span> 

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.None"
} -->
```http
HTTP/1.1 202 Accepted
```
#### <a name="sdk-sample-code"></a><span data-ttu-id="edea3-141">SDK サンプル コード</span><span class="sxs-lookup"><span data-stu-id="edea3-141">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="edea3-142">C#</span><span class="sxs-lookup"><span data-stu-id="edea3-142">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/call-reject-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="edea3-143">Javascript</span><span class="sxs-lookup"><span data-stu-id="edea3-143">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/call-reject-Javascript-snippets.md)]

# <a name="objective-ctabobjective-c"></a>[<span data-ttu-id="edea3-144">目的-C</span><span class="sxs-lookup"><span data-stu-id="edea3-144">Objective-C</span></span>](#tab/objective-c)
[!INCLUDE [sample-code](../includes/call-reject-Objective-C-snippets.md)]
---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

##### <a name="notification---deleted"></a><span data-ttu-id="edea3-145">通知-削除済み</span><span class="sxs-lookup"><span data-stu-id="edea3-145">Notification - deleted</span></span>

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
<!--
{
  "type": "#page.annotation",
  "description": "call: reject",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/call-reject.md:\r\n      BookmarkMissing: '[#tab/objective-c](Objective-C)'. Did you mean: #objective-c (score: 4)",
    "Error: /api-reference/beta/api/call-reject.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/beta/api/call-reject.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}
-->
