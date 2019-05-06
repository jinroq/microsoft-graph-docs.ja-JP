---
title: 契約の取得
description: Contract オブジェクトのプロパティと関係を取得します。
localization_priority: Normal
author: lleonard-msft
ms.prod: microsoft-identity-platform
ms.openlocfilehash: b91a985b83867d762ec5a3efd54d1eb97301399b
ms.sourcegitcommit: b8d01acfc1cb7610a0e1f5c18065da415bae0777
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/06/2019
ms.locfileid: "33591295"
---
# <a name="get-contract"></a><span data-ttu-id="ff102-103">契約の取得</span><span class="sxs-lookup"><span data-stu-id="ff102-103">Get Contract</span></span>

<span data-ttu-id="ff102-104">[Contract](../resources/contract.md)オブジェクトのプロパティと関係を取得します。</span><span class="sxs-lookup"><span data-stu-id="ff102-104">Retrieve the properties and relationships of [contract](../resources/contract.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="ff102-105">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="ff102-105">Permissions</span></span>

<span data-ttu-id="ff102-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="ff102-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="ff102-108">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="ff102-108">Permission type</span></span>      | <span data-ttu-id="ff102-109">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="ff102-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="ff102-110">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="ff102-110">Delegated (work or school account)</span></span> | <span data-ttu-id="ff102-111">Directory.Read.All、Directory.ReadWrite.All、Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="ff102-111">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="ff102-112">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="ff102-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="ff102-113">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="ff102-113">Not supported.</span></span>    |
|<span data-ttu-id="ff102-114">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="ff102-114">Application</span></span> | <span data-ttu-id="ff102-115">Directory.Read.All、Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ff102-115">Directory.Read.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="ff102-116">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="ff102-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /contracts/{id}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="ff102-117">オプションのクエリ パラメーター</span><span class="sxs-lookup"><span data-stu-id="ff102-117">Optional query parameters</span></span>

<span data-ttu-id="ff102-118">このメソッドは、応答をカスタマイズするための [OData クエリ パラメーター](https://developer.microsoft.com/graph/docs/concepts/query_parameters)をサポートします。</span><span class="sxs-lookup"><span data-stu-id="ff102-118">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="ff102-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="ff102-119">Request headers</span></span>

| <span data-ttu-id="ff102-120">名前</span><span class="sxs-lookup"><span data-stu-id="ff102-120">Name</span></span>      |<span data-ttu-id="ff102-121">説明</span><span class="sxs-lookup"><span data-stu-id="ff102-121">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="ff102-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="ff102-122">Authorization</span></span>  | <span data-ttu-id="ff102-p102">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="ff102-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="ff102-125">要求本文</span><span class="sxs-lookup"><span data-stu-id="ff102-125">Request body</span></span>

<span data-ttu-id="ff102-126">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="ff102-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="ff102-127">応答</span><span class="sxs-lookup"><span data-stu-id="ff102-127">Response</span></span>

<span data-ttu-id="ff102-128">成功した場合、このメソッド`200 OK`は応答コードと、応答本文で[Contract](../resources/contract.md)オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="ff102-128">If successful, this method returns a `200 OK` response code and [Contract](../resources/contract.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="ff102-129">例</span><span class="sxs-lookup"><span data-stu-id="ff102-129">Example</span></span>
##### <a name="request"></a><span data-ttu-id="ff102-130">要求</span><span class="sxs-lookup"><span data-stu-id="ff102-130">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "get_contract"
}-->
```http
GET https://graph.microsoft.com/v1.0/contracts/{id}
```

##### <a name="response"></a><span data-ttu-id="ff102-131">応答</span><span class="sxs-lookup"><span data-stu-id="ff102-131">Response</span></span>
<span data-ttu-id="ff102-p103">注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="ff102-p103">Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.contract"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 186

{
  "contractType": "contractType-value",
  "customerId": "customerId-value",
  "defaultDomainName": "defaultDomainName-value",
  "displayName": "displayName-value",
  "id": "id-value"
}
```
#### <a name="sdk-sample-code"></a><span data-ttu-id="ff102-134">SDK サンプルコード</span><span class="sxs-lookup"><span data-stu-id="ff102-134">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="ff102-135">Visual</span><span class="sxs-lookup"><span data-stu-id="ff102-135">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/get_contract-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="ff102-136">Java</span><span class="sxs-lookup"><span data-stu-id="ff102-136">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/get_contract-Javascript-snippets.md)]

---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get Contract",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/v1.0/api/contract-get.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/v1.0/api/contract-get.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}-->
