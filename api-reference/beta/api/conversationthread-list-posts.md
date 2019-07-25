---
title: 投稿を一覧表示する
description: '指定したスレッドの投稿を取得します。 親の会話とスレッドの両方を指定できます。または、 '
localization_priority: Normal
author: dkershaw10
ms.prod: groups
ms.openlocfilehash: ba48a498738e2b819995e87882dd2194f29c0d0b
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/25/2019
ms.locfileid: "35862909"
---
# <a name="list-posts"></a><span data-ttu-id="e8d78-104">投稿を一覧表示する</span><span class="sxs-lookup"><span data-stu-id="e8d78-104">List posts</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="e8d78-p102">指定したスレッドの投稿を取得します。親の会話とスレッドの両方を指定したり、親の会話を参照せずにスレッドを指定したりすることができます。</span><span class="sxs-lookup"><span data-stu-id="e8d78-p102">Get the posts of the specified thread. You can specify both the parent conversation and the thread, or, you can specify the thread without referencing the parent conversation.</span></span>

## <a name="permissions"></a><span data-ttu-id="e8d78-107">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="e8d78-107">Permissions</span></span>
<span data-ttu-id="e8d78-p103">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="e8d78-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e8d78-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="e8d78-110">Permission type</span></span>      | <span data-ttu-id="e8d78-111">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="e8d78-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="e8d78-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="e8d78-112">Delegated (work or school account)</span></span> | <span data-ttu-id="e8d78-113">グループ読み取り。すべてを取得します。</span><span class="sxs-lookup"><span data-stu-id="e8d78-113">Group.ReadWrite.All, Group.Read.All</span></span>    |
|<span data-ttu-id="e8d78-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="e8d78-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="e8d78-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="e8d78-115">Not supported.</span></span>    |
|<span data-ttu-id="e8d78-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="e8d78-116">Application</span></span> | <span data-ttu-id="e8d78-117">グループ読み取り。すべてを取得します。</span><span class="sxs-lookup"><span data-stu-id="e8d78-117">Group.ReadWrite.All, Group.Read.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="e8d78-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="e8d78-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /groups/{id}/threads/{id}/posts
GET /groups/{id}/conversations/{id}/threads/{id}/posts

```
## <a name="optional-query-parameters"></a><span data-ttu-id="e8d78-119">オプションのクエリ パラメーター</span><span class="sxs-lookup"><span data-stu-id="e8d78-119">Optional query parameters</span></span>
<span data-ttu-id="e8d78-120">このメソッドは、応答をカスタマイズするための [OData クエリ パラメーター](https://developer.microsoft.com/graph/docs/concepts/query_parameters)をサポートします。</span><span class="sxs-lookup"><span data-stu-id="e8d78-120">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="e8d78-121">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="e8d78-121">Request headers</span></span>
| <span data-ttu-id="e8d78-122">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="e8d78-122">Header</span></span>       | <span data-ttu-id="e8d78-123">値</span><span class="sxs-lookup"><span data-stu-id="e8d78-123">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="e8d78-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="e8d78-124">Authorization</span></span>  | <span data-ttu-id="e8d78-p104">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="e8d78-p104">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="e8d78-127">要求本文</span><span class="sxs-lookup"><span data-stu-id="e8d78-127">Request body</span></span>
<span data-ttu-id="e8d78-128">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="e8d78-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="e8d78-129">応答</span><span class="sxs-lookup"><span data-stu-id="e8d78-129">Response</span></span>

<span data-ttu-id="e8d78-130">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で [Post](../resources/post.md) オブジェクトのコレクションを返します。</span><span class="sxs-lookup"><span data-stu-id="e8d78-130">If successful, this method returns a `200 OK` response code and collection of [Post](../resources/post.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="e8d78-131">例</span><span class="sxs-lookup"><span data-stu-id="e8d78-131">Example</span></span>
##### <a name="request"></a><span data-ttu-id="e8d78-132">要求</span><span class="sxs-lookup"><span data-stu-id="e8d78-132">Request</span></span>
<span data-ttu-id="e8d78-133">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="e8d78-133">Here is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="e8d78-134">プロトコル</span><span class="sxs-lookup"><span data-stu-id="e8d78-134">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_posts"
}-->
```http
GET https://graph.microsoft.com/beta/groups/0d75b8dc-c42d-44dd-890a-751a99c0589f/threads/AAQkAD8EJUmcWwTJi06Cew==/posts
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="e8d78-135">C#</span><span class="sxs-lookup"><span data-stu-id="e8d78-135">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-posts-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="e8d78-136">Javascript</span><span class="sxs-lookup"><span data-stu-id="e8d78-136">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-posts-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="e8d78-137">目的-C</span><span class="sxs-lookup"><span data-stu-id="e8d78-137">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-posts-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="e8d78-138">Java</span><span class="sxs-lookup"><span data-stu-id="e8d78-138">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-posts-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="e8d78-139">応答</span><span class="sxs-lookup"><span data-stu-id="e8d78-139">Response</span></span>
<span data-ttu-id="e8d78-p105">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="e8d78-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.post",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "@odata.context":"https://graph.microsoft.com/beta/$metadata#groups('0d75b8dc-c42d-44dd-890a-751a99c0589f')/threads('AAQkAD8EJUmcWwTJi06Cew%3D%3D')/posts",
    "value":[
        {
            "@odata.etag":"W/\"CQAAABYAAAC/3QURwysWS6IJYYw5exv4AAAAAAlK\"",
            "id":"AQMkADgAAAIJbQAAAA==",
            "createdDateTime":"2018-01-11T17:36:17Z",
            "lastModifiedDateTime":"2018-01-11T17:36:17Z",
            "importance": "normal",
            "changeKey":"CQAAABYAAAC/3QURwysWS6IJYYw5exv4AAAAAAlK",
            "categories":[

            ],
            "receivedDateTime":"2018-01-11T17:36:17Z",
            "hasAttachments":false,
            "body":{
                "contentType":"html",
                "content":"<html><body></body></html>"
            },
            "from":{
                "emailAddress":{
                    "name":"Marketing",
                    "address":"Marketing@M365B489948.onmicrosoft.com"
                }
            },
            "sender":{
                "emailAddress":{
                    "name":"Marketing",
                    "address":"Marketing@M365B489948.onmicrosoft.com"
                }
            }
        }
    ]
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "List posts",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
