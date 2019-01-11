---
title: 'synchronizationSchema: 関数'
description: 現在、attributeMappingSource でサポートされているすべての関数の一覧を表示します。
localization_priority: Normal
ms.openlocfilehash: 5dc7734e9d747ac1e832aebb7d9c7355c2fbb52f
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/11/2019
ms.locfileid: "27841008"
---
# <a name="synchronizationschema-functions"></a><span data-ttu-id="8101f-103">synchronizationSchema: 関数</span><span class="sxs-lookup"><span data-stu-id="8101f-103">synchronizationSchema: functions</span></span>

> <span data-ttu-id="8101f-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="8101f-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="8101f-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="8101f-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="8101f-106">[AttributeMappingSource](../resources/synchronization-attributemappingsource.md)で現在サポートされているすべての関数の一覧を表示します。</span><span class="sxs-lookup"><span data-stu-id="8101f-106">List all the functions currently supported in the [attributeMappingSource](../resources/synchronization-attributemappingsource.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="8101f-107">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="8101f-107">Permissions</span></span>
<span data-ttu-id="8101f-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="8101f-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="8101f-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="8101f-110">Permission type</span></span>                        | <span data-ttu-id="8101f-111">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="8101f-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="8101f-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="8101f-112">Delegated (work or school account)</span></span>     |<span data-ttu-id="8101f-113">Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8101f-113">Directory.ReadWrite.All</span></span>  |
|<span data-ttu-id="8101f-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="8101f-114">Delegated (personal Microsoft account)</span></span> |<span data-ttu-id="8101f-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="8101f-115">Not supported.</span></span>|
|<span data-ttu-id="8101f-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="8101f-116">Application</span></span>                            |<span data-ttu-id="8101f-117">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="8101f-117">Not supported.</span></span> | 

## <a name="http-request"></a><span data-ttu-id="8101f-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="8101f-118">HTTP Request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /servicePrincipals/{id}/synchronization/jobs/{jobId}/schema/functions
GET /servicePrincipals/{id}/synchronization/templates/{templateId}/schema/functions
GET /applications/{id}/synchronization/templates/{templateId}/schema/functions
```

## <a name="request-headers"></a><span data-ttu-id="8101f-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="8101f-119">Request headers</span></span>

| <span data-ttu-id="8101f-120">名前</span><span class="sxs-lookup"><span data-stu-id="8101f-120">Name</span></span>           | <span data-ttu-id="8101f-121">種類</span><span class="sxs-lookup"><span data-stu-id="8101f-121">Type</span></span>    | <span data-ttu-id="8101f-122">説明</span><span class="sxs-lookup"><span data-stu-id="8101f-122">Description</span></span>|
|:---------------|:--------|:-----------|
| <span data-ttu-id="8101f-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="8101f-123">Authorization</span></span>  | <span data-ttu-id="8101f-124">string</span><span class="sxs-lookup"><span data-stu-id="8101f-124">string</span></span>  | <span data-ttu-id="8101f-p103">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="8101f-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="8101f-127">要求本文</span><span class="sxs-lookup"><span data-stu-id="8101f-127">Request body</span></span>

<span data-ttu-id="8101f-128">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="8101f-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="8101f-129">応答</span><span class="sxs-lookup"><span data-stu-id="8101f-129">Response</span></span>

<span data-ttu-id="8101f-130">かどうかは成功すると、このメソッドが返されます、`200 OK`応答コードおよび応答の本文に[attributemappingFunctionSchema](../resources/synchronization-attributemappingfunctionschema.md)オブジェクトのコレクションです。</span><span class="sxs-lookup"><span data-stu-id="8101f-130">If successful, this method returns a `200 OK` response code and a collection of [attributemappingFunctionSchema](../resources/synchronization-attributemappingfunctionschema.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="8101f-131">例</span><span class="sxs-lookup"><span data-stu-id="8101f-131">Example</span></span>

##### <a name="request"></a><span data-ttu-id="8101f-132">要求</span><span class="sxs-lookup"><span data-stu-id="8101f-132">Request</span></span>
<span data-ttu-id="8101f-133">要求の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="8101f-133">The following is an example of a request.</span></span>
<!-- {
  "blockType": "request",
  "name": "synchronizationschema_functions"
}-->
```http
GET https://graph.microsoft.com/beta/servicePrincipals/{id}/synchronization/jobs/{jobId}/schema/functions
```

##### <a name="response"></a><span data-ttu-id="8101f-134">応答</span><span class="sxs-lookup"><span data-stu-id="8101f-134">Response</span></span>
<span data-ttu-id="8101f-135">応答の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="8101f-135">The following is an example of a response.</span></span>

><span data-ttu-id="8101f-136">**注:** ここに示す応答オブジェクトは、読みやすさのために短縮されている場合があります。</span><span class="sxs-lookup"><span data-stu-id="8101f-136">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="8101f-137">すべてのプロパティは、実際の呼び出しで返されます。</span><span class="sxs-lookup"><span data-stu-id="8101f-137">All the properties will be returned in an actual call.</span></span>

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
<!-- {
  "type": "#page.annotation",
  "description": "synchronizationSchema: functions",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
