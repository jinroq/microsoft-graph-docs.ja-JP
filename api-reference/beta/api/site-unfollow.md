---
author: learafa
title: フォロー取り消しサイト
description: ユーザーのサイトのフォローを取り消します。
localization_priority: Normal
ms.prod: sharepoint
doc_type: apiPageType
ms.openlocfilehash: de1237c26c259eca72b7a800ca1842d9203c7eec
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/25/2019
ms.locfileid: "35869601"
---
# <a name="unfollow-site"></a><span data-ttu-id="c7ff3-103">フォロー取り消しサイト</span><span class="sxs-lookup"><span data-stu-id="c7ff3-103">Unfollow site</span></span> 

<span data-ttu-id="c7ff3-104">ユーザーの[サイト](../resources/site.md)または複数のサイトのフォローを取り消します。</span><span class="sxs-lookup"><span data-stu-id="c7ff3-104">Unfollow a user's [site](../resources/site.md) or multiple sites.</span></span>

## <a name="permissions"></a><span data-ttu-id="c7ff3-105">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="c7ff3-105">Permissions</span></span>

<span data-ttu-id="c7ff3-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="c7ff3-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|            <span data-ttu-id="c7ff3-108">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="c7ff3-108">Permission type</span></span>             | <span data-ttu-id="c7ff3-109">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="c7ff3-109">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :------------------------------------------ |
| <span data-ttu-id="c7ff3-110">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="c7ff3-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="c7ff3-111">Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c7ff3-111">Sites.ReadWrite.All</span></span>                         |
| <span data-ttu-id="c7ff3-112">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="c7ff3-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="c7ff3-113">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="c7ff3-113">Not supported.</span></span>                              |
| <span data-ttu-id="c7ff3-114">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="c7ff3-114">Application</span></span>                            | <span data-ttu-id="c7ff3-115">Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c7ff3-115">Sites.ReadWrite.All</span></span>                         |

## <a name="http-request"></a><span data-ttu-id="c7ff3-116">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="c7ff3-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /users/{user-id}/followedSites/remove
```

## <a name="request-body"></a><span data-ttu-id="c7ff3-117">要求本文</span><span class="sxs-lookup"><span data-stu-id="c7ff3-117">Request body</span></span>

<span data-ttu-id="c7ff3-118">要求本文で、次の表に記載されている id パラメーターを持つ JSON オブジェクトの配列を指定します。</span><span class="sxs-lookup"><span data-stu-id="c7ff3-118">In the request body, supply an array of JSON objects with the id parameter mentioned in the table below.</span></span> 


| <span data-ttu-id="c7ff3-119">名前</span><span class="sxs-lookup"><span data-stu-id="c7ff3-119">Name</span></span>                 | <span data-ttu-id="c7ff3-120">値</span><span class="sxs-lookup"><span data-stu-id="c7ff3-120">Value</span></span>  | <span data-ttu-id="c7ff3-121">説明</span><span class="sxs-lookup"><span data-stu-id="c7ff3-121">Description</span></span>                                                            |
|:---------------------|:-------|:-----------------------------------------------------------------------|
|   <span data-ttu-id="c7ff3-122">id</span><span class="sxs-lookup"><span data-stu-id="c7ff3-122">id</span></span>                 | <span data-ttu-id="c7ff3-123">string</span><span class="sxs-lookup"><span data-stu-id="c7ff3-123">string</span></span> | <span data-ttu-id="c7ff3-124">アイテムの[一意の識別子](../resources/site.md#id-property)。</span><span class="sxs-lookup"><span data-stu-id="c7ff3-124">The [unique identifier](../resources/site.md#id-property) of the item.</span></span> |

## <a name="response"></a><span data-ttu-id="c7ff3-125">応答</span><span class="sxs-lookup"><span data-stu-id="c7ff3-125">Response</span></span>

* <span data-ttu-id="c7ff3-126">要求が成功した場合、このメソッドは`204`コンテンツのない状態コードを返します。</span><span class="sxs-lookup"><span data-stu-id="c7ff3-126">If the request is successful, this method returns a `204` status code with no content.</span></span>  
* <span data-ttu-id="c7ff3-127">指定したサイトのフォローを取り消しているときにエラーが発生した`207`場合、このメソッドは状態コードを返し、応答本文には、[エラーが発生](/graph/errors)していないサイトを示す error オブジェクトと siteids 含むエントリの配列が含まれます。</span><span class="sxs-lookup"><span data-stu-id="c7ff3-127">If an error occured while unfollowing any of the specified sites, this method returns a `207` status code and the response body will contain an array of entries containing [error](/graph/errors) objects and siteIds indicating which sites unable to be unfollowed.</span></span>

## <a name="example"></a><span data-ttu-id="c7ff3-128">例</span><span class="sxs-lookup"><span data-stu-id="c7ff3-128">Example</span></span>

<span data-ttu-id="c7ff3-129">次の例は、複数のサイトをフォローする方法を示しています。</span><span class="sxs-lookup"><span data-stu-id="c7ff3-129">The following example shows how to unfollow multiple sites.</span></span>

### <a name="request"></a><span data-ttu-id="c7ff3-130">要求</span><span class="sxs-lookup"><span data-stu-id="c7ff3-130">Request</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="c7ff3-131">プロトコル</span><span class="sxs-lookup"><span data-stu-id="c7ff3-131">HTTP</span></span>](#tab/http)
<!-- { "blockType": "request", "name": "unfollow-site", "scopes": "sites.readwrite.all" } -->

```http
POST /users/{user-id}/followedSites/remove
Content-Type: application/json

{
    "value":
    [
        {
            "id": "contoso.sharepoint.com,da60e844-ba1d-49bc-b4d4-d5e36bae9019,712a596e-90a1-49e3-9b48-bfa80bee8740"
        },
        {
            "id": "contoso.sharepoint.com,da60e844-ba1d-49bc-b4d4-d5e36bae9019,0271110f-634f-4300-a841-3a8a2e851851"
        }
    ] 
}
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="c7ff3-132">C#</span><span class="sxs-lookup"><span data-stu-id="c7ff3-132">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/unfollow-site-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="c7ff3-133">Javascript</span><span class="sxs-lookup"><span data-stu-id="c7ff3-133">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/unfollow-site-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="c7ff3-134">目的-C</span><span class="sxs-lookup"><span data-stu-id="c7ff3-134">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/unfollow-site-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="c7ff3-135">Java</span><span class="sxs-lookup"><span data-stu-id="c7ff3-135">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/unfollow-site-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

### <a name="response"></a><span data-ttu-id="c7ff3-136">応答</span><span class="sxs-lookup"><span data-stu-id="c7ff3-136">Response</span></span>

<span data-ttu-id="c7ff3-137">成功した場合、次の JSON 応答を返します。</span><span class="sxs-lookup"><span data-stu-id="c7ff3-137">If successful, it returns the following JSON response.</span></span> 

<!-- { "blockType": "response", "@type": "microsoft.graph.site", "isCollection": true, "truncated": true } -->

```json
HTTP/1.1 204 No Content
```

<span data-ttu-id="c7ff3-138">エラーが発生した場合は、次の JSON 応答を返します。</span><span class="sxs-lookup"><span data-stu-id="c7ff3-138">If an error occured, it returns the following JSON response</span></span> 

<!-- { "blockType": "response", "@type": "microsoft.graph.site", "isCollection": true, "truncated": true } -->

```json
HTTP/1.1 207 Multi-Status
Content-type: application/json

{
    "value": [
        {
            "id": "contoso.sharepoint.com,da60e844-ba1d-49bc-b4d4-d5e36bae9019,512a596e-90a1-49e3-9b48-bfa80bee8740",
            "error": {
                "@odata.type": "#oneDrive.error",
                "code": "invalidRequest",
                "message": "The site Id information that is provided in the request is incorrect",
                "innerError": {
                    "code": "invalidRequest",
                    "errorType": "expected",
                    "message": "The site Id information that is provided in the request is incorrect",
                    "stackTrace": "",
                    "throwSite": ""
                }
            }
        }
    ]
}
```  

<!-- {
  "type": "#page.annotation",
  "description": "Unfollow sharepoint site/sites for a user.",
  "keywords": "unfollow site",
  "section": "documentation",
  "tocPath": "Sites/Unfollow site",
  "suppressions": [
  ]
} -->
