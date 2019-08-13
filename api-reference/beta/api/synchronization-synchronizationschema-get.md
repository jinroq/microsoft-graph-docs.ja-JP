---
title: 同期スキーマを取得する
description: 指定された同期ジョブまたはテンプレートのスキーマを取得します。
localization_priority: Normal
doc_type: apiPageType
author: davidmu1
ms.prod: microsoft-identity-platform
ms.openlocfilehash: f5b656149b5e12c285a1c2c64b7f4aafeb2d39bb
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/13/2019
ms.locfileid: "36363488"
---
# <a name="get-synchronizationschema"></a><span data-ttu-id="10d48-103">同期スキーマを取得する</span><span class="sxs-lookup"><span data-stu-id="10d48-103">Get synchronizationSchema</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="10d48-104">指定された同期ジョブまたはテンプレートのスキーマを取得します。</span><span class="sxs-lookup"><span data-stu-id="10d48-104">Retrieve the schema for a given synchronization job or template.</span></span>

## <a name="permissions"></a><span data-ttu-id="10d48-105">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="10d48-105">Permissions</span></span>
<span data-ttu-id="10d48-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="10d48-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="10d48-108">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="10d48-108">Permission type</span></span>                        | <span data-ttu-id="10d48-109">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="10d48-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="10d48-110">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="10d48-110">Delegated (work or school account)</span></span>     |<span data-ttu-id="10d48-111">Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="10d48-111">Directory.ReadWrite.All</span></span>  |
|<span data-ttu-id="10d48-112">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="10d48-112">Delegated (personal Microsoft account)</span></span> |<span data-ttu-id="10d48-113">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="10d48-113">Not supported.</span></span> |
|<span data-ttu-id="10d48-114">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="10d48-114">Application</span></span>                            |<span data-ttu-id="10d48-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="10d48-115">Not supported.</span></span> | 

## <a name="http-request"></a><span data-ttu-id="10d48-116">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="10d48-116">HTTP Request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /servicePrincipals/{id}/synchronization/jobs/{jobId}/schema
GET /servicePrincipals/{id}/synchronization/templates/{templateId}/schema
GET /applications/{id}/synchronization/templates/{templateId}/schema
```

## <a name="request-headers"></a><span data-ttu-id="10d48-117">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="10d48-117">Request headers</span></span>

| <span data-ttu-id="10d48-118">名前</span><span class="sxs-lookup"><span data-stu-id="10d48-118">Name</span></span>           | <span data-ttu-id="10d48-119">型</span><span class="sxs-lookup"><span data-stu-id="10d48-119">Type</span></span>    | <span data-ttu-id="10d48-120">説明</span><span class="sxs-lookup"><span data-stu-id="10d48-120">Description</span></span>|
|:---------------|:--------|:-----------|
| <span data-ttu-id="10d48-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="10d48-121">Authorization</span></span>  | <span data-ttu-id="10d48-122">string</span><span class="sxs-lookup"><span data-stu-id="10d48-122">string</span></span>  | <span data-ttu-id="10d48-p102">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="10d48-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="10d48-125">要求本文</span><span class="sxs-lookup"><span data-stu-id="10d48-125">Request body</span></span>

<span data-ttu-id="10d48-126">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="10d48-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="10d48-127">応答</span><span class="sxs-lookup"><span data-stu-id="10d48-127">Response</span></span>

<span data-ttu-id="10d48-128">成功した場合、このメソッド`200 OK`は応答コードと、応答本文で[同期スキーマ](../resources/synchronization-synchronizationschema.md)オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="10d48-128">If successful, this method returns a `200 OK` response code and a [synchronizationSchema](../resources/synchronization-synchronizationschema.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="10d48-129">例</span><span class="sxs-lookup"><span data-stu-id="10d48-129">Example</span></span>

##### <a name="request"></a><span data-ttu-id="10d48-130">要求</span><span class="sxs-lookup"><span data-stu-id="10d48-130">Request</span></span>
<span data-ttu-id="10d48-131">要求の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="10d48-131">The following is an example of a request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="10d48-132">プロトコル</span><span class="sxs-lookup"><span data-stu-id="10d48-132">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_synchronizationschema"
}-->
```http
GET https://graph.microsoft.com/beta/servicePrincipals/{id}/synchronization/jobs/{jobId}/schema
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="10d48-133">C#</span><span class="sxs-lookup"><span data-stu-id="10d48-133">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-synchronizationschema-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="10d48-134">JavaScript</span><span class="sxs-lookup"><span data-stu-id="10d48-134">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-synchronizationschema-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="10d48-135">目的-C</span><span class="sxs-lookup"><span data-stu-id="10d48-135">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-synchronizationschema-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="10d48-136">Java</span><span class="sxs-lookup"><span data-stu-id="10d48-136">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-synchronizationschema-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="10d48-137">応答</span><span class="sxs-lookup"><span data-stu-id="10d48-137">Response</span></span>
<span data-ttu-id="10d48-138">応答の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="10d48-138">The following is an example of a response.</span></span>

><span data-ttu-id="10d48-139">**注:** ここに示す応答オブジェクトは、読みやすさのために短縮されている場合があります。</span><span class="sxs-lookup"><span data-stu-id="10d48-139">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="10d48-140">実際の呼び出しでは、すべてのプロパティが返されます。</span><span class="sxs-lookup"><span data-stu-id="10d48-140">All the properties will be returned in an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.synchronizationSchema"
} -->
```http
HTTP/1.1 200 OK

{
    "directories": [
        {
            "name": "Azure Active Directory",
            "objects": [
                {
                    "name": "User",
                    "attributes": [
                        {
                            "name": "userPrincipalName",
                            "type": "string"
                        }
                    ]
                }
            ]
        },
        {
            "name": "Salesforce",
            "objects": [{}]
        }
    ],
    "synchronizationRules":[
        {
            "name": "USER_TO_USER",
            "sourceDirectoryName": "Azure Active Directory",
            "targetDirectoryName": "Salesforce",
            "objectMappings": [
                {
                    "sourceObjectName": "User",
                    "targetObjectName": "User",
                    "attributeMappings": [
                        {
                            "source": {},
                            "targetAttributeName": "userName"
                        },
                        {}
                    ]
                },
                {}
            ]
        },
        {}
    ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Get synchronizationSchema",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
