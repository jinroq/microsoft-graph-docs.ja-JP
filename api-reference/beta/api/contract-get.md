---
title: 契約の取得
description: Contract オブジェクトのプロパティと関係を取得します。
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
ms.openlocfilehash: a922dc6c764f3a37b20ba8d2442fc8d5af85e06e
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/02/2019
ms.locfileid: "35437545"
---
# <a name="get-contract"></a><span data-ttu-id="141e7-103">契約の取得</span><span class="sxs-lookup"><span data-stu-id="141e7-103">Get Contract</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="141e7-104">[Contract](../resources/contract.md)オブジェクトのプロパティと関係を取得します。</span><span class="sxs-lookup"><span data-stu-id="141e7-104">Retrieve the properties and relationships of [contract](../resources/contract.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="141e7-105">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="141e7-105">Permissions</span></span>

<span data-ttu-id="141e7-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="141e7-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="141e7-108">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="141e7-108">Permission type</span></span>      | <span data-ttu-id="141e7-109">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="141e7-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="141e7-110">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="141e7-110">Delegated (work or school account)</span></span> | <span data-ttu-id="141e7-111">Directory.Read.All、Directory.ReadWrite.All、Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="141e7-111">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="141e7-112">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="141e7-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="141e7-113">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="141e7-113">Not supported.</span></span>    |
|<span data-ttu-id="141e7-114">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="141e7-114">Application</span></span> | <span data-ttu-id="141e7-115">Directory.Read.All、Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="141e7-115">Directory.Read.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="141e7-116">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="141e7-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /contracts/{id}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="141e7-117">オプションのクエリ パラメーター</span><span class="sxs-lookup"><span data-stu-id="141e7-117">Optional query parameters</span></span>

<span data-ttu-id="141e7-118">このメソッドは、応答をカスタマイズするための [OData クエリ パラメーター](https://developer.microsoft.com/graph/docs/concepts/query_parameters)をサポートします。</span><span class="sxs-lookup"><span data-stu-id="141e7-118">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="141e7-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="141e7-119">Request headers</span></span>

| <span data-ttu-id="141e7-120">名前</span><span class="sxs-lookup"><span data-stu-id="141e7-120">Name</span></span>      |<span data-ttu-id="141e7-121">説明</span><span class="sxs-lookup"><span data-stu-id="141e7-121">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="141e7-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="141e7-122">Authorization</span></span>  | <span data-ttu-id="141e7-p102">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="141e7-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="141e7-125">要求本文</span><span class="sxs-lookup"><span data-stu-id="141e7-125">Request body</span></span>

<span data-ttu-id="141e7-126">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="141e7-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="141e7-127">応答</span><span class="sxs-lookup"><span data-stu-id="141e7-127">Response</span></span>

<span data-ttu-id="141e7-128">成功した場合、このメソッド`200 OK`は応答コードと、応答本文で[Contract](../resources/contract.md)オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="141e7-128">If successful, this method returns a `200 OK` response code and [Contract](../resources/contract.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="141e7-129">例</span><span class="sxs-lookup"><span data-stu-id="141e7-129">Example</span></span>
##### <a name="request"></a><span data-ttu-id="141e7-130">要求</span><span class="sxs-lookup"><span data-stu-id="141e7-130">Request</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="141e7-131">プロトコル</span><span class="sxs-lookup"><span data-stu-id="141e7-131">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_contract"
}-->
```http
GET https://graph.microsoft.com/beta/contracts/{id}
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="141e7-132">C#</span><span class="sxs-lookup"><span data-stu-id="141e7-132">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-contract-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="141e7-133">Javascript</span><span class="sxs-lookup"><span data-stu-id="141e7-133">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-contract-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="141e7-134">目的-C</span><span class="sxs-lookup"><span data-stu-id="141e7-134">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-contract-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="141e7-135">応答</span><span class="sxs-lookup"><span data-stu-id="141e7-135">Response</span></span>
<span data-ttu-id="141e7-p103">注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="141e7-p103">Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.Contract"
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

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Get Contract",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
