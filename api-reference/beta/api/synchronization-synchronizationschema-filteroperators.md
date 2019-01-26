---
title: 'synchronizationSchema: filterOperators'
description: スコープ フィルターでサポートされているすべての演算子の一覧を表示します。
localization_priority: Normal
ms.openlocfilehash: c564142aa6a26b3f83fa5f82036e3b97dc13e672
ms.sourcegitcommit: 66066b71d353fd7c2481d43b1dba2c33390eee61
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/26/2019
ms.locfileid: "29573229"
---
# <a name="synchronizationschema-filteroperators"></a><span data-ttu-id="028da-103">synchronizationSchema: filterOperators</span><span class="sxs-lookup"><span data-stu-id="028da-103">synchronizationSchema: filterOperators</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="028da-104">[スコープ フィルター](../resources/synchronization-filter.md)でサポートされているすべての演算子の一覧を表示します。</span><span class="sxs-lookup"><span data-stu-id="028da-104">List all operators supported in the [scoping filters](../resources/synchronization-filter.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="028da-105">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="028da-105">Permissions</span></span>
<span data-ttu-id="028da-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="028da-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="028da-108">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="028da-108">Permission type</span></span>                        | <span data-ttu-id="028da-109">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="028da-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="028da-110">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="028da-110">Delegated (work or school account)</span></span>     |<span data-ttu-id="028da-111">Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="028da-111">Directory.ReadWrite.All</span></span>  |
|<span data-ttu-id="028da-112">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="028da-112">Delegated (personal Microsoft account)</span></span> |<span data-ttu-id="028da-113">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="028da-113">Not supported.</span></span>|
|<span data-ttu-id="028da-114">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="028da-114">Application</span></span>                            |<span data-ttu-id="028da-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="028da-115">Not supported.</span></span> | 

## <a name="http-request"></a><span data-ttu-id="028da-116">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="028da-116">HTTP Request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /servicePrincipals/{id}/synchronization/jobs/{jobId}/schema/filterOperators
GET /servicePrincipals/{id}/synchronization/templates/{templateId}/schema/filterOperators
GET /applications/{id}/synchronization/templates/{templateId}/schema/filterOperators
```

## <a name="request-headers"></a><span data-ttu-id="028da-117">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="028da-117">Request headers</span></span>

| <span data-ttu-id="028da-118">名前</span><span class="sxs-lookup"><span data-stu-id="028da-118">Name</span></span>           | <span data-ttu-id="028da-119">型</span><span class="sxs-lookup"><span data-stu-id="028da-119">Type</span></span>    | <span data-ttu-id="028da-120">説明</span><span class="sxs-lookup"><span data-stu-id="028da-120">Description</span></span>|
|:---------------|:--------|:-----------|
| <span data-ttu-id="028da-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="028da-121">Authorization</span></span>  | <span data-ttu-id="028da-122">string</span><span class="sxs-lookup"><span data-stu-id="028da-122">string</span></span>  | <span data-ttu-id="028da-p102">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="028da-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="028da-125">要求本文</span><span class="sxs-lookup"><span data-stu-id="028da-125">Request body</span></span>

<span data-ttu-id="028da-126">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="028da-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="028da-127">応答</span><span class="sxs-lookup"><span data-stu-id="028da-127">Response</span></span>

<span data-ttu-id="028da-128">かどうかは成功すると、このメソッドが返されます、`200, OK`応答コードおよび応答の本文の[filterOperatorSchema](../resources/synchronization-filteroperatorschema.md)コレクション オブジェクトです。</span><span class="sxs-lookup"><span data-stu-id="028da-128">If successful, this method returns a `200, OK` response code and a [filterOperatorSchema](../resources/synchronization-filteroperatorschema.md) collection object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="028da-129">例</span><span class="sxs-lookup"><span data-stu-id="028da-129">Example</span></span>

##### <a name="request"></a><span data-ttu-id="028da-130">要求</span><span class="sxs-lookup"><span data-stu-id="028da-130">Request</span></span>
<span data-ttu-id="028da-131">要求の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="028da-131">The following is an example of a request.</span></span>
<!-- {
  "blockType": "request",
  "name": "synchronizationschema_filteroperators"
}-->
```http
GET https://graph.microsoft.com/beta/servicePrincipals/{id}/synchronization/jobs/{jobId}/schema/filterOperators
```

##### <a name="response"></a><span data-ttu-id="028da-132">応答</span><span class="sxs-lookup"><span data-stu-id="028da-132">Response</span></span>
<span data-ttu-id="028da-133">応答の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="028da-133">The following is an example of a response.</span></span>

><span data-ttu-id="028da-134">**注:** ここに示す応答オブジェクトは、読みやすさのために短縮されている場合があります。</span><span class="sxs-lookup"><span data-stu-id="028da-134">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="028da-135">すべてのプロパティは、実際の呼び出しで返されます。</span><span class="sxs-lookup"><span data-stu-id="028da-135">All the properties will be returned in an actual call.</span></span>

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
            "arity": "Unary",
            "multivaluedComparisonType": "All",
            "supportedAttributeTypes": [                
                "@string"
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
               "Boolean"
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
                "Boolean"
            ]
        },
        {
            "name": "IS NULL",
            "arity": "Unary",
            "multivaluedComparisonType": "All",
            "supportedAttributeTypes": [
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
                "Boolean"
            ]
        },
        {
            "name": "NOT REGEX MATCH",
            "arity": "Binary",
            "multivaluedComparisonType": "All",
            "supportedAttributeTypes": [
                "Boolean"
            ]
        },
        {
            "name": "REGEX MATCH",
            "arity": "Binary",
            "multivaluedComparisonType": "All",
            "supportedAttributeTypes": [
                "Boolean"
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
