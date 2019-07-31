---
title: 契約を一覧表示する
description: アグリーメントオブジェクトの一覧を取得します。
localization_priority: Normal
doc_type: apiPageType
ms.prod: ''
author: ''
ms.openlocfilehash: 7c07a0308443c1d631122dd22c031789d8eb5acf
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "35945712"
---
# <a name="list-agreements"></a><span data-ttu-id="24c73-103">契約を一覧表示する</span><span class="sxs-lookup"><span data-stu-id="24c73-103">List agreements</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="24c73-104">[アグリーメント](../resources/agreement.md)オブジェクトの一覧を取得します。</span><span class="sxs-lookup"><span data-stu-id="24c73-104">Retrieve a list of [agreement](../resources/agreement.md) objects.</span></span>
## <a name="permissions"></a><span data-ttu-id="24c73-105">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="24c73-105">Permissions</span></span>
<span data-ttu-id="24c73-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="24c73-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="24c73-108">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="24c73-108">Permission type</span></span>                        | <span data-ttu-id="24c73-109">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="24c73-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="24c73-110">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="24c73-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="24c73-111">Agreement.Read.All</span><span class="sxs-lookup"><span data-stu-id="24c73-111">Agreement.Read.All</span></span> |
|<span data-ttu-id="24c73-112">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="24c73-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="24c73-113">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="24c73-113">Not supported.</span></span> |
|<span data-ttu-id="24c73-114">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="24c73-114">Application</span></span>                            | <span data-ttu-id="24c73-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="24c73-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="24c73-116">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="24c73-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /agreements
```
<!--
## Optional query parameters
This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.
-->

## <a name="request-headers"></a><span data-ttu-id="24c73-117">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="24c73-117">Request headers</span></span>
| <span data-ttu-id="24c73-118">名前</span><span class="sxs-lookup"><span data-stu-id="24c73-118">Name</span></span>         | <span data-ttu-id="24c73-119">型</span><span class="sxs-lookup"><span data-stu-id="24c73-119">Type</span></span>        | <span data-ttu-id="24c73-120">説明</span><span class="sxs-lookup"><span data-stu-id="24c73-120">Description</span></span> |
|:-------------|:------------|:------------|
| <span data-ttu-id="24c73-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="24c73-121">Authorization</span></span> | <span data-ttu-id="24c73-122">string</span><span class="sxs-lookup"><span data-stu-id="24c73-122">string</span></span> | <span data-ttu-id="24c73-p102">ベアラー \{トークン\}。必須。</span><span class="sxs-lookup"><span data-stu-id="24c73-p102">Bearer \{token\}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="24c73-125">要求本文</span><span class="sxs-lookup"><span data-stu-id="24c73-125">Request body</span></span>
<span data-ttu-id="24c73-126">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="24c73-126">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="24c73-127">応答</span><span class="sxs-lookup"><span data-stu-id="24c73-127">Response</span></span>
<span data-ttu-id="24c73-128">成功した場合、このメソッド`200 OK`は応答コードと、応答本文で[アグリーメント](../resources/agreement.md)オブジェクトのコレクションを返します。</span><span class="sxs-lookup"><span data-stu-id="24c73-128">If successful, this method returns a `200 OK` response code and collection of [agreement](../resources/agreement.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="24c73-129">例</span><span class="sxs-lookup"><span data-stu-id="24c73-129">Example</span></span>
##### <a name="request"></a><span data-ttu-id="24c73-130">要求</span><span class="sxs-lookup"><span data-stu-id="24c73-130">Request</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="24c73-131">プロトコル</span><span class="sxs-lookup"><span data-stu-id="24c73-131">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_agreements"
}-->
```http
GET https://graph.microsoft.com/beta/agreements
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="24c73-132">C#</span><span class="sxs-lookup"><span data-stu-id="24c73-132">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-agreements-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="24c73-133">Javascript</span><span class="sxs-lookup"><span data-stu-id="24c73-133">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-agreements-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="24c73-134">目的-C</span><span class="sxs-lookup"><span data-stu-id="24c73-134">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-agreements-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="24c73-135">Java</span><span class="sxs-lookup"><span data-stu-id="24c73-135">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-agreements-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="24c73-136">応答</span><span class="sxs-lookup"><span data-stu-id="24c73-136">Response</span></span>
><span data-ttu-id="24c73-p103">**注:** 読みやすくするために、ここに示す応答オブジェクトは短縮されている場合があります。実際の呼び出しからは、すべてのプロパティが返されます。</span><span class="sxs-lookup"><span data-stu-id="24c73-p103">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
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
<!--
{
  "type": "#page.annotation",
  "description": "List agreements",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
