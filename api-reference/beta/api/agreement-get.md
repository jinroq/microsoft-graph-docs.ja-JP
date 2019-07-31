---
title: 契約を取得する
description: アグリーメントオブジェクトのプロパティと関係を取得します。
localization_priority: Normal
doc_type: apiPageType
ms.prod: ''
author: ''
ms.openlocfilehash: 21d090a3e1b23a1870fc86d418fd3edfc3ff69ee
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "35945699"
---
# <a name="get-agreement"></a><span data-ttu-id="5c028-103">契約を取得する</span><span class="sxs-lookup"><span data-stu-id="5c028-103">Get agreement</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="5c028-104">[アグリーメント](../resources/agreement.md)オブジェクトのプロパティと関係を取得します。</span><span class="sxs-lookup"><span data-stu-id="5c028-104">Retrieve the properties and relationships of an [agreement](../resources/agreement.md) object.</span></span>
## <a name="permissions"></a><span data-ttu-id="5c028-105">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="5c028-105">Permissions</span></span>
<span data-ttu-id="5c028-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="5c028-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="5c028-108">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="5c028-108">Permission type</span></span>                        | <span data-ttu-id="5c028-109">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="5c028-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="5c028-110">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="5c028-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="5c028-111">Agreement.Read.All</span><span class="sxs-lookup"><span data-stu-id="5c028-111">Agreement.Read.All</span></span> |
|<span data-ttu-id="5c028-112">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="5c028-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="5c028-113">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="5c028-113">Not supported.</span></span> |
|<span data-ttu-id="5c028-114">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="5c028-114">Application</span></span>                            | <span data-ttu-id="5c028-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="5c028-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="5c028-116">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="5c028-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /agreements/<id>
```
<!--
## Optional query parameters
This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.
-->

## <a name="request-headers"></a><span data-ttu-id="5c028-117">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="5c028-117">Request headers</span></span>
| <span data-ttu-id="5c028-118">名前</span><span class="sxs-lookup"><span data-stu-id="5c028-118">Name</span></span>         | <span data-ttu-id="5c028-119">型</span><span class="sxs-lookup"><span data-stu-id="5c028-119">Type</span></span>        | <span data-ttu-id="5c028-120">説明</span><span class="sxs-lookup"><span data-stu-id="5c028-120">Description</span></span> |
|:-------------|:------------|:------------|
| <span data-ttu-id="5c028-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="5c028-121">Authorization</span></span> | <span data-ttu-id="5c028-122">string</span><span class="sxs-lookup"><span data-stu-id="5c028-122">string</span></span> | <span data-ttu-id="5c028-p102">ベアラー \{トークン\}。必須。</span><span class="sxs-lookup"><span data-stu-id="5c028-p102">Bearer \{token\}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="5c028-125">要求本文</span><span class="sxs-lookup"><span data-stu-id="5c028-125">Request body</span></span>
<span data-ttu-id="5c028-126">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="5c028-126">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="5c028-127">応答</span><span class="sxs-lookup"><span data-stu-id="5c028-127">Response</span></span>
<span data-ttu-id="5c028-128">成功した場合、このメソッド`200 OK`は応答コードと、応答本文で[アグリーメント](../resources/agreement.md)オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="5c028-128">If successful, this method returns a `200 OK` response code and [agreement](../resources/agreement.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="5c028-129">例</span><span class="sxs-lookup"><span data-stu-id="5c028-129">Example</span></span>
##### <a name="request"></a><span data-ttu-id="5c028-130">要求</span><span class="sxs-lookup"><span data-stu-id="5c028-130">Request</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="5c028-131">プロトコル</span><span class="sxs-lookup"><span data-stu-id="5c028-131">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_agreement"
}-->
```http
GET https://graph.microsoft.com/beta/agreements/<id>?$expand=files
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="5c028-132">C#</span><span class="sxs-lookup"><span data-stu-id="5c028-132">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-agreement-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="5c028-133">Javascript</span><span class="sxs-lookup"><span data-stu-id="5c028-133">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-agreement-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="5c028-134">目的-C</span><span class="sxs-lookup"><span data-stu-id="5c028-134">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-agreement-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="5c028-135">Java</span><span class="sxs-lookup"><span data-stu-id="5c028-135">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-agreement-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="5c028-136">応答</span><span class="sxs-lookup"><span data-stu-id="5c028-136">Response</span></span>
><span data-ttu-id="5c028-p103">**注:** 読みやすくするために、ここに示す応答オブジェクトは短縮されている場合があります。実際の呼び出しからは、すべてのプロパティが返されます。</span><span class="sxs-lookup"><span data-stu-id="5c028-p103">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.agreement"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "displayName": "MSGraph Sample",
  "isViewingBeforeAcceptanceRequired": true,
  "id": "id-value",
  "files": [
    {
      "id": "id-value",
      "language": "en",
      "fileName": "TOU.pdf",
      "isDefault": true
    }
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Get agreement",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
