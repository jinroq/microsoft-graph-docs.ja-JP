---
title: '通話: ミュート解除'
description: アプリケーションで自分自身のミュートを解除します。
author: VinodRavichandran
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: 83a309dd1ef321bb3149f2d3d0f9b2a48f33ee7f
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "35944394"
---
# <a name="call-unmute"></a><span data-ttu-id="e668a-103">通話: ミュート解除</span><span class="sxs-lookup"><span data-stu-id="e668a-103">call: unmute</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="e668a-104">アプリケーションで自分自身のミュートを解除します。</span><span class="sxs-lookup"><span data-stu-id="e668a-104">Allows the application to unmute itself.</span></span>

## <a name="permissions"></a><span data-ttu-id="e668a-105">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="e668a-105">Permissions</span></span>
<span data-ttu-id="e668a-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="e668a-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="e668a-108">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="e668a-108">Permission type</span></span>                        | <span data-ttu-id="e668a-109">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="e668a-109">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="e668a-110">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="e668a-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="e668a-111">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="e668a-111">Not supported.</span></span>                               |
| <span data-ttu-id="e668a-112">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="e668a-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="e668a-113">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="e668a-113">Not supported.</span></span>                               |
| <span data-ttu-id="e668a-114">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="e668a-114">Application</span></span>                            | <span data-ttu-id="e668a-115">なし。</span><span class="sxs-lookup"><span data-stu-id="e668a-115">None.</span></span>                                        |

## <a name="http-request"></a><span data-ttu-id="e668a-116">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="e668a-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /app/calls/{id}/unmute
POST /applications/{id}/calls/{id}/unmute
```

## <a name="request-headers"></a><span data-ttu-id="e668a-117">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="e668a-117">Request headers</span></span>
| <span data-ttu-id="e668a-118">名前</span><span class="sxs-lookup"><span data-stu-id="e668a-118">Name</span></span>          | <span data-ttu-id="e668a-119">説明</span><span class="sxs-lookup"><span data-stu-id="e668a-119">Description</span></span>               |
|:--------------|:--------------------------|
| <span data-ttu-id="e668a-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="e668a-120">Authorization</span></span> | <span data-ttu-id="e668a-p102">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="e668a-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="e668a-123">要求本文</span><span class="sxs-lookup"><span data-stu-id="e668a-123">Request body</span></span>
<span data-ttu-id="e668a-124">要求本文で、次のパラメーターを含む JSON オブジェクトを指定します。</span><span class="sxs-lookup"><span data-stu-id="e668a-124">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="e668a-125">パラメーター</span><span class="sxs-lookup"><span data-stu-id="e668a-125">Parameter</span></span>      | <span data-ttu-id="e668a-126">型</span><span class="sxs-lookup"><span data-stu-id="e668a-126">Type</span></span>    |<span data-ttu-id="e668a-127">説明</span><span class="sxs-lookup"><span data-stu-id="e668a-127">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="e668a-128">clientContext</span><span class="sxs-lookup"><span data-stu-id="e668a-128">clientContext</span></span>|<span data-ttu-id="e668a-129">String</span><span class="sxs-lookup"><span data-stu-id="e668a-129">String</span></span>|<span data-ttu-id="e668a-130">クライアントコンテキスト。</span><span class="sxs-lookup"><span data-stu-id="e668a-130">The client context.</span></span>|

## <a name="response"></a><span data-ttu-id="e668a-131">応答</span><span class="sxs-lookup"><span data-stu-id="e668a-131">Response</span></span>
<span data-ttu-id="e668a-132">成功した場合、この`200 OK`メソッドは応答コードと、応答本文で[commsOperation](../resources/commsoperation.md)オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="e668a-132">If successful, this method returns `200 OK` response code and [commsOperation](../resources/commsoperation.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="e668a-133">例</span><span class="sxs-lookup"><span data-stu-id="e668a-133">Example</span></span>
<span data-ttu-id="e668a-134">次の例は、この API を呼び出す方法を示しています。</span><span class="sxs-lookup"><span data-stu-id="e668a-134">The following example shows how to call this API.</span></span>

##### <a name="request"></a><span data-ttu-id="e668a-135">要求</span><span class="sxs-lookup"><span data-stu-id="e668a-135">Request</span></span>
<span data-ttu-id="e668a-136">次の例は要求を示しています。</span><span class="sxs-lookup"><span data-stu-id="e668a-136">The following example shows the request.</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="e668a-137">プロトコル</span><span class="sxs-lookup"><span data-stu-id="e668a-137">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "call-unmute"
}-->
```http
POST https://graph.microsoft.com/beta/app/calls/{id}/unmute
Content-Type: application/json
Content-Length: 46

{
  "clientContext": "clientContext-value"
}
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="e668a-138">C#</span><span class="sxs-lookup"><span data-stu-id="e668a-138">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/call-unmute-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="e668a-139">Javascript</span><span class="sxs-lookup"><span data-stu-id="e668a-139">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/call-unmute-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="e668a-140">目的-C</span><span class="sxs-lookup"><span data-stu-id="e668a-140">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/call-unmute-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="e668a-141">Java</span><span class="sxs-lookup"><span data-stu-id="e668a-141">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/call-unmute-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="e668a-142">応答</span><span class="sxs-lookup"><span data-stu-id="e668a-142">Response</span></span>

> <span data-ttu-id="e668a-p103">**注:** 読みやすくするために、ここに示す応答オブジェクトは短縮されている場合があります。実際の呼び出しからは、すべてのプロパティが返されます。</span><span class="sxs-lookup"><span data-stu-id="e668a-p103">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.commsOperation"
} -->
```http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 259

{
  "id": "17e3b46c-f61d-4f4d-9635-c626ef18e6ad",
  "status": "completed",
  "createdDateTime": "2018-09-06T15:58:41Z",
  "lastActionDateTime": "2018-09-06T15:58:41Z",
  "clientContext": "d45324c1-fcb5-430a-902c-f20af696537c"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "call: unmute",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
