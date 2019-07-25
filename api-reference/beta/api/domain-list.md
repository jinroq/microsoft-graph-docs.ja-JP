---
title: ドメインを一覧表示する
description: ドメインオブジェクトの一覧を取得します。
author: davidmu1
localization_priority: Normal
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 4b6d0d425d6a36729cc21348e555d5158b8ecd10
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/25/2019
ms.locfileid: "35861787"
---
# <a name="list-domains"></a><span data-ttu-id="a03d2-103">ドメインを一覧表示する</span><span class="sxs-lookup"><span data-stu-id="a03d2-103">List domains</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="a03d2-104">ドメインオブジェクトの一覧を取得します。</span><span class="sxs-lookup"><span data-stu-id="a03d2-104">Retrieve a list of domain objects.</span></span>

## <a name="permissions"></a><span data-ttu-id="a03d2-105">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="a03d2-105">Permissions</span></span>
<span data-ttu-id="a03d2-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="a03d2-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a03d2-108">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="a03d2-108">Permission type</span></span>      | <span data-ttu-id="a03d2-109">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="a03d2-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="a03d2-110">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="a03d2-110">Delegated (work or school account)</span></span> | <span data-ttu-id="a03d2-111">Directory.Read.All</span><span class="sxs-lookup"><span data-stu-id="a03d2-111">Directory.Read.All</span></span>    |
|<span data-ttu-id="a03d2-112">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="a03d2-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="a03d2-113">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="a03d2-113">Not supported.</span></span>    |
|<span data-ttu-id="a03d2-114">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="a03d2-114">Application</span></span> | <span data-ttu-id="a03d2-115">Directory.Read.All、Domain.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a03d2-115">Directory.Read.All, Domain.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="a03d2-116">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="a03d2-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /domains
```
## <a name="optional-query-parameters"></a><span data-ttu-id="a03d2-117">オプションのクエリ パラメーター</span><span class="sxs-lookup"><span data-stu-id="a03d2-117">Optional query parameters</span></span>
<span data-ttu-id="a03d2-118">このメソッドは、応答をカスタマイズするための [OData クエリ パラメーター](https://developer.microsoft.com/graph/docs/concepts/query_parameters)をサポートします。</span><span class="sxs-lookup"><span data-stu-id="a03d2-118">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="a03d2-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="a03d2-119">Request headers</span></span>
| <span data-ttu-id="a03d2-120">名前</span><span class="sxs-lookup"><span data-stu-id="a03d2-120">Name</span></span>      |<span data-ttu-id="a03d2-121">説明</span><span class="sxs-lookup"><span data-stu-id="a03d2-121">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="a03d2-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="a03d2-122">Authorization</span></span>  | <span data-ttu-id="a03d2-p102">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="a03d2-p102">Bearer {token}. Required.</span></span>|
| <span data-ttu-id="a03d2-125">承諾</span><span class="sxs-lookup"><span data-stu-id="a03d2-125">Accept</span></span>         | <span data-ttu-id="a03d2-126">application/json;</span><span class="sxs-lookup"><span data-stu-id="a03d2-126">application/json;</span></span> |

## <a name="request-body"></a><span data-ttu-id="a03d2-127">要求本文</span><span class="sxs-lookup"><span data-stu-id="a03d2-127">Request body</span></span>
<span data-ttu-id="a03d2-128">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="a03d2-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="a03d2-129">応答</span><span class="sxs-lookup"><span data-stu-id="a03d2-129">Response</span></span>

<span data-ttu-id="a03d2-130">成功した場合、このメソッド`200 OK`は応答コードと、応答本文で[domain](../resources/domain.md)オブジェクトのコレクションを返します。</span><span class="sxs-lookup"><span data-stu-id="a03d2-130">If successful, this method returns a `200 OK` response code and collection of [domain](../resources/domain.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="a03d2-131">例</span><span class="sxs-lookup"><span data-stu-id="a03d2-131">Example</span></span>
##### <a name="request"></a><span data-ttu-id="a03d2-132">要求</span><span class="sxs-lookup"><span data-stu-id="a03d2-132">Request</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="a03d2-133">プロトコル</span><span class="sxs-lookup"><span data-stu-id="a03d2-133">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_domains"
}-->
```http
GET https://graph.microsoft.com/beta/domains
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="a03d2-134">C#</span><span class="sxs-lookup"><span data-stu-id="a03d2-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-domains-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="a03d2-135">Javascript</span><span class="sxs-lookup"><span data-stu-id="a03d2-135">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-domains-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="a03d2-136">目的-C</span><span class="sxs-lookup"><span data-stu-id="a03d2-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-domains-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="a03d2-137">Java</span><span class="sxs-lookup"><span data-stu-id="a03d2-137">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-domains-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="a03d2-138">応答</span><span class="sxs-lookup"><span data-stu-id="a03d2-138">Response</span></span>
<span data-ttu-id="a03d2-p103">注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="a03d2-p103">Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.domain",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 245

{
  "value": [
    {
      "authenticationType": "authenticationType-value",
      "availabilityStatus": "availabilityStatus-value",
      "isAdminManaged": true,
      "isDefault": true,
      "isInitial": true,
      "isRoot": true,
      "name": "contoso.com",
      "supportedServices": [
        "Email",
        "OfficeCommunicationsOnline"
      ]
    }
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "List domains",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
