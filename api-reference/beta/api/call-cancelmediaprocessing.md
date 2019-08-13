---
title: '通話: cancelMediaProcessing'
description: すべての進行中の再生プロンプトまたはレコード操作のメディア処理をキャンセルします。
author: VinodRavichandran
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: c2d9d552727452a1d1f417629cbae90dac76b84c
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/13/2019
ms.locfileid: "36317797"
---
# <a name="call-cancelmediaprocessing"></a><span data-ttu-id="cc2ea-103">通話: cancelMediaProcessing</span><span class="sxs-lookup"><span data-stu-id="cc2ea-103">call: cancelMediaProcessing</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="cc2ea-104">すべての進行中の再生プロンプトまたはレコード操作のメディア処理をキャンセルします。</span><span class="sxs-lookup"><span data-stu-id="cc2ea-104">Cancels media processing for all in-progress any PlayPrompt or Record operations.</span></span>

## <a name="permissions"></a><span data-ttu-id="cc2ea-105">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="cc2ea-105">Permissions</span></span>
<span data-ttu-id="cc2ea-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="cc2ea-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="cc2ea-108">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="cc2ea-108">Permission type</span></span>                        | <span data-ttu-id="cc2ea-109">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="cc2ea-109">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="cc2ea-110">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="cc2ea-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="cc2ea-111">サポートされません。</span><span class="sxs-lookup"><span data-stu-id="cc2ea-111">Not Supported.</span></span>                              |
| <span data-ttu-id="cc2ea-112">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="cc2ea-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="cc2ea-113">サポートされません。</span><span class="sxs-lookup"><span data-stu-id="cc2ea-113">Not Supported.</span></span>                              |
| <span data-ttu-id="cc2ea-114">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="cc2ea-114">Application</span></span>                            | <span data-ttu-id="cc2ea-115">なし。</span><span class="sxs-lookup"><span data-stu-id="cc2ea-115">None.</span></span>                                       |

## <a name="http-request"></a><span data-ttu-id="cc2ea-116">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="cc2ea-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /app/calls/{id}/cancelMediaProcessing
POST /applications/{id}/calls/{id}/cancelMediaProcessing
```

## <a name="request-headers"></a><span data-ttu-id="cc2ea-117">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="cc2ea-117">Request headers</span></span>
| <span data-ttu-id="cc2ea-118">名前</span><span class="sxs-lookup"><span data-stu-id="cc2ea-118">Name</span></span>          | <span data-ttu-id="cc2ea-119">説明</span><span class="sxs-lookup"><span data-stu-id="cc2ea-119">Description</span></span>               |
|:--------------|:--------------------------|
| <span data-ttu-id="cc2ea-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="cc2ea-120">Authorization</span></span> | <span data-ttu-id="cc2ea-p102">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="cc2ea-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="cc2ea-123">要求本文</span><span class="sxs-lookup"><span data-stu-id="cc2ea-123">Request body</span></span>
<span data-ttu-id="cc2ea-124">要求本文で、次のパラメーターを含む JSON オブジェクトを指定します。</span><span class="sxs-lookup"><span data-stu-id="cc2ea-124">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="cc2ea-125">パラメーター</span><span class="sxs-lookup"><span data-stu-id="cc2ea-125">Parameter</span></span>      | <span data-ttu-id="cc2ea-126">型</span><span class="sxs-lookup"><span data-stu-id="cc2ea-126">Type</span></span>    | <span data-ttu-id="cc2ea-127">説明</span><span class="sxs-lookup"><span data-stu-id="cc2ea-127">Description</span></span>                                                    |
|:---------------|:--------|:---------------------------------------------------------------|
| <span data-ttu-id="cc2ea-128">すべての</span><span class="sxs-lookup"><span data-stu-id="cc2ea-128">all</span></span>            | <span data-ttu-id="cc2ea-129">Boolean</span><span class="sxs-lookup"><span data-stu-id="cc2ea-129">Boolean</span></span> | <span data-ttu-id="cc2ea-130">すべての操作または現在の終了を停止するかどうかを示すフラグ。</span><span class="sxs-lookup"><span data-stu-id="cc2ea-130">The flag indicating whether to stop all operations or current.</span></span> |
| <span data-ttu-id="cc2ea-131">clientContext</span><span class="sxs-lookup"><span data-stu-id="cc2ea-131">clientContext</span></span>  | <span data-ttu-id="cc2ea-132">String</span><span class="sxs-lookup"><span data-stu-id="cc2ea-132">String</span></span>  | <span data-ttu-id="cc2ea-133">クライアントコンテキスト。</span><span class="sxs-lookup"><span data-stu-id="cc2ea-133">The client context.</span></span>                                            |

## <a name="response"></a><span data-ttu-id="cc2ea-134">応答</span><span class="sxs-lookup"><span data-stu-id="cc2ea-134">Response</span></span>
<span data-ttu-id="cc2ea-135">この`202 Accepted`要求に対して作成された[commsOperation](../resources/commsoperation.md)への uri を持つ応答コードと位置ヘッダーを返します。</span><span class="sxs-lookup"><span data-stu-id="cc2ea-135">Returns `202 Accepted` response code and a Location header with a uri to the [commsOperation](../resources/commsoperation.md) created for this request.</span></span>

## <a name="example"></a><span data-ttu-id="cc2ea-136">例</span><span class="sxs-lookup"><span data-stu-id="cc2ea-136">Example</span></span>
<span data-ttu-id="cc2ea-137">次の例は、この API を呼び出す方法を示しています。</span><span class="sxs-lookup"><span data-stu-id="cc2ea-137">The following example shows how to call this API.</span></span>

##### <a name="request"></a><span data-ttu-id="cc2ea-138">要求</span><span class="sxs-lookup"><span data-stu-id="cc2ea-138">Request</span></span>
<span data-ttu-id="cc2ea-139">次の例は要求を示しています。</span><span class="sxs-lookup"><span data-stu-id="cc2ea-139">The following example shows the request.</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="cc2ea-140">プロトコル</span><span class="sxs-lookup"><span data-stu-id="cc2ea-140">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "call-cancelMediaProcessing"
}-->
```http
POST https://graph.microsoft.com/beta/app/calls/{id}/cancelMediaProcessing
Content-Type: application/json
Content-Length: 62

{
  "all": true,
  "clientContext": "clientContext-value"
}
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="cc2ea-141">C#</span><span class="sxs-lookup"><span data-stu-id="cc2ea-141">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/call-cancelmediaprocessing-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="cc2ea-142">JavaScript</span><span class="sxs-lookup"><span data-stu-id="cc2ea-142">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/call-cancelmediaprocessing-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="cc2ea-143">目的-C</span><span class="sxs-lookup"><span data-stu-id="cc2ea-143">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/call-cancelmediaprocessing-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="cc2ea-144">Java</span><span class="sxs-lookup"><span data-stu-id="cc2ea-144">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/call-cancelmediaprocessing-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="cc2ea-145">応答</span><span class="sxs-lookup"><span data-stu-id="cc2ea-145">Response</span></span>

> <span data-ttu-id="cc2ea-p103">**注:** 読みやすくするために、ここに示す応答オブジェクトは短縮されている場合があります。実際の呼び出しからは、すべてのプロパティが返されます。</span><span class="sxs-lookup"><span data-stu-id="cc2ea-p103">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.commsOperation"
} -->
```http
HTTP/1.1 202 Accepted
Location: https://graph.microsoft.com/beta/app/calls/57dab8b1-894c-409a-b240-bd8beae78896/operations/0fe0623f-d628-42ed-b4bd-8ac290072cc5
```

##### <a name="notification---operation-completed"></a><span data-ttu-id="cc2ea-148">通知-操作が完了しました</span><span class="sxs-lookup"><span data-stu-id="cc2ea-148">Notification - operation completed</span></span>

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
  "description": "call: cancelMediaProcessing",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
