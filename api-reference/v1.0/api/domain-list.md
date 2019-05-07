---
title: ドメインを一覧表示する
description: ドメインオブジェクトの一覧を取得します。
author: lleonard-msft
localization_priority: Normal
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 6c84c01a423bed5507cbc07e8202a2e963e5b0c4
ms.sourcegitcommit: b8d01acfc1cb7610a0e1f5c18065da415bae0777
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/06/2019
ms.locfileid: "33617033"
---
# <a name="list-domains"></a><span data-ttu-id="c5046-103">ドメインを一覧表示する</span><span class="sxs-lookup"><span data-stu-id="c5046-103">List domains</span></span>

<span data-ttu-id="c5046-104">ドメインオブジェクトの一覧を取得します。</span><span class="sxs-lookup"><span data-stu-id="c5046-104">Retrieve a list of domain objects.</span></span>

## <a name="permissions"></a><span data-ttu-id="c5046-105">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="c5046-105">Permissions</span></span>
<span data-ttu-id="c5046-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="c5046-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c5046-108">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="c5046-108">Permission type</span></span>      | <span data-ttu-id="c5046-109">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="c5046-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="c5046-110">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="c5046-110">Delegated (work or school account)</span></span> | <span data-ttu-id="c5046-111">Directory.Read.All</span><span class="sxs-lookup"><span data-stu-id="c5046-111">Directory.Read.All</span></span>    |
|<span data-ttu-id="c5046-112">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="c5046-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="c5046-113">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="c5046-113">Not supported.</span></span>    |
|<span data-ttu-id="c5046-114">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="c5046-114">Application</span></span> | <span data-ttu-id="c5046-115">Directory.Read.All、Domain.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c5046-115">Directory.Read.All, Domain.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="c5046-116">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="c5046-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /domains
```
## <a name="optional-query-parameters"></a><span data-ttu-id="c5046-117">オプションのクエリ パラメーター</span><span class="sxs-lookup"><span data-stu-id="c5046-117">Optional query parameters</span></span>
<span data-ttu-id="c5046-118">このメソッドは、応答をカスタマイズするための [OData クエリ パラメーター](https://developer.microsoft.com/graph/docs/concepts/query_parameters)をサポートします。</span><span class="sxs-lookup"><span data-stu-id="c5046-118">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="c5046-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="c5046-119">Request headers</span></span>
| <span data-ttu-id="c5046-120">名前</span><span class="sxs-lookup"><span data-stu-id="c5046-120">Name</span></span>      |<span data-ttu-id="c5046-121">説明</span><span class="sxs-lookup"><span data-stu-id="c5046-121">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="c5046-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="c5046-122">Authorization</span></span>  | <span data-ttu-id="c5046-p102">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="c5046-p102">Bearer {token}. Required.</span></span>|
| <span data-ttu-id="c5046-125">承諾</span><span class="sxs-lookup"><span data-stu-id="c5046-125">Accept</span></span>         | <span data-ttu-id="c5046-126">application/json;</span><span class="sxs-lookup"><span data-stu-id="c5046-126">application/json;</span></span> |

## <a name="request-body"></a><span data-ttu-id="c5046-127">要求本文</span><span class="sxs-lookup"><span data-stu-id="c5046-127">Request body</span></span>
<span data-ttu-id="c5046-128">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="c5046-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="c5046-129">応答</span><span class="sxs-lookup"><span data-stu-id="c5046-129">Response</span></span>

<span data-ttu-id="c5046-130">成功した場合、このメソッド`200 OK`は応答コードと、応答本文で[domain](../resources/domain.md)オブジェクトのコレクションを返します。</span><span class="sxs-lookup"><span data-stu-id="c5046-130">If successful, this method returns a `200 OK` response code and collection of [domain](../resources/domain.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="c5046-131">例</span><span class="sxs-lookup"><span data-stu-id="c5046-131">Example</span></span>
##### <a name="request"></a><span data-ttu-id="c5046-132">要求</span><span class="sxs-lookup"><span data-stu-id="c5046-132">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "get_domains"
}-->
```http
GET https://graph.microsoft.com/v1.0/domains
```
##### <a name="response"></a><span data-ttu-id="c5046-133">応答</span><span class="sxs-lookup"><span data-stu-id="c5046-133">Response</span></span>
<span data-ttu-id="c5046-p103">注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="c5046-p103">Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
      "id": "contoso.com",
      "supportedServices": [
        "Email",
        "OfficeCommunicationsOnline"
      ]
    }
  ]
}
```
#### <a name="sdk-sample-code"></a><span data-ttu-id="c5046-136">SDK サンプルコード</span><span class="sxs-lookup"><span data-stu-id="c5046-136">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="c5046-137">Visual</span><span class="sxs-lookup"><span data-stu-id="c5046-137">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/get_domains-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="c5046-138">Java</span><span class="sxs-lookup"><span data-stu-id="c5046-138">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/get_domains-Javascript-snippets.md)]

---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List domains",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/v1.0/api/domain-list.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/v1.0/api/domain-list.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}-->
