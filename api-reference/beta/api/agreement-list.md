---
title: リスト契約
description: 契約オブジェクトのリストを取得します。
ms.openlocfilehash: c49a23be801168f552b9db8f1911e03e65d521ed
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27069291"
---
# <a name="list-agreements"></a><span data-ttu-id="d13dc-103">リスト契約</span><span class="sxs-lookup"><span data-stu-id="d13dc-103">List agreements</span></span>

> <span data-ttu-id="d13dc-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="d13dc-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="d13dc-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="d13dc-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="d13dc-106">[契約](../resources/agreement.md)オブジェクトのリストを取得します。</span><span class="sxs-lookup"><span data-stu-id="d13dc-106">Retrieve a list of [agreement](../resources/agreement.md) objects.</span></span>
## <a name="permissions"></a><span data-ttu-id="d13dc-107">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="d13dc-107">Permissions</span></span>
<span data-ttu-id="d13dc-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="d13dc-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d13dc-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="d13dc-110">Permission type</span></span>                        | <span data-ttu-id="d13dc-111">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="d13dc-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="d13dc-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="d13dc-112">Delegated (work or school account)</span></span>     | <span data-ttu-id="d13dc-113">Agreement.Read.All</span><span class="sxs-lookup"><span data-stu-id="d13dc-113">Agreement.Read.All</span></span> |
|<span data-ttu-id="d13dc-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="d13dc-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="d13dc-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="d13dc-115">Not supported.</span></span> |
|<span data-ttu-id="d13dc-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="d13dc-116">Application</span></span>                            | <span data-ttu-id="d13dc-117">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="d13dc-117">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="d13dc-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="d13dc-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /agreements
```
<!--
## Optional query parameters
This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.
-->

## <a name="request-headers"></a><span data-ttu-id="d13dc-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="d13dc-119">Request headers</span></span>
| <span data-ttu-id="d13dc-120">名前</span><span class="sxs-lookup"><span data-stu-id="d13dc-120">Name</span></span>         | <span data-ttu-id="d13dc-121">型</span><span class="sxs-lookup"><span data-stu-id="d13dc-121">Type</span></span>        | <span data-ttu-id="d13dc-122">説明</span><span class="sxs-lookup"><span data-stu-id="d13dc-122">Description</span></span> |
|:-------------|:------------|:------------|
| <span data-ttu-id="d13dc-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="d13dc-123">Authorization</span></span> | <span data-ttu-id="d13dc-124">string</span><span class="sxs-lookup"><span data-stu-id="d13dc-124">string</span></span> | <span data-ttu-id="d13dc-125">ベアラー\{トークン\}。</span><span class="sxs-lookup"><span data-stu-id="d13dc-125">Bearer \{token\}.</span></span> <span data-ttu-id="d13dc-126">必須。</span><span class="sxs-lookup"><span data-stu-id="d13dc-126">Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="d13dc-127">要求本文</span><span class="sxs-lookup"><span data-stu-id="d13dc-127">Request body</span></span>
<span data-ttu-id="d13dc-128">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="d13dc-128">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="d13dc-129">応答</span><span class="sxs-lookup"><span data-stu-id="d13dc-129">Response</span></span>
<span data-ttu-id="d13dc-130">かどうかは成功すると、このメソッドが返されます、`200 OK`応答コードおよび応答の本文の[許可書](../resources/agreement.md)オブジェクトのコレクションです。</span><span class="sxs-lookup"><span data-stu-id="d13dc-130">If successful, this method returns a `200 OK` response code and collection of [agreement](../resources/agreement.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="d13dc-131">例</span><span class="sxs-lookup"><span data-stu-id="d13dc-131">Example</span></span>
##### <a name="request"></a><span data-ttu-id="d13dc-132">要求</span><span class="sxs-lookup"><span data-stu-id="d13dc-132">Request</span></span>
<!-- {
  "blockType": "request",
  "name": "get_agreements"
}-->
```http
GET https://graph.microsoft.com/beta/agreements
```
##### <a name="response"></a><span data-ttu-id="d13dc-133">応答</span><span class="sxs-lookup"><span data-stu-id="d13dc-133">Response</span></span>
><span data-ttu-id="d13dc-p104">**注:** 読みやすくするために、ここに示す応答オブジェクトは短くされている場合があります。実際の呼び出しからは、すべてのプロパティが返されます。</span><span class="sxs-lookup"><span data-stu-id="d13dc-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.agreement",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 146

{
  "value": [
    {
      "displayName": "displayName-value",
      "isViewingBeforeAcceptanceRequired": true,
      "id": "id-value"
    }
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List agreements",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->