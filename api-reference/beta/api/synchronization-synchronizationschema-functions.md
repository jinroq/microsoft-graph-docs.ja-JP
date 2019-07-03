---
title: '同期スキーマ: 関数'
description: AttributeMappingSource で現在サポートされているすべての関数を一覧表示します。
localization_priority: Normal
ms.openlocfilehash: a9967f1d3a6d68c847596f1e1ece2224ba0242fc
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/02/2019
ms.locfileid: "35458158"
---
# <a name="synchronizationschema-functions"></a><span data-ttu-id="131af-103">同期スキーマ: 関数</span><span class="sxs-lookup"><span data-stu-id="131af-103">synchronizationSchema: functions</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="131af-104">[AttributeMappingSource](../resources/synchronization-attributemappingsource.md)で現在サポートされているすべての関数を一覧表示します。</span><span class="sxs-lookup"><span data-stu-id="131af-104">List all the functions currently supported in the [attributeMappingSource](../resources/synchronization-attributemappingsource.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="131af-105">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="131af-105">Permissions</span></span>
<span data-ttu-id="131af-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="131af-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="131af-108">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="131af-108">Permission type</span></span>                        | <span data-ttu-id="131af-109">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="131af-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="131af-110">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="131af-110">Delegated (work or school account)</span></span>     |<span data-ttu-id="131af-111">Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="131af-111">Directory.ReadWrite.All</span></span>  |
|<span data-ttu-id="131af-112">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="131af-112">Delegated (personal Microsoft account)</span></span> |<span data-ttu-id="131af-113">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="131af-113">Not supported.</span></span>|
|<span data-ttu-id="131af-114">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="131af-114">Application</span></span>                            |<span data-ttu-id="131af-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="131af-115">Not supported.</span></span> | 

## <a name="http-request"></a><span data-ttu-id="131af-116">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="131af-116">HTTP Request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /servicePrincipals/{id}/synchronization/jobs/{jobId}/schema/functions
GET /servicePrincipals/{id}/synchronization/templates/{templateId}/schema/functions
GET /applications/{id}/synchronization/templates/{templateId}/schema/functions
```

## <a name="request-headers"></a><span data-ttu-id="131af-117">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="131af-117">Request headers</span></span>

| <span data-ttu-id="131af-118">名前</span><span class="sxs-lookup"><span data-stu-id="131af-118">Name</span></span>           | <span data-ttu-id="131af-119">型</span><span class="sxs-lookup"><span data-stu-id="131af-119">Type</span></span>    | <span data-ttu-id="131af-120">説明</span><span class="sxs-lookup"><span data-stu-id="131af-120">Description</span></span>|
|:---------------|:--------|:-----------|
| <span data-ttu-id="131af-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="131af-121">Authorization</span></span>  | <span data-ttu-id="131af-122">string</span><span class="sxs-lookup"><span data-stu-id="131af-122">string</span></span>  | <span data-ttu-id="131af-p102">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="131af-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="131af-125">要求本文</span><span class="sxs-lookup"><span data-stu-id="131af-125">Request body</span></span>

<span data-ttu-id="131af-126">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="131af-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="131af-127">応答</span><span class="sxs-lookup"><span data-stu-id="131af-127">Response</span></span>

<span data-ttu-id="131af-128">成功した場合、このメソッド`200 OK`は応答コードと、応答本文で[attributemappingFunctionSchema](../resources/synchronization-attributemappingfunctionschema.md)オブジェクトのコレクションを返します。</span><span class="sxs-lookup"><span data-stu-id="131af-128">If successful, this method returns a `200 OK` response code and a collection of [attributemappingFunctionSchema](../resources/synchronization-attributemappingfunctionschema.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="131af-129">例</span><span class="sxs-lookup"><span data-stu-id="131af-129">Example</span></span>

##### <a name="request"></a><span data-ttu-id="131af-130">要求</span><span class="sxs-lookup"><span data-stu-id="131af-130">Request</span></span>
<span data-ttu-id="131af-131">要求の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="131af-131">The following is an example of a request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="131af-132">プロトコル</span><span class="sxs-lookup"><span data-stu-id="131af-132">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "synchronizationschema_functions"
}-->
```http
GET https://graph.microsoft.com/beta/servicePrincipals/{id}/synchronization/jobs/{jobId}/schema/functions
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="131af-133">C#</span><span class="sxs-lookup"><span data-stu-id="131af-133">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/synchronizationschema-functions-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="131af-134">Javascript</span><span class="sxs-lookup"><span data-stu-id="131af-134">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/synchronizationschema-functions-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="131af-135">目的-C</span><span class="sxs-lookup"><span data-stu-id="131af-135">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/synchronizationschema-functions-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="131af-136">応答</span><span class="sxs-lookup"><span data-stu-id="131af-136">Response</span></span>
<span data-ttu-id="131af-137">応答の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="131af-137">The following is an example of a response.</span></span>

><span data-ttu-id="131af-138">**注:** ここに示す応答オブジェクトは、読みやすさのために短縮されている場合があります。</span><span class="sxs-lookup"><span data-stu-id="131af-138">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="131af-139">実際の呼び出しでは、すべてのプロパティが返されます。</span><span class="sxs-lookup"><span data-stu-id="131af-139">All the properties will be returned in an actual call.</span></span>

<!--
{
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.attributeMappingFunctionSchema",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#functions",
    "value": [
        {
            "name": "Append",
            "parameters": [
                {
                    "allowMultipleOccurrences": false,
                    "name": "source",
                    "required": true,
                    "type": "String"
                },
                {
                    "allowMultipleOccurrences": false,
                    "name": "suffix",
                    "required": true,
                    "type": "String"
                }
            ]
        },
        {
            "name": "DefaultDomain",
            "parameters": []
        },
        {
            "name": "AppRoleAssignments",
            "parameters": [
                {
                    "allowMultipleOccurrences": false,
                    "name": "source",
                    "required": true,
                    "type": "String"
                }
            ]
        },
        {
            "name": "FormatDateTime",
            "parameters": [
                {
                    "allowMultipleOccurrences": false,
                    "name": "source",
                    "required": true,
                    "type": "String"
                },
                {
                    "allowMultipleOccurrences": false,
                    "name": "inputFormat",
                    "required": true,
                    "type": "String"
                },
                {
                    "allowMultipleOccurrences": false,
                    "name": "outputFormat",
                    "required": true,
                    "type": "String"
                }
            ]
        }
    ]
}
```

<!--
Below is the full response, which had to be redacted above as Markdown Scanner tool trips over "type" values containing 
non-string type names like "Integer" or "Boolean"

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#functions",
    "value": [
        {
            "name": "Append",
            "parameters": [
                {
                    "allowMultipleOccurrences": false,
                    "name": "source",
                    "required": true,
                    "type": "String"
                },
                {
                    "allowMultipleOccurrences": false,
                    "name": "suffix",
                    "required": true,
                    "type": "String"
                }
            ]
        },
        {
            "name": "DefaultDomain",
            "parameters": []
        },
        {
            "name": "AppRoleAssignments",
            "parameters": [
                {
                    "allowMultipleOccurrences": false,
                    "name": "source",
                    "required": true,
                    "type": "String"
                }
            ]
        },
        {
            "name": "FormatDateTime",
            "parameters": [
                {
                    "allowMultipleOccurrences": false,
                    "name": "source",
                    "required": true,
                    "type": "String"
                },
                {
                    "allowMultipleOccurrences": false,
                    "name": "inputFormat",
                    "required": true,
                    "type": "String"
                },
                {
                    "allowMultipleOccurrences": false,
                    "name": "outputFormat",
                    "required": true,
                    "type": "String"
                }
            ]
        },
        {
            "name": "IsNothing",
            "parameters": [
                {
                    "allowMultipleOccurrences": false,
                    "name": "source",
                    "required": true,
                    "type": "Boolean"
                }
            ]
        },
        {
            "name": "Join",
            "parameters": [
                {
                    "allowMultipleOccurrences": false,
                    "name": "separator",
                    "required": true,
                    "type": "String"
                },
                {
                    "allowMultipleOccurrences": true,
                    "name": "source",
                    "required": true,
                    "type": "String"
                }
            ]
        },
        {
            "name": "Prepend",
            "parameters": [
                {
                    "allowMultipleOccurrences": false,
                    "name": "prefix",
                    "required": true,
                    "type": "String"
                },
                {
                    "allowMultipleOccurrences": false,
                    "name": "source",
                    "required": true,
                    "type": "String"
                }
            ]
        },
        {
            "name": "Mid",
            "parameters": [
                {
                    "allowMultipleOccurrences": false,
                    "name": "source",
                    "required": true,
                    "type": "String"
                },
                {
                    "allowMultipleOccurrences": false,
                    "name": "start",
                    "required": true,
                    "type": "Integer"
                },
                {
                    "allowMultipleOccurrences": false,
                    "name": "length",
                    "required": true,
                    "type": "Integer"
                }
            ]
        },
        {
            "name": "Not",
            "parameters": [
                {
                    "allowMultipleOccurrences": false,
                    "name": "source",
                    "required": true,
                    "type": "Boolean"
                }
            ]
        },
        {
            "name": "Replace",
            "parameters": [
                {
                    "allowMultipleOccurrences": false,
                    "name": "source",
                    "required": true,
                    "type": "String"
                },
                {
                    "allowMultipleOccurrences": false,
                    "name": "Find",
                    "required": false,
                    "type": "String"
                },
                {
                    "allowMultipleOccurrences": false,
                    "name": "RegularExpression",
                    "required": false,
                    "type": "String"
                },
                {
                    "allowMultipleOccurrences": false,
                    "name": "RegularExpressionGroupName",
                    "required": false,
                    "type": "String"
                },
                {
                    "allowMultipleOccurrences": false,
                    "name": "Replacement",
                    "required": false,
                    "type": "String"
                },
                {
                    "allowMultipleOccurrences": false,
                    "name": "ReplacementPropertyName",
                    "required": false,
                    "type": "String"
                },
                {
                    "allowMultipleOccurrences": false,
                    "name": "Template",
                    "required": false,
                    "type": "String"
                }
            ]
        },
        {
            "name": "SingleAppRoleAssignment",
            "parameters": [
                {
                    "allowMultipleOccurrences": false,
                    "name": "source",
                    "required": true,
                    "type": "String"
                }
            ]
        },
        {
            "name": "Split",
            "parameters": [
                {
                    "allowMultipleOccurrences": false,
                    "name": "source",
                    "required": true,
                    "type": "String"
                },
                {
                    "allowMultipleOccurrences": false,
                    "name": "delimiter",
                    "required": false,
                    "type": "String"
                }
            ]
        },
        {
            "name": "StripSpaces",
            "parameters": [
                {
                    "allowMultipleOccurrences": false,
                    "name": "source",
                    "required": true,
                    "type": "String"
                }
            ]
        },
        {
            "name": "Switch",
            "parameters": [
                {
                    "allowMultipleOccurrences": false,
                    "name": "source",
                    "required": true,
                    "type": "String"
                },
                {
                    "allowMultipleOccurrences": false,
                    "name": "defaultValue",
                    "required": false,
                    "type": "String"
                },
                {
                    "allowMultipleOccurrences": true,
                    "name": "switchValue",
                    "required": false,
                    "type": "String"
                }
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
  "description": "synchronizationSchema: functions",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
