---
title: 'synchronizationSchema: filterOperators'
description: スコープ フィルターでサポートされているすべての演算子の一覧を表示します。
ms.openlocfilehash: 968abf6584868b2b0b5e664c59f14eebc780f151
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27069663"
---
# <a name="synchronizationschema-filteroperators"></a><span data-ttu-id="20287-103">synchronizationSchema: filterOperators</span><span class="sxs-lookup"><span data-stu-id="20287-103">synchronizationSchema: filterOperators</span></span>

> <span data-ttu-id="20287-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="20287-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="20287-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="20287-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="20287-106">[スコープ フィルター](../resources/synchronization-filter.md)でサポートされているすべての演算子の一覧を表示します。</span><span class="sxs-lookup"><span data-stu-id="20287-106">List all operators supported in the [scoping filters](../resources/synchronization-filter.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="20287-107">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="20287-107">Permissions</span></span>
<span data-ttu-id="20287-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="20287-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="20287-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="20287-110">Permission type</span></span>                        | <span data-ttu-id="20287-111">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="20287-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="20287-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="20287-112">Delegated (work or school account)</span></span>     |<span data-ttu-id="20287-113">Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="20287-113">Directory.ReadWrite.All</span></span>  |
|<span data-ttu-id="20287-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="20287-114">Delegated (personal Microsoft account)</span></span> |<span data-ttu-id="20287-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="20287-115">Not supported.</span></span>|
|<span data-ttu-id="20287-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="20287-116">Application</span></span>                            |<span data-ttu-id="20287-117">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="20287-117">Not supported.</span></span> | 

## <a name="http-request"></a><span data-ttu-id="20287-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="20287-118">HTTP Request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /servicePrincipals/{id}/synchronization/jobs/{jobId}/schema/filterOperators
GET /servicePrincipals/{id}/synchronization/templates/{templateId}/schema/filterOperators
GET /applications/{id}/synchronization/templates/{templateId}/schema/filterOperators
```

## <a name="request-headers"></a><span data-ttu-id="20287-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="20287-119">Request headers</span></span>

| <span data-ttu-id="20287-120">名前</span><span class="sxs-lookup"><span data-stu-id="20287-120">Name</span></span>           | <span data-ttu-id="20287-121">型</span><span class="sxs-lookup"><span data-stu-id="20287-121">Type</span></span>    | <span data-ttu-id="20287-122">説明</span><span class="sxs-lookup"><span data-stu-id="20287-122">Description</span></span>|
|:---------------|:--------|:-----------|
| <span data-ttu-id="20287-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="20287-123">Authorization</span></span>  | <span data-ttu-id="20287-124">string</span><span class="sxs-lookup"><span data-stu-id="20287-124">string</span></span>  | <span data-ttu-id="20287-p103">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="20287-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="20287-127">要求本文</span><span class="sxs-lookup"><span data-stu-id="20287-127">Request body</span></span>

<span data-ttu-id="20287-128">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="20287-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="20287-129">応答</span><span class="sxs-lookup"><span data-stu-id="20287-129">Response</span></span>

<span data-ttu-id="20287-130">かどうかは成功すると、このメソッドが返されます、`200, OK`応答コードおよび応答の本文の[filterOperatorSchema](../resources/synchronization-filteroperatorschema.md)コレクション オブジェクトです。</span><span class="sxs-lookup"><span data-stu-id="20287-130">If successful, this method returns a `200, OK` response code and a [filterOperatorSchema](../resources/synchronization-filteroperatorschema.md) collection object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="20287-131">例</span><span class="sxs-lookup"><span data-stu-id="20287-131">Example</span></span>

##### <a name="request"></a><span data-ttu-id="20287-132">要求</span><span class="sxs-lookup"><span data-stu-id="20287-132">Request</span></span>
<span data-ttu-id="20287-133">要求の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="20287-133">The following is an example of a request.</span></span>
<!-- {
  "blockType": "request",
  "name": "synchronizationschema_filteroperators"
}-->
```http
GET https://graph.microsoft.com/beta/servicePrincipals/{id}/synchronization/jobs/{jobId}/schema/filterOperators
```

##### <a name="response"></a><span data-ttu-id="20287-134">応答</span><span class="sxs-lookup"><span data-stu-id="20287-134">Response</span></span>
<span data-ttu-id="20287-135">応答の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="20287-135">The following is an example of a response.</span></span>

><span data-ttu-id="20287-136">**注:** ここに示す応答オブジェクトは、読みやすさのために短縮されている場合があります。</span><span class="sxs-lookup"><span data-stu-id="20287-136">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="20287-137">すべてのプロパティは、実際の呼び出しで返されます。</span><span class="sxs-lookup"><span data-stu-id="20287-137">All the properties will be returned in an actual call.</span></span>

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
<!-- {
  "type": "#page.annotation",
  "description": "synchronizationSchema: filterOperators",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->