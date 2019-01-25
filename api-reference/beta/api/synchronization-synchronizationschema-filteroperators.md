---
title: 'synchronizationSchema: filterOperators'
description: スコープ フィルターでサポートされているすべての演算子の一覧を表示します。
localization_priority: Normal
ms.openlocfilehash: 68e0c9f583e92989213d1442aee1610b1495bae0
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/24/2019
ms.locfileid: "29516470"
---
# <a name="synchronizationschema-filteroperators"></a><span data-ttu-id="e747a-103">synchronizationSchema: filterOperators</span><span class="sxs-lookup"><span data-stu-id="e747a-103">synchronizationSchema: filterOperators</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="e747a-104">[スコープ フィルター](../resources/synchronization-filter.md)でサポートされているすべての演算子の一覧を表示します。</span><span class="sxs-lookup"><span data-stu-id="e747a-104">List all operators supported in the [scoping filters](../resources/synchronization-filter.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="e747a-105">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="e747a-105">Permissions</span></span>
<span data-ttu-id="e747a-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="e747a-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e747a-108">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="e747a-108">Permission type</span></span>                        | <span data-ttu-id="e747a-109">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="e747a-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="e747a-110">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="e747a-110">Delegated (work or school account)</span></span>     |<span data-ttu-id="e747a-111">Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e747a-111">Directory.ReadWrite.All</span></span>  |
|<span data-ttu-id="e747a-112">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="e747a-112">Delegated (personal Microsoft account)</span></span> |<span data-ttu-id="e747a-113">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="e747a-113">Not supported.</span></span>|
|<span data-ttu-id="e747a-114">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="e747a-114">Application</span></span>                            |<span data-ttu-id="e747a-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="e747a-115">Not supported.</span></span> | 

## <a name="http-request"></a><span data-ttu-id="e747a-116">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="e747a-116">HTTP Request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /servicePrincipals/{id}/synchronization/jobs/{jobId}/schema/filterOperators
GET /servicePrincipals/{id}/synchronization/templates/{templateId}/schema/filterOperators
GET /applications/{id}/synchronization/templates/{templateId}/schema/filterOperators
```

## <a name="request-headers"></a><span data-ttu-id="e747a-117">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="e747a-117">Request headers</span></span>

| <span data-ttu-id="e747a-118">名前</span><span class="sxs-lookup"><span data-stu-id="e747a-118">Name</span></span>           | <span data-ttu-id="e747a-119">型</span><span class="sxs-lookup"><span data-stu-id="e747a-119">Type</span></span>    | <span data-ttu-id="e747a-120">説明</span><span class="sxs-lookup"><span data-stu-id="e747a-120">Description</span></span>|
|:---------------|:--------|:-----------|
| <span data-ttu-id="e747a-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="e747a-121">Authorization</span></span>  | <span data-ttu-id="e747a-122">string</span><span class="sxs-lookup"><span data-stu-id="e747a-122">string</span></span>  | <span data-ttu-id="e747a-p102">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="e747a-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="e747a-125">要求本文</span><span class="sxs-lookup"><span data-stu-id="e747a-125">Request body</span></span>

<span data-ttu-id="e747a-126">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="e747a-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="e747a-127">応答</span><span class="sxs-lookup"><span data-stu-id="e747a-127">Response</span></span>

<span data-ttu-id="e747a-128">かどうかは成功すると、このメソッドが返されます、`200, OK`応答コードおよび応答の本文の[filterOperatorSchema](../resources/synchronization-filteroperatorschema.md)コレクション オブジェクトです。</span><span class="sxs-lookup"><span data-stu-id="e747a-128">If successful, this method returns a `200, OK` response code and a [filterOperatorSchema](../resources/synchronization-filteroperatorschema.md) collection object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="e747a-129">例</span><span class="sxs-lookup"><span data-stu-id="e747a-129">Example</span></span>

##### <a name="request"></a><span data-ttu-id="e747a-130">要求</span><span class="sxs-lookup"><span data-stu-id="e747a-130">Request</span></span>
<span data-ttu-id="e747a-131">要求の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="e747a-131">The following is an example of a request.</span></span>
<!-- {
  "blockType": "request",
  "name": "synchronizationschema_filteroperators"
}-->
```http
GET https://graph.microsoft.com/beta/servicePrincipals/{id}/synchronization/jobs/{jobId}/schema/filterOperators
```

##### <a name="response"></a><span data-ttu-id="e747a-132">応答</span><span class="sxs-lookup"><span data-stu-id="e747a-132">Response</span></span>
<span data-ttu-id="e747a-133">応答の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="e747a-133">The following is an example of a response.</span></span>

><span data-ttu-id="e747a-134">**注:** ここに示す応答オブジェクトは、読みやすさのために短縮されている場合があります。</span><span class="sxs-lookup"><span data-stu-id="e747a-134">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="e747a-135">すべてのプロパティは、実際の呼び出しで返されます。</span><span class="sxs-lookup"><span data-stu-id="e747a-135">All the properties will be returned in an actual call.</span></span>

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
    "Error: /api-reference/beta/api/synchronization-synchronizationschema-filteroperators.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
