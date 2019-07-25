---
title: '同期スキーマ: filterOperators'
description: スコープフィルターでサポートされているすべての演算子を一覧表示します。
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
ms.openlocfilehash: ba5616cd767ff48d0b1d14e2ddf6db9d0c3d1959
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/25/2019
ms.locfileid: "35869221"
---
# <a name="synchronizationschema-filteroperators"></a><span data-ttu-id="0fe1d-103">同期スキーマ: filterOperators</span><span class="sxs-lookup"><span data-stu-id="0fe1d-103">synchronizationSchema: filterOperators</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="0fe1d-104">[スコープフィルター](../resources/synchronization-filter.md)でサポートされているすべての演算子を一覧表示します。</span><span class="sxs-lookup"><span data-stu-id="0fe1d-104">List all operators supported in the [scoping filters](../resources/synchronization-filter.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="0fe1d-105">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="0fe1d-105">Permissions</span></span>
<span data-ttu-id="0fe1d-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="0fe1d-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="0fe1d-108">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="0fe1d-108">Permission type</span></span>                        | <span data-ttu-id="0fe1d-109">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="0fe1d-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="0fe1d-110">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="0fe1d-110">Delegated (work or school account)</span></span>     |<span data-ttu-id="0fe1d-111">Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="0fe1d-111">Directory.ReadWrite.All</span></span>  |
|<span data-ttu-id="0fe1d-112">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="0fe1d-112">Delegated (personal Microsoft account)</span></span> |<span data-ttu-id="0fe1d-113">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="0fe1d-113">Not supported.</span></span>|
|<span data-ttu-id="0fe1d-114">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="0fe1d-114">Application</span></span>                            |<span data-ttu-id="0fe1d-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="0fe1d-115">Not supported.</span></span> | 

## <a name="http-request"></a><span data-ttu-id="0fe1d-116">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="0fe1d-116">HTTP Request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /servicePrincipals/{id}/synchronization/jobs/{jobId}/schema/filterOperators
GET /servicePrincipals/{id}/synchronization/templates/{templateId}/schema/filterOperators
GET /applications/{id}/synchronization/templates/{templateId}/schema/filterOperators
```

## <a name="request-headers"></a><span data-ttu-id="0fe1d-117">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="0fe1d-117">Request headers</span></span>

| <span data-ttu-id="0fe1d-118">名前</span><span class="sxs-lookup"><span data-stu-id="0fe1d-118">Name</span></span>           | <span data-ttu-id="0fe1d-119">型</span><span class="sxs-lookup"><span data-stu-id="0fe1d-119">Type</span></span>    | <span data-ttu-id="0fe1d-120">説明</span><span class="sxs-lookup"><span data-stu-id="0fe1d-120">Description</span></span>|
|:---------------|:--------|:-----------|
| <span data-ttu-id="0fe1d-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="0fe1d-121">Authorization</span></span>  | <span data-ttu-id="0fe1d-122">string</span><span class="sxs-lookup"><span data-stu-id="0fe1d-122">string</span></span>  | <span data-ttu-id="0fe1d-p102">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="0fe1d-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="0fe1d-125">要求本文</span><span class="sxs-lookup"><span data-stu-id="0fe1d-125">Request body</span></span>

<span data-ttu-id="0fe1d-126">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="0fe1d-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="0fe1d-127">応答</span><span class="sxs-lookup"><span data-stu-id="0fe1d-127">Response</span></span>

<span data-ttu-id="0fe1d-128">成功した場合、このメソッド`200, OK`は応答コードと、応答本文で[filter演算子スキーマ](../resources/synchronization-filteroperatorschema.md)コレクションオブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="0fe1d-128">If successful, this method returns a `200, OK` response code and a [filterOperatorSchema](../resources/synchronization-filteroperatorschema.md) collection object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="0fe1d-129">例</span><span class="sxs-lookup"><span data-stu-id="0fe1d-129">Example</span></span>

##### <a name="request"></a><span data-ttu-id="0fe1d-130">要求</span><span class="sxs-lookup"><span data-stu-id="0fe1d-130">Request</span></span>
<span data-ttu-id="0fe1d-131">要求の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="0fe1d-131">The following is an example of a request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="0fe1d-132">プロトコル</span><span class="sxs-lookup"><span data-stu-id="0fe1d-132">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "synchronizationschema_filteroperators"
}-->
```http
GET https://graph.microsoft.com/beta/servicePrincipals/{id}/synchronization/jobs/{jobId}/schema/filterOperators
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="0fe1d-133">C#</span><span class="sxs-lookup"><span data-stu-id="0fe1d-133">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/synchronizationschema-filteroperators-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="0fe1d-134">Javascript</span><span class="sxs-lookup"><span data-stu-id="0fe1d-134">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/synchronizationschema-filteroperators-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="0fe1d-135">目的-C</span><span class="sxs-lookup"><span data-stu-id="0fe1d-135">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/synchronizationschema-filteroperators-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="0fe1d-136">Java</span><span class="sxs-lookup"><span data-stu-id="0fe1d-136">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/synchronizationschema-filteroperators-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="0fe1d-137">応答</span><span class="sxs-lookup"><span data-stu-id="0fe1d-137">Response</span></span>
<span data-ttu-id="0fe1d-138">応答の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="0fe1d-138">The following is an example of a response.</span></span>

><span data-ttu-id="0fe1d-139">**注:** ここに示す応答オブジェクトは、読みやすさのために短縮されている場合があります。</span><span class="sxs-lookup"><span data-stu-id="0fe1d-139">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="0fe1d-140">実際の呼び出しでは、すべてのプロパティが返されます。</span><span class="sxs-lookup"><span data-stu-id="0fe1d-140">All the properties will be returned in an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.filterOperatorSchema",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "value": [
        {
            "name": "EQUALS",
            "arity": "Binary",
            "multivaluedComparisonType": "All",
            "supportedAttributeTypes": [
                "String",
                "Integer"
            ]
        }
    ]
}
```
<!--
Below is the full response, which had to be redacted above as Markdown Scanner tool trips over "type" values containing 
non-string type names like "Integer" or "Boolean"

{
    "value": [
        {
            "name": "EQUALS",
            "arity": "Binary",
            "multivaluedComparisonType": "All",
            "supportedAttributeTypes": [
                "Integer",
                "String"
            ]
        },
        {
            "name": "IS FALSE",
            "arity": "Unary",
            "multivaluedComparisonType": "All",
            "supportedAttributeTypes": [
                "Boolean"
            ]
        },
        {
            "name": "IS NOT NULL",
            "arity": "Unary",
            "multivaluedComparisonType": "All",
            "supportedAttributeTypes": [
                "Integer",
                "String",
                "Binary",
                "Boolean"
            ]
        },
        {
            "name": "IS NULL",
            "arity": "Unary",
            "multivaluedComparisonType": "All",
            "supportedAttributeTypes": [
                "Integer",
                "String",
                "Binary",
                "Boolean"
            ]
        },
        {
            "name": "IS TRUE",
            "arity": "Unary",
            "multivaluedComparisonType": "All",
            "supportedAttributeTypes": [
                "Boolean"
            ]
        },
        {
            "name": "NOT EQUALS",
            "arity": "Binary",
            "multivaluedComparisonType": "All",
            "supportedAttributeTypes": [
                "Integer",
                "String"
            ]
        },
        {
            "name": "NOT REGEX MATCH",
            "arity": "Binary",
            "multivaluedComparisonType": "All",
            "supportedAttributeTypes": [
                "Integer",
                "String"
            ]
        },
        {
            "name": "REGEX MATCH",
            "arity": "Binary",
            "multivaluedComparisonType": "All",
            "supportedAttributeTypes": [
                "Integer",
                "String"
            ]
        }
    ]
}
-->
<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "synchronizationSchema: filterOperators",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: synchronizationschema_filteroperators/container/arity:\r\n       Expected type String but actual was Binary. Property: arity, actual value: 'Binary'"
  ]
}
-->
