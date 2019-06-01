---
title: ドメインを取得する
description: ドメインオブジェクトのプロパティと関係を取得します。
author: davidmu1
localization_priority: Normal
ms.prod: microsoft-identity-platform
ms.openlocfilehash: ad4fe48857324098bd27ba79c751b407ed59de84
ms.sourcegitcommit: 33f1cf5b3b79bfba6a06b52d34e558a6ba327d21
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/31/2019
ms.locfileid: "34656637"
---
# <a name="get-domain"></a><span data-ttu-id="72eb6-103">ドメインを取得する</span><span class="sxs-lookup"><span data-stu-id="72eb6-103">Get domain</span></span>

<span data-ttu-id="72eb6-104">ドメインオブジェクトのプロパティと関係を取得します。</span><span class="sxs-lookup"><span data-stu-id="72eb6-104">Retrieve the properties and relationships of domain object.</span></span>

## <a name="permissions"></a><span data-ttu-id="72eb6-105">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="72eb6-105">Permissions</span></span>

<span data-ttu-id="72eb6-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="72eb6-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="72eb6-108">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="72eb6-108">Permission type</span></span>      | <span data-ttu-id="72eb6-109">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="72eb6-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="72eb6-110">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="72eb6-110">Delegated (work or school account)</span></span> | <span data-ttu-id="72eb6-111">Directory.Read.All</span><span class="sxs-lookup"><span data-stu-id="72eb6-111">Directory.Read.All</span></span>    |
|<span data-ttu-id="72eb6-112">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="72eb6-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="72eb6-113">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="72eb6-113">Not supported.</span></span>    |
|<span data-ttu-id="72eb6-114">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="72eb6-114">Application</span></span> | <span data-ttu-id="72eb6-115">Directory.Read.All、Domain.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="72eb6-115">Directory.Read.All, Domain.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="72eb6-116">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="72eb6-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->
```http
GET /domains/{id}
```

> <span data-ttu-id="72eb6-117">{Id} には、ドメインを完全修飾ドメイン名で指定します。</span><span class="sxs-lookup"><span data-stu-id="72eb6-117">For {id}, specify the domain with its fully qualified domain name.</span></span>

## <a name="optional-query-parameters"></a><span data-ttu-id="72eb6-118">オプションのクエリ パラメーター</span><span class="sxs-lookup"><span data-stu-id="72eb6-118">Optional query parameters</span></span>

<span data-ttu-id="72eb6-119">このメソッドは、応答をカスタマイズするための [OData クエリ パラメーター](https://developer.microsoft.com/graph/docs/concepts/query_parameters)をサポートします。</span><span class="sxs-lookup"><span data-stu-id="72eb6-119">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="72eb6-120">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="72eb6-120">Request headers</span></span>

| <span data-ttu-id="72eb6-121">名前</span><span class="sxs-lookup"><span data-stu-id="72eb6-121">Name</span></span>      |<span data-ttu-id="72eb6-122">説明</span><span class="sxs-lookup"><span data-stu-id="72eb6-122">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="72eb6-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="72eb6-123">Authorization</span></span>  | <span data-ttu-id="72eb6-p102">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="72eb6-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="72eb6-126">Content-Type</span><span class="sxs-lookup"><span data-stu-id="72eb6-126">Content-Type</span></span>  | <span data-ttu-id="72eb6-127">application/json</span><span class="sxs-lookup"><span data-stu-id="72eb6-127">application/json</span></span> |

## <a name="request-body"></a><span data-ttu-id="72eb6-128">要求本文</span><span class="sxs-lookup"><span data-stu-id="72eb6-128">Request body</span></span>
<span data-ttu-id="72eb6-129">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="72eb6-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="72eb6-130">応答</span><span class="sxs-lookup"><span data-stu-id="72eb6-130">Response</span></span>

<span data-ttu-id="72eb6-131">成功した場合、このメソッド`200 OK`は応答コードと、応答本文で[domain](../resources/domain.md)オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="72eb6-131">If successful, this method returns a `200 OK` response code and [domain](../resources/domain.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="72eb6-132">例</span><span class="sxs-lookup"><span data-stu-id="72eb6-132">Example</span></span>
##### <a name="request"></a><span data-ttu-id="72eb6-133">要求</span><span class="sxs-lookup"><span data-stu-id="72eb6-133">Request</span></span>

<!-- {
  "blockType": "request",
  "sampleKeys": ["contoso.com"],
  "name": "get_domain"
}-->
```http
GET https://graph.microsoft.com/v1.0/domains/contoso.com
```
##### <a name="response"></a><span data-ttu-id="72eb6-134">応答</span><span class="sxs-lookup"><span data-stu-id="72eb6-134">Response</span></span>
<span data-ttu-id="72eb6-p103">注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="72eb6-p103">Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
#### <a name="sdk-sample-code"></a><span data-ttu-id="72eb6-137">SDK サンプル コード</span><span class="sxs-lookup"><span data-stu-id="72eb6-137">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="72eb6-138">C#</span><span class="sxs-lookup"><span data-stu-id="72eb6-138">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/get_domain-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="72eb6-139">Javascript</span><span class="sxs-lookup"><span data-stu-id="72eb6-139">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/get_domain-Javascript-snippets.md)]

---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get domain",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/v1.0/api/domain-get.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/v1.0/api/domain-get.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}-->
