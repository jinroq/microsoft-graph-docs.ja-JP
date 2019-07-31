---
title: ドメインを取得する
description: ドメインオブジェクトのプロパティと関係を取得します。
author: davidmu1
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 84cb4a896c98e3a0ed1d751e1ab25e0c630e9f1b
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "35957473"
---
# <a name="get-domain"></a><span data-ttu-id="e7fc5-103">ドメインを取得する</span><span class="sxs-lookup"><span data-stu-id="e7fc5-103">Get domain</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="e7fc5-104">ドメインオブジェクトのプロパティと関係を取得します。</span><span class="sxs-lookup"><span data-stu-id="e7fc5-104">Retrieve the properties and relationships of domain object.</span></span>

## <a name="permissions"></a><span data-ttu-id="e7fc5-105">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="e7fc5-105">Permissions</span></span>

<span data-ttu-id="e7fc5-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="e7fc5-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="e7fc5-108">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="e7fc5-108">Permission type</span></span>      | <span data-ttu-id="e7fc5-109">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="e7fc5-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="e7fc5-110">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="e7fc5-110">Delegated (work or school account)</span></span> | <span data-ttu-id="e7fc5-111">Directory.Read.All</span><span class="sxs-lookup"><span data-stu-id="e7fc5-111">Directory.Read.All</span></span>    |
|<span data-ttu-id="e7fc5-112">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="e7fc5-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="e7fc5-113">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="e7fc5-113">Not supported.</span></span>    |
|<span data-ttu-id="e7fc5-114">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="e7fc5-114">Application</span></span> | <span data-ttu-id="e7fc5-115">Directory.Read.All、Domain.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e7fc5-115">Directory.Read.All, Domain.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="e7fc5-116">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="e7fc5-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->
```http
GET /domains/{id}
```

> <span data-ttu-id="e7fc5-117">{Id} には、ドメインを完全修飾ドメイン名で指定します。</span><span class="sxs-lookup"><span data-stu-id="e7fc5-117">For {id}, specify the domain with its fully qualified domain name.</span></span>

## <a name="optional-query-parameters"></a><span data-ttu-id="e7fc5-118">オプションのクエリ パラメーター</span><span class="sxs-lookup"><span data-stu-id="e7fc5-118">Optional query parameters</span></span>

<span data-ttu-id="e7fc5-119">このメソッドは、応答をカスタマイズするための [OData クエリ パラメーター](https://developer.microsoft.com/graph/docs/concepts/query_parameters)をサポートします。</span><span class="sxs-lookup"><span data-stu-id="e7fc5-119">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="e7fc5-120">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="e7fc5-120">Request headers</span></span>

| <span data-ttu-id="e7fc5-121">名前</span><span class="sxs-lookup"><span data-stu-id="e7fc5-121">Name</span></span>      |<span data-ttu-id="e7fc5-122">説明</span><span class="sxs-lookup"><span data-stu-id="e7fc5-122">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="e7fc5-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="e7fc5-123">Authorization</span></span>  | <span data-ttu-id="e7fc5-p102">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="e7fc5-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="e7fc5-126">Content-Type</span><span class="sxs-lookup"><span data-stu-id="e7fc5-126">Content-Type</span></span>  | <span data-ttu-id="e7fc5-127">application/json</span><span class="sxs-lookup"><span data-stu-id="e7fc5-127">application/json</span></span> |

## <a name="request-body"></a><span data-ttu-id="e7fc5-128">要求本文</span><span class="sxs-lookup"><span data-stu-id="e7fc5-128">Request body</span></span>
<span data-ttu-id="e7fc5-129">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="e7fc5-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="e7fc5-130">応答</span><span class="sxs-lookup"><span data-stu-id="e7fc5-130">Response</span></span>

<span data-ttu-id="e7fc5-131">成功した場合、このメソッド`200 OK`は応答コードと、応答本文で[domain](../resources/domain.md)オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="e7fc5-131">If successful, this method returns a `200 OK` response code and [domain](../resources/domain.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="e7fc5-132">例</span><span class="sxs-lookup"><span data-stu-id="e7fc5-132">Example</span></span>
##### <a name="request"></a><span data-ttu-id="e7fc5-133">要求</span><span class="sxs-lookup"><span data-stu-id="e7fc5-133">Request</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="e7fc5-134">プロトコル</span><span class="sxs-lookup"><span data-stu-id="e7fc5-134">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_domain"
}-->
```http
GET https://graph.microsoft.com/beta/domains/contoso.com
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="e7fc5-135">C#</span><span class="sxs-lookup"><span data-stu-id="e7fc5-135">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-domain-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="e7fc5-136">Javascript</span><span class="sxs-lookup"><span data-stu-id="e7fc5-136">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-domain-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="e7fc5-137">目的-C</span><span class="sxs-lookup"><span data-stu-id="e7fc5-137">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-domain-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="e7fc5-138">Java</span><span class="sxs-lookup"><span data-stu-id="e7fc5-138">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-domain-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="e7fc5-139">応答</span><span class="sxs-lookup"><span data-stu-id="e7fc5-139">Response</span></span>
<span data-ttu-id="e7fc5-p103">注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="e7fc5-p103">Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.domain"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 192

{
  "authenticationType": "authenticationType-value",
  "availabilityStatus": "availabilityStatus-value",
  "id": "contoso.com",
  "isAdminManaged": true,
  "isDefault": true,
  "isInitial": true,
  "isRoot": true
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Get domain",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
