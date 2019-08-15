---
title: 通話の削除
description: アクティブな通話を削除または切断します。
author: VinodRavichandran
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: cfc0578261d4821bd4992b3a066c83194e40d1f1
ms.sourcegitcommit: 1066aa4045d48f9c9b764d3b2891cf4f806d17d5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/15/2019
ms.locfileid: "36418986"
---
# <a name="delete-call"></a><span data-ttu-id="60a7a-103">通話の削除</span><span class="sxs-lookup"><span data-stu-id="60a7a-103">Delete call</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="60a7a-104">アクティブな通話を削除または切断します。</span><span class="sxs-lookup"><span data-stu-id="60a7a-104">Delete or hang up an active call.</span></span>

## <a name="permissions"></a><span data-ttu-id="60a7a-105">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="60a7a-105">Permissions</span></span>

<span data-ttu-id="60a7a-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="60a7a-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="60a7a-108">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="60a7a-108">Permission type</span></span> | <span data-ttu-id="60a7a-109">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="60a7a-109">Permissions (from least to most privileged)</span></span>                  |
| :-------------- | :----------------------------------------------------------- |
| <span data-ttu-id="60a7a-110">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="60a7a-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="60a7a-111">サポートされません。</span><span class="sxs-lookup"><span data-stu-id="60a7a-111">Not Supported.</span></span>                         |
| <span data-ttu-id="60a7a-112">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="60a7a-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="60a7a-113">サポートされません。</span><span class="sxs-lookup"><span data-stu-id="60a7a-113">Not Supported.</span></span>                         |
| <span data-ttu-id="60a7a-114">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="60a7a-114">Application</span></span>                            | <span data-ttu-id="60a7a-115">なし。</span><span class="sxs-lookup"><span data-stu-id="60a7a-115">None.</span></span>                                  |

## <a name="http-request"></a><span data-ttu-id="60a7a-116">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="60a7a-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /app/calls/{id}
DELETE /applications/{id}/calls/{id}
```

## <a name="request-headers"></a><span data-ttu-id="60a7a-117">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="60a7a-117">Request headers</span></span>
| <span data-ttu-id="60a7a-118">名前</span><span class="sxs-lookup"><span data-stu-id="60a7a-118">Name</span></span>          | <span data-ttu-id="60a7a-119">説明</span><span class="sxs-lookup"><span data-stu-id="60a7a-119">Description</span></span>               |
|:--------------|:--------------------------|
| <span data-ttu-id="60a7a-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="60a7a-120">Authorization</span></span> | <span data-ttu-id="60a7a-p102">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="60a7a-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="60a7a-123">要求本文</span><span class="sxs-lookup"><span data-stu-id="60a7a-123">Request body</span></span>
<span data-ttu-id="60a7a-124">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="60a7a-124">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="60a7a-125">応答</span><span class="sxs-lookup"><span data-stu-id="60a7a-125">Response</span></span>
<span data-ttu-id="60a7a-p103">成功した場合、このメソッドは `204 No Content` 応答コードを返します。応答本文には何も返されません。</span><span class="sxs-lookup"><span data-stu-id="60a7a-p103">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="60a7a-128">例</span><span class="sxs-lookup"><span data-stu-id="60a7a-128">Example</span></span>

##### <a name="request"></a><span data-ttu-id="60a7a-129">要求</span><span class="sxs-lookup"><span data-stu-id="60a7a-129">Request</span></span>
<span data-ttu-id="60a7a-130">次の例は要求を示しています。</span><span class="sxs-lookup"><span data-stu-id="60a7a-130">The following example shows the request.</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="60a7a-131">プロトコル</span><span class="sxs-lookup"><span data-stu-id="60a7a-131">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete-call"
}-->
```http
DELETE https://graph.microsoft.com/beta/app/calls/{id}
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="60a7a-132">C#</span><span class="sxs-lookup"><span data-stu-id="60a7a-132">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-call-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="60a7a-133">JavaScript</span><span class="sxs-lookup"><span data-stu-id="60a7a-133">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-call-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="60a7a-134">目的-C</span><span class="sxs-lookup"><span data-stu-id="60a7a-134">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-call-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="60a7a-135">応答</span><span class="sxs-lookup"><span data-stu-id="60a7a-135">Response</span></span>

> <span data-ttu-id="60a7a-p104">**注:** 読みやすくするために、ここに示す応答オブジェクトは短縮されている場合があります。実際の呼び出しからは、すべてのプロパティが返されます。</span><span class="sxs-lookup"><span data-stu-id="60a7a-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 204 No Content
```

##### <a name="notification---terminating"></a><span data-ttu-id="60a7a-138">通知-終了</span><span class="sxs-lookup"><span data-stu-id="60a7a-138">Notification - terminating</span></span>

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
        "state": "terminating"
      }
    }
  ]
}
```

##### <a name="notification---terminated"></a><span data-ttu-id="60a7a-139">通知の終了</span><span class="sxs-lookup"><span data-stu-id="60a7a-139">Notification - terminated</span></span>

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
        "terminationReason": "AppInitiated"
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
  "description": "Delete call",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
