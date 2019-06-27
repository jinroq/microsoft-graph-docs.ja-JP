---
title: '通話: ミュート解除'
description: アプリケーションで自分自身のミュートを解除します。
author: VinodRavichandran
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: ea75e22cc2378e6fb97e8d52741f1ad70aced1c1
ms.sourcegitcommit: 0e1101d499f35b08aa2309e273871438b1774979
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/27/2019
ms.locfileid: "35262231"
---
# <a name="call-unmute"></a><span data-ttu-id="e8fcf-103">通話: ミュート解除</span><span class="sxs-lookup"><span data-stu-id="e8fcf-103">call: unmute</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="e8fcf-104">アプリケーションで自分自身のミュートを解除します。</span><span class="sxs-lookup"><span data-stu-id="e8fcf-104">Allows the application to unmute itself.</span></span>

## <a name="permissions"></a><span data-ttu-id="e8fcf-105">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="e8fcf-105">Permissions</span></span>
<span data-ttu-id="e8fcf-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="e8fcf-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="e8fcf-108">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="e8fcf-108">Permission type</span></span>                        | <span data-ttu-id="e8fcf-109">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="e8fcf-109">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="e8fcf-110">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="e8fcf-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="e8fcf-111">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="e8fcf-111">Not supported.</span></span>                               |
| <span data-ttu-id="e8fcf-112">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="e8fcf-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="e8fcf-113">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="e8fcf-113">Not supported.</span></span>                               |
| <span data-ttu-id="e8fcf-114">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="e8fcf-114">Application</span></span>                            | <span data-ttu-id="e8fcf-115">なし。</span><span class="sxs-lookup"><span data-stu-id="e8fcf-115">None.</span></span>                                        |

## <a name="http-request"></a><span data-ttu-id="e8fcf-116">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="e8fcf-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /app/calls/{id}/unmute
POST /applications/{id}/calls/{id}/unmute
```

## <a name="request-headers"></a><span data-ttu-id="e8fcf-117">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="e8fcf-117">Request headers</span></span>
| <span data-ttu-id="e8fcf-118">名前</span><span class="sxs-lookup"><span data-stu-id="e8fcf-118">Name</span></span>          | <span data-ttu-id="e8fcf-119">説明</span><span class="sxs-lookup"><span data-stu-id="e8fcf-119">Description</span></span>               |
|:--------------|:--------------------------|
| <span data-ttu-id="e8fcf-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="e8fcf-120">Authorization</span></span> | <span data-ttu-id="e8fcf-p102">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="e8fcf-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="e8fcf-123">要求本文</span><span class="sxs-lookup"><span data-stu-id="e8fcf-123">Request body</span></span>
<span data-ttu-id="e8fcf-124">要求本文で、次のパラメーターを含む JSON オブジェクトを指定します。</span><span class="sxs-lookup"><span data-stu-id="e8fcf-124">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="e8fcf-125">パラメーター</span><span class="sxs-lookup"><span data-stu-id="e8fcf-125">Parameter</span></span>      | <span data-ttu-id="e8fcf-126">型</span><span class="sxs-lookup"><span data-stu-id="e8fcf-126">Type</span></span>    |<span data-ttu-id="e8fcf-127">説明</span><span class="sxs-lookup"><span data-stu-id="e8fcf-127">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="e8fcf-128">clientContext</span><span class="sxs-lookup"><span data-stu-id="e8fcf-128">clientContext</span></span>|<span data-ttu-id="e8fcf-129">String</span><span class="sxs-lookup"><span data-stu-id="e8fcf-129">String</span></span>|<span data-ttu-id="e8fcf-130">クライアントコンテキスト。</span><span class="sxs-lookup"><span data-stu-id="e8fcf-130">The client context.</span></span>|

## <a name="response"></a><span data-ttu-id="e8fcf-131">応答</span><span class="sxs-lookup"><span data-stu-id="e8fcf-131">Response</span></span>
<span data-ttu-id="e8fcf-132">成功した場合、この`200 OK`メソッドは応答コードと、応答本文で[commsOperation](../resources/commsoperation.md)オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="e8fcf-132">If successful, this method returns `200 OK` response code and [commsOperation](../resources/commsoperation.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="e8fcf-133">例</span><span class="sxs-lookup"><span data-stu-id="e8fcf-133">Example</span></span>
<span data-ttu-id="e8fcf-134">次の例は、この API を呼び出す方法を示しています。</span><span class="sxs-lookup"><span data-stu-id="e8fcf-134">The following example shows how to call this API.</span></span>

##### <a name="request"></a><span data-ttu-id="e8fcf-135">要求</span><span class="sxs-lookup"><span data-stu-id="e8fcf-135">Request</span></span>
<span data-ttu-id="e8fcf-136">次の例は要求を示しています。</span><span class="sxs-lookup"><span data-stu-id="e8fcf-136">The following example shows the request.</span></span>

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

##### <a name="response"></a><span data-ttu-id="e8fcf-137">応答</span><span class="sxs-lookup"><span data-stu-id="e8fcf-137">Response</span></span>

> <span data-ttu-id="e8fcf-p103">**注:** 読みやすくするために、ここに示す応答オブジェクトは短縮されている場合があります。実際の呼び出しからは、すべてのプロパティが返されます。</span><span class="sxs-lookup"><span data-stu-id="e8fcf-p103">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
#### <a name="sdk-sample-code"></a><span data-ttu-id="e8fcf-140">SDK サンプル コード</span><span class="sxs-lookup"><span data-stu-id="e8fcf-140">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="e8fcf-141">C#</span><span class="sxs-lookup"><span data-stu-id="e8fcf-141">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/call-unmute-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="e8fcf-142">Javascript</span><span class="sxs-lookup"><span data-stu-id="e8fcf-142">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/call-unmute-Javascript-snippets.md)]

# <a name="objective-ctabobjective-c"></a>[<span data-ttu-id="e8fcf-143">目的-C</span><span class="sxs-lookup"><span data-stu-id="e8fcf-143">Objective-C</span></span>](#tab/objective-c)
[!INCLUDE [sample-code](../includes/call-unmute-Objective-C-snippets.md)]
---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

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
    "Error: /api-reference/beta/api/call-unmute.md:\r\n      BookmarkMissing: '[#tab/objective-c](Objective-C)'. Did you mean: #objective-c (score: 4)",
    "Error: /api-reference/beta/api/call-unmute.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/beta/api/call-unmute.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}
-->
