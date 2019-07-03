---
author: learafa
title: サイトをフォローする
description: ユーザーのサイトまたはサイトをフォローします。
localization_priority: Normal
ms.prod: sharepoint
doc_type: apiPageType
ms.openlocfilehash: 14592ff24e1f88d13184b0f69caf700c895cd9e9
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/02/2019
ms.locfileid: "35453657"
---
# <a name="follow-site"></a><span data-ttu-id="418c5-103">サイトをフォローする</span><span class="sxs-lookup"><span data-stu-id="418c5-103">Follow site</span></span> 

<span data-ttu-id="418c5-104">ユーザーの[サイト](../resources/site.md)または複数のサイトに従います。</span><span class="sxs-lookup"><span data-stu-id="418c5-104">Follow a user's [site](../resources/site.md) or multiple sites.</span></span>

## <a name="permissions"></a><span data-ttu-id="418c5-105">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="418c5-105">Permissions</span></span>

<span data-ttu-id="418c5-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="418c5-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|            <span data-ttu-id="418c5-108">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="418c5-108">Permission type</span></span>             | <span data-ttu-id="418c5-109">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="418c5-109">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :------------------------------------------ |
| <span data-ttu-id="418c5-110">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="418c5-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="418c5-111">Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="418c5-111">Sites.ReadWrite.All</span></span>                         |
| <span data-ttu-id="418c5-112">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="418c5-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="418c5-113">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="418c5-113">Not supported.</span></span>                              |
| <span data-ttu-id="418c5-114">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="418c5-114">Application</span></span>                            | <span data-ttu-id="418c5-115">Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="418c5-115">Sites.ReadWrite.All</span></span>                         |

## <a name="http-request"></a><span data-ttu-id="418c5-116">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="418c5-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /users/{user-id}/followedSites/add
```

## <a name="request-body"></a><span data-ttu-id="418c5-117">要求本文</span><span class="sxs-lookup"><span data-stu-id="418c5-117">Request body</span></span>

<span data-ttu-id="418c5-118">要求本文で、次の表に記載されている id パラメーターを持つ JSON オブジェクトの配列を指定します。</span><span class="sxs-lookup"><span data-stu-id="418c5-118">In the request body, supply an array of JSON objects with the id parameter mentioned in the table below.</span></span> 


| <span data-ttu-id="418c5-119">名前</span><span class="sxs-lookup"><span data-stu-id="418c5-119">Name</span></span>                 | <span data-ttu-id="418c5-120">値</span><span class="sxs-lookup"><span data-stu-id="418c5-120">Value</span></span>  | <span data-ttu-id="418c5-121">説明</span><span class="sxs-lookup"><span data-stu-id="418c5-121">Description</span></span>                                                            |
|:---------------------|:-------|:-----------------------------------------------------------------------|
|   <span data-ttu-id="418c5-122">id</span><span class="sxs-lookup"><span data-stu-id="418c5-122">id</span></span>                 | <span data-ttu-id="418c5-123">string</span><span class="sxs-lookup"><span data-stu-id="418c5-123">string</span></span> | <span data-ttu-id="418c5-124">アイテムの[一意の識別子](../resources/site.md#id-property)。</span><span class="sxs-lookup"><span data-stu-id="418c5-124">The [unique identifier](../resources/site.md#id-property) of the item.</span></span> |


## <a name="response"></a><span data-ttu-id="418c5-125">応答</span><span class="sxs-lookup"><span data-stu-id="418c5-125">Response</span></span> 

* <span data-ttu-id="418c5-126">要求が成功した場合、このメソッドは、フォローされたサイトの配列を返します。</span><span class="sxs-lookup"><span data-stu-id="418c5-126">If the request is successful, this method returns an array of sites that were followed.</span></span>  
* <span data-ttu-id="418c5-127">指定したサイトのフォロー中にエラーが発生した場合、この`207`メソッドは状態コードを返し、応答本文には、フォローできないサイトを示す[Error](/graph/errors)オブジェクトと siteids を含むエントリの配列が含まれます。</span><span class="sxs-lookup"><span data-stu-id="418c5-127">If an error occured while following any of the specified sites, this method returns a `207` status code and the response body will contain an array of entries containing [error](/graph/errors) objects and siteIds indicating which sites were unable to be followed.</span></span>

## <a name="example"></a><span data-ttu-id="418c5-128">例</span><span class="sxs-lookup"><span data-stu-id="418c5-128">Example</span></span>

<span data-ttu-id="418c5-129">次の例は、複数のサイトをフォローする方法を示しています。</span><span class="sxs-lookup"><span data-stu-id="418c5-129">The following example shows how to follow multiple sites.</span></span> 

### <a name="request"></a><span data-ttu-id="418c5-130">要求</span><span class="sxs-lookup"><span data-stu-id="418c5-130">Request</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="418c5-131">プロトコル</span><span class="sxs-lookup"><span data-stu-id="418c5-131">HTTP</span></span>](#tab/http)
<!-- { "blockType": "request", "name": "follow-site", "scopes": "sites.readwrite.all" } -->

```http
POST /users/{user-id}/followedSites/add
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
# <a name="ctabcsharp"></a>[<span data-ttu-id="418c5-132">C#</span><span class="sxs-lookup"><span data-stu-id="418c5-132">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/follow-site-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="418c5-133">Javascript</span><span class="sxs-lookup"><span data-stu-id="418c5-133">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/follow-site-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="418c5-134">目的-C</span><span class="sxs-lookup"><span data-stu-id="418c5-134">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/follow-site-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

### <a name="response"></a><span data-ttu-id="418c5-135">応答</span><span class="sxs-lookup"><span data-stu-id="418c5-135">Response</span></span>

<span data-ttu-id="418c5-136">成功した場合、次の JSON 応答を返します。</span><span class="sxs-lookup"><span data-stu-id="418c5-136">If successful, it returns the following JSON response.</span></span> 

<!-- { "blockType": "response", "@type": "microsoft.graph.site", "isCollection": true, "truncated": true } -->

```json
HTTP/1.1 200 OK
Content-type: application/json

{
    "value": [
        {
            "id": "contoso.sharepoint.com,da60e844-ba1d-49bc-b4d4-d5e36bae9019,712a596e-90a1-49e3-9b48-bfa80bee8740",
            "webUrl": "http://contoso.sharepoint.com/sites/SiteFollowed1",
            "name": "SiteFollowed1",
            "sharepointIds": {
                "siteId": "da60e844-ba1d-49bc-b4d4-d5e36bae9019",
                "siteUrl": "http://contoso.sharepoint.com/sites/SiteFollowed1",
                "webId": "712a596e-90a1-49e3-9b48-bfa80bee8740"
            },
            "siteCollection": {
                "hostname": "contoso.sharepoint.com"
            }
        },
        {
            "id": "contoso.sharepoint.com,da60e844-ba1d-49bc-b4d4-d5e36bae9019,0271110f-634f-4300-a841-3a8a2e851851",
            "webUrl": "http://contoso.sharepoint.com/sites/SiteFollowed2",
            "name": "SiteFollowed2",
            "sharepointIds": {
                "siteId": "da60e844-ba1d-49bc-b4d4-d5e36bae9019",
                "siteUrl": "http://contoso.sharepoint.com/sites/SiteFollowed2",
                "webId": "0271110f-634f-4300-a841-3a8a2e851851"
            },
            "siteCollection": {
                "hostname": "contoso.sharepoint.com"
            }
        }
    ]
}
```

<span data-ttu-id="418c5-137">エラーが発生した場合は、次の JSON 応答を返します。</span><span class="sxs-lookup"><span data-stu-id="418c5-137">If an error occured, it returns the following JSON response</span></span> 

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
        },
        {
            "id": "contoso.sharepoint.com,da60e844-ba1d-49bc-b4d4-d5e36bae9019,0271110f-634f-4300-a841-3a8a2e851851",
            "webUrl": "http://contoso.sharepoint.com/sites/SiteFollowed2",
            "name": "SiteFollowed2",
            "sharepointIds": {
                "siteId": "da60e844-ba1d-49bc-b4d4-d5e36bae9019",
                "siteUrl": "http://contoso.sharepoint.com/sites/SiteFollowed2",
                "webId": "0271110f-634f-4300-a841-3a8a2e851851"
            },
            "siteCollection": {
                "hostname": "contoso.sharepoint.com"
            }
        }
    ]
}
```  

<!-- {
  "type": "#page.annotation",
  "description": "Follow sharepoint site for a user.",
  "keywords": "follow site",
  "section": "documentation",
  "tocPath": "Sites/Follow site",
  "suppressions": [
  ]
} -->
