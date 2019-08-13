---
title: 契約書を一覧表示する
description: パートナーテナントに関連付けられている契約オブジェクトの一覧を取得します。
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 180ba5881879c57c2a4a51deed9b6ccc32920528
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/13/2019
ms.locfileid: "36319775"
---
# <a name="list-contracts"></a><span data-ttu-id="3b3f0-103">契約書を一覧表示する</span><span class="sxs-lookup"><span data-stu-id="3b3f0-103">List contracts</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="3b3f0-104">パートナーテナントに関連付けられている[契約](../resources/contract.md)オブジェクトの一覧を取得します。</span><span class="sxs-lookup"><span data-stu-id="3b3f0-104">Retrieve a list of [contract](../resources/contract.md) objects associated to a partner tenant.</span></span>

## <a name="permissions"></a><span data-ttu-id="3b3f0-105">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="3b3f0-105">Permissions</span></span>

<span data-ttu-id="3b3f0-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="3b3f0-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="3b3f0-108">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="3b3f0-108">Permission type</span></span>      | <span data-ttu-id="3b3f0-109">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="3b3f0-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="3b3f0-110">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="3b3f0-110">Delegated (work or school account)</span></span> | <span data-ttu-id="3b3f0-111">Directory.Read.All、Directory.ReadWrite.All、Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="3b3f0-111">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="3b3f0-112">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="3b3f0-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="3b3f0-113">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="3b3f0-113">Not supported.</span></span>    |
|<span data-ttu-id="3b3f0-114">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="3b3f0-114">Application</span></span> | <span data-ttu-id="3b3f0-115">Directory.Read.All、Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="3b3f0-115">Directory.Read.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="3b3f0-116">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="3b3f0-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->

```http
GET /contracts
```

## <a name="optional-query-parameters"></a><span data-ttu-id="3b3f0-117">オプションのクエリ パラメーター</span><span class="sxs-lookup"><span data-stu-id="3b3f0-117">Optional query parameters</span></span>

<span data-ttu-id="3b3f0-118">このメソッドは、応答をカスタマイズするための [OData クエリ パラメーター](https://developer.microsoft.com/graph/docs/concepts/query_parameters)をサポートします。</span><span class="sxs-lookup"><span data-stu-id="3b3f0-118">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span> 

> <span data-ttu-id="3b3f0-119">フィルター処理は、customerId、defaultDomainName、および displayName でサポートされています。</span><span class="sxs-lookup"><span data-stu-id="3b3f0-119">Filtering is supported for customerId, defaultDomainName, and displayName.</span></span>

## <a name="request-headers"></a><span data-ttu-id="3b3f0-120">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="3b3f0-120">Request headers</span></span>

| <span data-ttu-id="3b3f0-121">名前</span><span class="sxs-lookup"><span data-stu-id="3b3f0-121">Name</span></span>      |<span data-ttu-id="3b3f0-122">説明</span><span class="sxs-lookup"><span data-stu-id="3b3f0-122">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="3b3f0-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="3b3f0-123">Authorization</span></span>  | <span data-ttu-id="3b3f0-p102">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="3b3f0-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="3b3f0-126">要求本文</span><span class="sxs-lookup"><span data-stu-id="3b3f0-126">Request body</span></span>

<span data-ttu-id="3b3f0-127">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="3b3f0-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="3b3f0-128">応答</span><span class="sxs-lookup"><span data-stu-id="3b3f0-128">Response</span></span>

<span data-ttu-id="3b3f0-129">成功した場合、このメソッド`200 OK`は応答コードと、応答本文で[Contract](../resources/contract.md)オブジェクトのコレクションを返します。</span><span class="sxs-lookup"><span data-stu-id="3b3f0-129">If successful, this method returns a `200 OK` response code and a collection of [Contract](../resources/contract.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="3b3f0-130">例</span><span class="sxs-lookup"><span data-stu-id="3b3f0-130">Example</span></span>
##### <a name="request"></a><span data-ttu-id="3b3f0-131">要求</span><span class="sxs-lookup"><span data-stu-id="3b3f0-131">Request</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="3b3f0-132">プロトコル</span><span class="sxs-lookup"><span data-stu-id="3b3f0-132">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_contract"
}-->
```http
GET https://graph.microsoft.com/beta/contracts
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="3b3f0-133">C#</span><span class="sxs-lookup"><span data-stu-id="3b3f0-133">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-contract-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="3b3f0-134">JavaScript</span><span class="sxs-lookup"><span data-stu-id="3b3f0-134">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-contract-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="3b3f0-135">目的-C</span><span class="sxs-lookup"><span data-stu-id="3b3f0-135">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-contract-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="3b3f0-136">Java</span><span class="sxs-lookup"><span data-stu-id="3b3f0-136">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-contract-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="3b3f0-137">応答</span><span class="sxs-lookup"><span data-stu-id="3b3f0-137">Response</span></span>

<span data-ttu-id="3b3f0-p103">注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="3b3f0-p103">Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.Contract",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "value": [
    {
      "contractType": "contractType-value",
      "customerId": "customerId-value",
      "defaultDomainName": "defaultDomainName-value",
      "displayName": "displayName-value",
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
  "description": "Get Contract",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
