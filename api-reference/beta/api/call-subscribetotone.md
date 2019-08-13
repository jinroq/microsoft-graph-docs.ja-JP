---
title: '通話: subscribeToTone'
description: DTMF (デュアルトーンマルチ周波数信号) をサブスクライブします。 これにより、ユーザーが ' プッシュホン ' 電話でキーを押したときに通知を受けることができます。
author: VinodRavichandran
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: 2c7960d7e42f9845551cf3396bff9b00d43cc409
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/13/2019
ms.locfileid: "36317579"
---
# <a name="call-subscribetotone"></a><span data-ttu-id="65db4-104">通話: subscribeToTone</span><span class="sxs-lookup"><span data-stu-id="65db4-104">call: subscribeToTone</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="65db4-105">DTMF (デュアルトーンマルチ周波数信号) をサブスクライブします。</span><span class="sxs-lookup"><span data-stu-id="65db4-105">Subscribe to DTMF (dual-tone multi-frequency signaling).</span></span> <span data-ttu-id="65db4-106">これにより、ユーザーが "プッシュホン" 電話でキーを押したときに通知を受けることができます。</span><span class="sxs-lookup"><span data-stu-id="65db4-106">This allows you to be notified when the user presses keys on a "touchtone" phone.</span></span>

## <a name="permissions"></a><span data-ttu-id="65db4-107">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="65db4-107">Permissions</span></span>
<span data-ttu-id="65db4-p103">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="65db4-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="65db4-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="65db4-110">Permission type</span></span> | <span data-ttu-id="65db4-111">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="65db4-111">Permissions (from least to most privileged)</span></span> |
| :-------------- | :------------------------------------------ |
| <span data-ttu-id="65db4-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="65db4-112">Delegated (work or school account)</span></span>     | <span data-ttu-id="65db4-113">サポート対象外</span><span class="sxs-lookup"><span data-stu-id="65db4-113">Not Supported</span></span>        |
| <span data-ttu-id="65db4-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="65db4-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="65db4-115">サポート対象外</span><span class="sxs-lookup"><span data-stu-id="65db4-115">Not Supported</span></span>        |
| <span data-ttu-id="65db4-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="65db4-116">Application</span></span>     | <span data-ttu-id="65db4-117">Calls.AccessMedia.All</span><span class="sxs-lookup"><span data-stu-id="65db4-117">Calls.AccessMedia.All</span></span>                       |

## <a name="http-request"></a><span data-ttu-id="65db4-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="65db4-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /app/calls/{id}/subscribeToTone
POST /applications/{id}/calls/{id}/subscribeToTone
```

## <a name="request-headers"></a><span data-ttu-id="65db4-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="65db4-119">Request headers</span></span>
| <span data-ttu-id="65db4-120">名前</span><span class="sxs-lookup"><span data-stu-id="65db4-120">Name</span></span>          | <span data-ttu-id="65db4-121">説明</span><span class="sxs-lookup"><span data-stu-id="65db4-121">Description</span></span>               |
|:--------------|:--------------------------|
| <span data-ttu-id="65db4-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="65db4-122">Authorization</span></span> | <span data-ttu-id="65db4-p104">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="65db4-p104">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="65db4-125">要求本文</span><span class="sxs-lookup"><span data-stu-id="65db4-125">Request body</span></span>
<span data-ttu-id="65db4-126">要求本文で、次のパラメーターを含む JSON オブジェクトを指定します。</span><span class="sxs-lookup"><span data-stu-id="65db4-126">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="65db4-127">パラメーター</span><span class="sxs-lookup"><span data-stu-id="65db4-127">Parameter</span></span>      | <span data-ttu-id="65db4-128">型</span><span class="sxs-lookup"><span data-stu-id="65db4-128">Type</span></span>    | <span data-ttu-id="65db4-129">説明</span><span class="sxs-lookup"><span data-stu-id="65db4-129">Description</span></span> |
|:---------------|:--------|:------------|
| <span data-ttu-id="65db4-130">clientContext</span><span class="sxs-lookup"><span data-stu-id="65db4-130">clientContext</span></span>  | <span data-ttu-id="65db4-131">String</span><span class="sxs-lookup"><span data-stu-id="65db4-131">String</span></span>  | <span data-ttu-id="65db4-132">クライアントコンテキスト。</span><span class="sxs-lookup"><span data-stu-id="65db4-132">The client context.</span></span> |

## <a name="response"></a><span data-ttu-id="65db4-133">応答</span><span class="sxs-lookup"><span data-stu-id="65db4-133">Response</span></span>
<span data-ttu-id="65db4-134">この`202 Accepted`要求に対して作成された[commsOperation](../resources/commsoperation.md)への uri を持つ応答コードと位置ヘッダーを返します。</span><span class="sxs-lookup"><span data-stu-id="65db4-134">Returns `202 Accepted` response code and a Location header with a uri to the [commsOperation](../resources/commsoperation.md) created for this request.</span></span>

## <a name="example"></a><span data-ttu-id="65db4-135">例</span><span class="sxs-lookup"><span data-stu-id="65db4-135">Example</span></span>
<span data-ttu-id="65db4-136">次の例は、この API を呼び出す方法を示しています。</span><span class="sxs-lookup"><span data-stu-id="65db4-136">The following example shows how to call this API.</span></span>

##### <a name="request"></a><span data-ttu-id="65db4-137">要求</span><span class="sxs-lookup"><span data-stu-id="65db4-137">Request</span></span>
<span data-ttu-id="65db4-138">次の例は要求を示しています。</span><span class="sxs-lookup"><span data-stu-id="65db4-138">The following example shows the request.</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="65db4-139">プロトコル</span><span class="sxs-lookup"><span data-stu-id="65db4-139">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "call-subscribeToTone"
}-->
```http
POST https://graph.microsoft.com/beta/app/calls/{id}/subscribeToTone
Content-Type: application/json
Content-Length: 46

{
  "clientContext": "d45324c1-fcb5-430a-902c-f20af696537c"
}
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="65db4-140">C#</span><span class="sxs-lookup"><span data-stu-id="65db4-140">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/call-subscribetotone-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="65db4-141">JavaScript</span><span class="sxs-lookup"><span data-stu-id="65db4-141">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/call-subscribetotone-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="65db4-142">目的-C</span><span class="sxs-lookup"><span data-stu-id="65db4-142">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/call-subscribetotone-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="65db4-143">Java</span><span class="sxs-lookup"><span data-stu-id="65db4-143">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/call-subscribetotone-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="65db4-144">応答</span><span class="sxs-lookup"><span data-stu-id="65db4-144">Response</span></span>

> <span data-ttu-id="65db4-p105">**注:** 読みやすくするために、ここに示す応答オブジェクトは短縮されている場合があります。実際の呼び出しからは、すべてのプロパティが返されます。</span><span class="sxs-lookup"><span data-stu-id="65db4-p105">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.commsOperation"
} -->
```http
HTTP/1.1 202 Accepted
Location: https://graph.microsoft.com/beta/app/calls/57dab8b1-894c-409a-b240-bd8beae78896/operations/0fe0623f-d628-42ed-b4bd-8ac290072cc5
```

##### <a name="notification---operation-completed"></a><span data-ttu-id="65db4-147">通知-操作が完了しました</span><span class="sxs-lookup"><span data-stu-id="65db4-147">Notification - operation completed</span></span>

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
        "status": "completed"
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
  "description": "call: subscribeToTone",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
